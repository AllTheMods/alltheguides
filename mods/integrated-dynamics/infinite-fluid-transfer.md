# Infinite Fluid Transfer

## Items Required

* Sink (or other infinite fluid source)
* Variable Card
* Logic Cable
* Fluid Interface
* Fluid Exporter

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

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F3fdOeWYnPLrdFAFp4rar%2Fuploads%2F2Qog3KvfK2yXCdnKGDvG%2FidInfiniteTransfer.mp4?alt=media&token=0e8646d6-4431-41db-8ff5-ab993f9f6074" %}

> Integrated Dynamics | [CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/integrated-dynamics)
