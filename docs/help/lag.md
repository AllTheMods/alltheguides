---
title: Lag / Profiling
description: Find and Fix server lag, and or FPS issues
---

# Lag

For identifying Lag sources/causes most of our packs have Spark and Observable in them by Default.

### [Spark Profiler](https://spark.lucko.me/docs)

Normal players also have access to the command `/spark tps` & `/forge tps` and that gives a general indication of any potential lag issues that might need investigating.

**For Spark**, players in SP worlds with cheats enabled, or Server OPs can use the command `/spark profiler --timeout 180` to get a 3 minute snapshot of the server and anything that could be causing TPS issues. You can look at the URL returned by the mod to see an interactive online view of all server threads.
Users can also use the command `/spark profiler --only-ticks-over 100 --timeout 60`, to identify intermittent lag spikes.

!!! Note
    For profiling client side FPS issues, use the `sparkc` command instead using same arguments above.

---

### [Observable](https://www.curseforge.com/minecraft/mc-mods/observable)

Observable has the same permission requirements, but users need to set a keybind in their Keybinds settings to open the UI, from there click the profile TPS button and wait for it to complete, then depending on the mc version, you will either get a url, or an in-game table listing what blocks/entities are costing the most TPS, it will also visually highlight blocks with a spectrum color coding from **Green** to **Red**, with things colored in red generally being the worst for performance.

Observable is an in-game profiler can be used  as OP (_must create keybind_)

### [Crash Utilities](https://legacy.curseforge.com/minecraft/mc-mods/crash-utilities) (Item Clear)

By default, **Crash Utilities** comes with most of our packs, though one feature **Item Clear** is disabled. It's a very handy feature to have enabled with packs containing farms and automation to prevent massive entity leaks, which causes lag & crashes. This can keep your server entity count low for better performance.
    
To enable, locate and open `world/serverconfigs/crashutilities-server.toml`. Very top section, set `enabled` to `true`. The `timer` is the amount of time in minutes entities will be checked, followed by an Item Clear chat announcement when the entities goes over the `maximum` threshold.

!!! Warning "When editing configs, please make sure server / client is not running"

    For clients, it's safe to edit `world/serverconfigs/` while not in the world and or restarting entire client.


### Useful Commands

??? Note "General Commands"

    ``` title="Kill Item Entities (Or Specific Entity)"
    /kill @e[type=minecraft:item]
    ```

    ``` title="Kill Everything, Except Players"
    /kill @e[type=!minecraft:player]
    ```

??? Note "Spark"

    ``` title="Run Server Side Profiler (TPS Issues)"
    /spark profiler --timeout 30
    ```

    ``` title="Run Client Side Profiler (FPS/TPS Issues)"
    /sparkc profiler --timeout 30 
    ```

    !!! Tip "`--only-ticks-over 20` argument will record only ticks that's over 20 that's considered problematic."
    !!! Tip "`--thread *` can help record all threads Spark may not pick up."

??? Note "Crash Utilities Commands"

    ``` title="Entities List"
    /cu entities list
    ```

    ``` title="Item Clear (Must Be Enabled)"
    /cu callItemClear
    ```

    ``` title="Teleport Player To Spawn (Even Offline Player(s))"
    /cu unstuck <name>
    ```

    ``` title='Open Player Inventory (Even Offline Player(s))'
    /cu inventory <name>
    ```


