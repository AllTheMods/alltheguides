---
title: Commands
description: Known useful commands for most of ATM servers
---

# Commands

??? Info "Useful Minecraft Commands"
    ## Minecraft
    === "Player Commands"
        ```title="Teleport To Spawn"
        /spawn
        ```
        ```title="Forge TPS Count"
        /forge tps
        ```
    === "Admin Commands"
        ```title="Kill/Remove Item Entities"
        /kill @e[type=minecraft:item]
        ```
        ```title="Kill All Entities, Except Players"
        /kill @e[type=!minecraft:player]
        ```

??? Info "Corail Tombstone"
    ## Corail Tombstone
    === "Player Commands"
        ```title="Knowledge GUI"
        /tbgui
        ```
        ```title="Request Teleport To Player"
        /tbrequestteleport <name>
        ```
        ```title="Teleport Binding (Like /sethome)"
        /tbbind set 1-5
        /tbbind teleport 1-5
        ```
        ```title="Teleport to death position"
        /tbteleport death
        ```
    === "Admin Commands"
        ```title="Modify Knowledge Points"
        /tbknowledge
        ```
        ```title="Restore Graves"
        /tbrestoreinventory
        ```
        ```title="Get last graves coordinates"
        /tbshowlastgraves
        ```
        ```title="Restore Graves From Player Backups"
        /tbrcovery
        ```

??? Info "Spark"
    ## Spark
    === "Player Commands"
        ```title="Client Profiling"
        /sparkc profiler --timeout 30
        ```
        ```title="Spark TPS Count"
        /spark tps
        ```
    === "Admin Commands"
        ```title="Server Profiling"
        /spark profiler --timeout 30
        ```
    !!! Tip "`--only-ticks-over 20` argument will record only ticks that's over 20 ticks that's considered problematic"
    !!! Tip "`--thread *` can help record all threads that Spark may not pick up"

??? Info "FTBChunks"
    ## FTBChunks
    === "Admin Commands"
        ```title="Modifiy Claim Chunks Count"
        /ftbchunks admin extra_claim_chunks <player> <set/add> <amount>
        ```
        ```title="Modify Force Loaded Chunks Count"
        /ftbchunks admin extra_force_load_chunks <player> <set/add> <amount>
        ```
        ```title="Bypass Chunk Claims"
        /ftbchunks admin bypass_claims
        ```
        ```title="Unload All Forced Loaded Chunks"
        /ftbchunks admin unload_everything
        ```
        ```title="Unclaim All Chunks (All Team/Player Chunks)"
        /ftbchunks admin unclaim_everything
        ```

??? Info "FTBTeams/Party"
    ## FTBTeams/Party

??? Info "Crash Utilities"
    ## Crash Utilities
    
    === "Admin Commands"
        ```title="Clear Entities (Must be enabled)"
        /cu callItemClear
        ```
        ```title="Get world entities list"
        /cu entities list
        ```
        ```title="Teleport Player (Even Offline) to spawn"
        /cu unstuck <name>
        ```
