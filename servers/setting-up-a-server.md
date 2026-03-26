---
description: >-
  This guide will explain how to setup an AllTheMods server locally, or with a
  server host.
---

# Setting up a server

### Prerequisites <a href="#prerequisites" id="prerequisites"></a>

* Server with at least **4GB+** allocated RAM (_As required for most ATM packs_) are recommended. Dependant on your host, you may want to start higher than this.
* The specific [Java](https://allthemods.github.io/alltheguides/help/java/) version based on the pack’s **Minecraft** version.

### Installation

* Go to the **Curseforge** Page of the modpack
* Click on **Files** and chose the version you want to play on
* Scroll down and click on **Additional Files**
* Scroll down again and download the **Server Files**
* Go to your **Download** Folder and extract the **Server-Files.zip** to a folder.

{% hint style="info" %}
If you’ve a 3rd party Anti-Virus installed, exclude the folder the files will be extracted too, as files may get remove or corrupted after extracting.
{% endhint %}

{% hint style="danger" %}
If you are an **Akliz** customer, you will not need to install these files manually, you can install all of our packs on their latest versions directly from their system, by searching \`all the mods\` from [**Here**](https://cc.akliz.net/games/minecraft)
{% endhint %}

#### Java <a href="#java" id="java"></a>

If you have **multiple** [Java](https://allthemods.github.io/alltheguides/help/java/) versions installed, the default `java -version` will be used, which may not be the correct version based on the **Minecraft** version. Either of these solutions will work, you do not have to do all of them.

If you only have **one** [Java](https://allthemods.github.io/alltheguides/help/java/) version installed, you do not have to specify a **Java Path** or **System Environmental Variable**, but specifying the path anyway will ensure you won’t break anything if you ever decide to install another version of java

1. Simply uninstall all [Java](https://allthemods.github.io/alltheguides/help/java/) versions except the one being used.
2. Edit the `startserver` file and change `java` to the desired install-location
   * Ex: `C:\Program Files\Eclipse Adoptium\jdk-21.0.4.7-hotspot\bin\java.exe` [![](https://allthemods.github.io/alltheguides/help/img/setJava.png)](https://allthemods.github.io/alltheguides/help/img/setJava.png)
3. Look for **System Environmental Variable** in your Windows Search bar
   * Under the Tab **Advanced**, click on **Environmental Variables**
   * Under **System Variables**, choose **new**
   * Name it as specified at the top in the **startserver** file (Ex: **ATM10\_Java**)
   * Set **Value** as the install-location of the desired Java version
4. On **Linux**, you can re-configure [Java](https://allthemods.github.io/alltheguides/help/java/) using `sudo update-alternatives --config java`

{% hint style="info" %}
If you’ve just installed [Java](https://allthemods.github.io/alltheguides/help/java/), you may need to restart your OS.
{% endhint %}

#### Local Installation <a href="#local-installation" id="local-installation"></a>

* Extract **Server-Files** to a folder.
* **Window**: Do not unzip files under **OneDrive** or any other cloud folder, as this can potentially remove / corrupt files.
* **Linux**: Ensure server folder has read/write permission, and script has execute permission,
  * To avoid any _read/write_ permission errors, install server under `/home/<user>/` folder.
  * Run once: `sudo chmod +x startserver.sh`.
* Starting Server:
  * **Windows**: Execute `startserver.bat`
  * **Linux**: Execute `./startserver.sh`

The first time you run `startserver` it will generate a bunch of files. **Do not end the installer during this**. If you do so, you might have to start over

After running `serverstart` once, you’re required to accept the [Minecraft Eula](https://www.minecraft.net/en-us/eula) in the `eula.txt` file that was automatically generated, by setting `eula=true`

Make any changes necessary to `server.properties`, `configs`, and or `world/serverconfigs`, and run `startserver.bat/sh` again to start the server.

Once it says **Dedicated server took xx seconds to load** you’re good to go and can join the server

{% hint style="warning" %}
Many guides tell you to edit `server-ip` or `server-port`. In most cases you **DO NOT** need to edit these, especially `server-ip`. This can prevent your server from starting.
{% endhint %}

<details>

<summary>No <code>startserver.bat/sh</code> script?</summary>

Install **NeoForge** first,

* `java -jar neoforge-installer*.jar --installServer`
* You will then instead `run.bat/sh` to start server.

</details>

<details>

<summary>How to add Arguments?</summary>

To add [Arguments](https://allthemods.github.io/alltheguides/help/java/#java-arguments) set them within the `usr_jvm_args.txt` file. Older versions of **Forge** will require adding arguments in the script file, if that file doesn’t exist.

</details>

<details>

<summary>How to increase Ram?</summary>

Edit the `-Xms` (Startup Ram) and `-Xmx` (Maximum Ram) within the `usr_jvm_args.txt` file

</details>

<details>

<summary>How to import a world?</summary>

Upload world folder to server folder. Make sure the world folder is named `world`.

</details>

{% hint style="success" %}
Performance Tips: Check out [Lag / Profiling](https://allthemods.github.io/alltheguides/help/lag/)
{% endhint %}
