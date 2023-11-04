---
title: Infinite Fluid Transfer
description: Infinite Fluid Transfer
authors:
  - Jebraltar
date: 2023-09-10
---

# Infinite Fluid Transfer

## Items Required
 - Sink (or other infinite fluid source)
 - Variable Card
 - Logic Cable
 - Fluid Interface
 - Fluid Exporter

## Setting it up

  1. Place a Sink down where you want it
  2. Put the Fluid Interface on the Sink via crouch + right-click
  3. Put a Fluid Exporter on the block you want to export fluid into, also by crouch + right-clicking
  4. Connect the Fluid Interface and Fluid Exporter with Logic Cables
  5. Right-click the Fluid Exporter to open an interface
  6. Insert a Variable Card in the **Export All Fluids** row
  7. Click the **+** icon on the **Export All Fluids** row
  8. Cycle pages with the **>** icon in the top right of the interface to **Fluid Transfer Rate**
  9. Set the value to **2000000000**
  10. Close the interface
  11. Enjoy infinite fluid!

## How it works

The Fluid Interface makes the Sink accessible to the Integrated Dynamics network

The Fluid Exporter exports fluids on the network into the block it is attached to

The Logic Cable connecting the interface and exporter serves as the network

The Variable Card acts as a boolean true value to enable the **Export All Fluids** mode on the Fluid Exporter

<video width='960' height='384' controls>
  <source src='../img/JgeZnCD.mp4' type='video/mp4'>
</video>