---
title: All The Modium
description: Dimension customization
authors:
  - Satherov
---

# Customization

---

This page will give you some information on how you can **customize** certain dimensions. The examples all follow the same format where
you should create missing folders. `<root>` refers to the location of your modpack installation.

`path/to/place/the/file/in/example.json`
```json
{
    "Example": "Example"
}
```
In the above example the file should be named `example.json` and be placed at `path/to/place/the/file/in`.

Note: The examples are for `Version 1.21.1` but should also work in `Version 1.20.1`. There is no guarantee that they will work in any other versions.

Head to your modpack's installation folder or your server root and follow the given path.
Create a JSON file with the instructed name, paste the contents given and restart your game / server.

---

## Mining Dimension

### Dimension color

Removes the permanent bright light from the mining dimension

`<root>/kubejs/data/allthemodium/dimension_type/mining.json`
```json
{
  "ultrawarm": false,
  "monster_spawn_block_light_limit": 15,
  "monster_spawn_light_level": 0,
  "natural": true,
  "piglin_safe": false,
  "respawn_anchor_works": false,
  "bed_works": true,
  "has_raids": true,
  "has_skylight": true,
  "has_ceiling": false,
  "coordinate_scale": 1,
  "ambient_light": 0.05,
  "logical_height": 384,
  "effects": "minecraft:overworld",
  "infiniburn": "#minecraft:infiniburn_overworld",
  "min_y": -64,
  "height": 384
}
```

### Grass color

Reduces the brightness of the grass color

`<root>/kubejs/data/allthemodium/worldgen/biome/mining.json`
```json
{
  "temperature": 1,
  "downfall": 0.0,
  "has_precipitation": false,
  "temperature_modifier": "none",
  "category": "none",
  "effects": {
    "fog_color": 12345678,
    "sky_color": 7254527,
    "water_color": 4159204,
    "water_fog_color": 329011,
    "grass_color": 9551193,
    "foliage_color": 7842607
  },
  "spawners": {},
  "spawn_costs": {},
  "carvers": {},
  "features": [
    [],
    [],
    [],
    [],
    [],
    [],
    [],
    [],
    [],
    [],
    []
  ]
}
```

## The Beyond

### Sky color

Makes the sky color appear blue-ish like in the overworld

`<root>/kubejs/data/allthemodium/dimension_type/the_beyond.json`
```json
{
  "temperature": 0.7,
  "downfall": 0,
  "has_precipitation": false,
  "effects": {
    "fog_color": 12638463,
    "sky_color": 7907327,
    "water_color": 4159204,
    "water_fog_color": 329011,
    "grass_color": 9551193,
    "foliage_color": 7842607
  },
  "spawners": {},
  "spawn_costs": {},
  "carvers": {},
  "features": []
}
```
