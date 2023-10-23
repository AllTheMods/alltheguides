---
title: Java
description: Get the right Java you need!
---

# Java

### Java Versions

- Minecraft **<= 1.15** | [Java 8](https://adoptium.net/?variant=openjdk8&jvmVariant=hotspot) | `sudo apt install openjdk-8-jdk`
- Minecraft **1.16**  | [Java 8](https://adoptium.net/?variant=openjdk8&jvmVariant=hotspot) OR [Java 11](https://adoptium.net/?variant=openjdk11&jvmVariant=hotspot) | `sudo apt install openjdk-11-jdk`
- Minecraft **1.17** | [Java 16](https://adoptium.net/?variant=openjdk16&jvmVariant=hotspot) | `sudo apt install openjdk-16-jdk`
- Minecraft **1.18+** | [Java 17](https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot) | `sudo apt install openjdk-17-jdk`

??? Note "Other Java Download Links"
    [Amazon Corretto](https://aws.amazon.com/corretto/), [Azul Zulu](https://www.azul.com/downloads/?package=jdk#zulu), or [Oracle JDK](https://www.oracle.com/java/technologies/downloads/archive/)

---

### Java Arguments

These can help both server and client with performance in,

- Reducing Ram Usage. (_GC will clean up more efficiently_)
- Reduced Lag Spikes. (_GC will clean more frequently, reducing large lag spikes_)

``` title="Java 8+ Arguments"
-XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=32M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true
```

---

??? Java Arguments Explanation

    - `UnlockExperimentalVMOptions`

    : Needed for some the below options

    - `G1NewSizePercent`

    : These are the important ones. You now can specify percentages of an overall desired range for the new generation. With these settings, we tell G1 to not use its default 5% for new gen, and instead give it 40%! **Minecraft has an extremely high a memory allocation rate, ranging to at least 800 Megabytes a second on a 30 player server! And this is mostly short-lived objects (Block Position).**

    - `G1MixedGCLiveThresholdPercent`

    : Controls when to include regions in Mixed GC's in the Young GC collection, keeping Old Gen tidy without doing a normal Old Gen GC collection. When your memory is less than this percent, old gen won't even be included in 'mixed' collections. Mixed are not as heavy as a full old collection, so having small incremental cleanups of old keeps memory usage light.

    : Default is 65 to 85 depending on Java Version, we are setting to 90 to ensure we reclaim garbage in old gen as fast as possible to retain as much free regions as we can.

    - `G1ReservePercent=20`

    : MC Memory allocation rate in up-to-date versions is really insane. We run the risk of a dreaded "to-space exhaustion" not having enough memory free to move data around. This ensures more memory is waiting to be used for this operation. Default is 10, so we are giving another 10 to it.

    - `MaxTenuringThreshold=1`

    : Minecraft has a really high allocation rate of memory. Of that memory, most is reclaimed in the eden generation. However, transient data will overflow into survivor. Initially played with completely removing Survivor and had decent results, but does result in transient data making its way to Old which is not good.Max Tenuring 1 ensures that we do not promote transient data to old generation, but anything that survives 2 passes of Garbage Collection is just going to be assumed as longer-lived.

    : Doing this greatly reduces pause times in Young Collections as copying data up to 15 times in Survivor space for a tenured object really takes a lot of time for actually old memory. Ideally the GC engine would track average age for objects instead and tenure out data faster, but that is not how it works.

    : Considering average GC rate is 10s to the upwards of minutes per young collection, this does not result in any 'garbage' being promoted, and just delays longer lived memory to be collected in Mixed GC's.

    - `SurvivorRatio=32`

    : Because we drastically reduced MaxTenuringThreshold, we will be reducing use of survivor space drastically. This frees up more regions to be used by Eden instead.

    - `AlwaysPreTouch`

    : AlwaysPreTouch gets the memory setup and reserved at process start ensuring it is contiguous, improving the efficiency of it more. This improves the operating systems memory access speed. Mandatory to use Transparent Huge Pages.

    - `+DisableExplicitGC`

    : Many plugins think they know how to control memory, and try to invoke garbage collection. Plugins that do this trigger a full garbage collection, triggering a massive lag spike. This flag disables plugins from trying to do this, protecting you from their bad code.

    - `MaxGCPauseMillis=200`

    : This setting controls how much memory is used in between the Minimum and Maximum ranges specified for your New Generation. This is a "goal" for how long you want your server to pause for collections. 200 is aiming for at most loss of 4 ticks. This will result in a short TPS drop, however the server can make up for this drop instantly, meaning it will have no meaningful impact to your TPS. 200ms is lower than players can recognize. In testing, having this value constrained to an even lower number results in G1 not recollecting memory fast enough and potentially running out of old gen triggering a Full collection. Just because this number is 200 does not mean every collection will be 200. It means it can use up to 200 if it really needs it, and we need to let it do its job when there is memory to collect.

    - `+ParallelRefProcEnabled`

    : Optimizes the GC process to use multiple threads for weak reference checking. Not sure why this isn't default...

    - `G1RSetUpdatingPauseTimePercent=5`

    : Default is 10% of time spent during pause updating Rsets, reduce this to 5% to make more of it concurrent to reduce pause durations.

    - `G1MixedGCCountTarget=4`

    : Default is 8. Because we are aiming to collect slower, with less old gen usage, try to reclaim old gen memory faster to avoid running out of old.

    - `G1HeapRegionSize=8M+`

    : Default is auto calculated. SUPER important for Minecraft, especially 1.15, as with low memory situations, the default calculation will in most times be too low. Any memory allocation half of this size (4MB) will be treated as "Humongous" and promote straight to old generation and is harder to free. If you allow java to use the default, you will be destroyed with a significant chunk of your memory getting treated as Humongous.

    - `+PerfDisableSharedMem`

    : Causes GC to write to file system which can cause major latency if disk IO is high -- See [JVM MMAP Pause](https://www.evanjones.ca/jvm-mmap-pause.html)

    : **Note**: This argument can prevent **VisualVM** from detecting the Java process.


    - Using Large Pages

    : For Large Pages -- It's even more important to use -Xms = -Xmx! Large Pages needs to have all the memory specified for it, or you could end up without the gains. This memory will not be used by the OS anyway, so use it. Additionally, use these flags (Metaspace is Java 8 Only, don't use it for Java7): 
    
    : `-XX:+UseLargePagesInMetaspace`

    - Transparent Huge Pages

    : Controversial feature but may be usable if you can not configure your host for real HugeTLBFS. Try adding `-XX:+UseTransparentHugePages` but it's extremely important you also have AlwaysPreTouch set. Otherwise, THP will likely hurt you. We have not measured how THP works for MC or its impact with AlwaysPreTouch, so this section is for the advanced users who want to experiment.