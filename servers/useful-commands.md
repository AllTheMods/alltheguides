# Useful Commands

<details>

<summary>Useful Minecraft Commands</summary>

### Minecraft <a href="#minecraft" id="minecraft"></a>

**Teleport to spawn**

```
/spawn
```

**Kill/Remove Item Entities**

```
/kill @e[type=minecraft:item]
```

**Kill All Entities, Except Players**

```
/kill @e[type=!minecraft:player]
```

**Clear Inventory**

```
/clear
```

**TPS Count**

```
/forge tps OR /neoforge tps
```

</details>

<details>

<summary>Spark</summary>

### Spark <a href="#spark" id="spark"></a>

```
/sparkc profiler --timeout 30
```

Spark TPS Count

```
/spark tps
```

Server Ping

```
/spark ping
```

`--only-ticks-over 20` argument for profiling will record only ticks that’s over 20 ticks that’s considered problematic

`--thread *` for profiling can help record all threads that Spark may not pick up



Server Profiling

```
/spark profiler --timeout 30
```

Server Health

```
/spark health
/spark health --memory
/spark health --network
```

Tick Monitoring

```
/spark tickmonitor
/spark tickmonitor --threshold <percent>
/spark tickmonitor --threshold-tick <milliseconds>
/spark tickmonitor --without-gc
```

Spark Garbage Collection History

```
/spark gc
```

Garbage Collection Monitor

```
/spark gcmonitor
```

Spark Heap Summary

```
/spark heapsummary
```

Spark Heap Dump

```
/spark heapdump
```

Past Spark Activity/History

```
/spark activity
```

</details>

<details>

<summary>FTBChunks</summary>

### FTBChunks <a href="#ftbchunks" id="ftbchunks"></a>

**Admin Commands**

Modify Claimed Chunks Count

```
/ftbchunks admin extra_claim_chunks <player> <set/add> <amount>
```

Modify Force Loaded Chunks Count

```
/ftbchunks admin extra_force_load_chunks <player> <set/add> <amount>
```

Bypass Chunk Claims

```
/ftbchunks admin bypass_claims
```

Unload All Forced Loaded Chunks

```
/ftbchunks admin unload_everything
```

Unclaim All Chunks (All Team/Player Chunks)

```
/ftbchunks admin unclaim_everything
```

</details>

<details>

<summary>FTBQuests</summary>

FTBQuests Edit Mode

```
/ftbquests editing_mode true
```

</details>

<details>

<summary>Crash Utilities</summary>

### Crash Utilities[¶](https://allthemods.github.io/alltheguides/help/commands/#crash-utilities) <a href="#crash-utilities" id="crash-utilities"></a>

Clear Entities (Must be enabled in configs)

```
/cu callItemClear
```

Get world entities list

```
/cu entities list
```

Teleport Player (Even Offline) to spawn

```
/cu unstuck <name>
```

</details>

<details>

<summary>Mahou Tsuaki</summary>

### Mahou Tsuaki[¶](https://allthemods.github.io/alltheguides/help/commands/#mahou-tsuaki) <a href="#mahou-tsuaki" id="mahou-tsuaki"></a>

MahouSet Morgan Damage

```
/mahouset morgan @p 5000000
```

Show/Hide Mahou Count

```
/showmahou
```

</details>

<details>

<summary>Corail Tombstone</summary>

### Corail Tombstone[¶](https://allthemods.github.io/alltheguides/help/commands/#corail-tombstone) <a href="#corail-tombstone" id="corail-tombstone"></a>

Knowledge GUI

```
/tbgui
```

Request Teleport To Player

```
/tbrequestteleport <name>
```

Teleport Binding (Like /sethome)

```
/tbbind set 1-5
/tbbind teleport 1-5
```

Teleport to death position

```
/tbteleport death
```

</details>
