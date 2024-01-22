# Mekanism

To get started in **Mekanism** you just need **coal**, **osmium**, **redstone** and **iron** to make some **steel**. The Official [Mekanism Wiki](https://wiki.aidancbrady.com/wiki/Main_Page) has a lot of information on the setup of machines and how they can be used. Also, the Surviving with **Mekanism** series by **RagePlaysGames** is top notch! Every video has chapters so you can easily skip to the section you need, and each video is divided into **intro**, **mats**, **crafting**, **building**, and **how to use**. You can't go wrong.


![type:video](https://www.youtube.com/embed/EC6S9k54Mp4?si=2BwdTw8O5G_xeDz5)

??? Tip "Fission Reactor Diagram"

    ```mermaid
    graph TD
    W(((Water))) --> ES_O[Electrolytic Separator]
    S(((Sulfur))) --> CO_SD[Chemical Oxidizer]
    U(((Uranium)))
    ES_O -- Oxygen --> CO_SD -- Sulfur Dioxide --> CI_ST[Chemical Infuser]
    W --> RC_WV[Rotary Condensentrator]
    CI_ST -- Sulfur Trioxide --> CI_SA[Chemical Infuser]
    RC_WV -- Water Vapor --> CI_SA
    F(((Fluorite))) --> CDC_HA[Chemical Dissolution Chamber]
    CI_SA -- Sulfuric Acid --> CDC_HA
    CDC_HA -- Hydrofluoric Acid --> CI_UH[Chemical Infuser]

    U ----> EC_YCU[Electrolytic Separator]
    EC_YCU -- Yellow Cake Uranium --> CO_UO[Chemical Oxidizer]
    CO_UO -- Uranium Oxide --> CI_UH

    CI_UH -- Uranium Heaxfluoride --> IC_FF[Isotopic Centrifuge]
    IC_FF -- Fissile Fuel --> R{REACTOR}
    ```


!!! Warning  "Accidentally leaked radiation? `/mek radiation removeAll`, `/mek radiation heal`"

> Mekanism | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/mekanism)