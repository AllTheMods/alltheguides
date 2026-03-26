# AMP Install Guide

This is a guide for installing ATM10 (and possibly other packs) on CubeCoderz’s AMP gameserver hosting software!

<details open>

<summary>Info</summary>

The current version of AMP as of the creation of this guide is **2.6.0.12**. As the software is updated, the exact location of settings may change.

</details>

<details open>

<summary>Warning</summary>

This guide is currently hosted by the official ATM website/Discord. If found anywhere else please advise them to delete it and instead link to this [official version](https://allthemods.github.io/alltheguides/help/server/).

</details>

<details open>

<summary>This guide assumes:</summary>

* You have fully installed the AMP software and have successfully gained access to the web based GUI. If you need help installing the base software please refer to the [CubeCoderz Documentation](https://github.com/CubeCoders/AMP/wiki).
* You have already downloaded the latest version of the [ATM Pack ServerFiles](https://legacy.curseforge.com/members/atmteam/projects) and have unzipped them into a folder.

</details>

### Creating a New Instance. <a href="#creating-a-new-instance" id="creating-a-new-instance"></a>

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS1.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS1.png)

* Under **Select Application**, choose **Minecraft Java Edition**.
* Under **Friendly Name**, pick a name to reference the server such as **ATM10**.
* Under **After Creation**, pick **Do Nothing**.
  * If you do not want the instance to start every time AMP is started, uncheck the **Start Instance on Boot** option. This is **ON** by default.
* Select **Create Instance**

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS2.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS2.png)

***

### Configuring Server Settings <a href="#configuring-server-settings" id="configuring-server-settings"></a>

* Choose **Manage** from the newly created instance

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS3.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS3.png)

* On the left menu, select **Configuration** and then **Minecraft**

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS4.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS4.png) [![](https://allthemods.github.io/alltheguides/help/server/img/ampSS4\(2\).png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS4\(2\).png)

* The tabs on the top show the different categories

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSSTabs.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSSTabs.png)

***

#### Java and Memory <a href="#java-and-memory" id="java-and-memory"></a>

* **Memory Limit (MB)**: Min: `6144`. Max: `16384`.
  * `12000`+ is recommended for multiple players.
* **Additional java options**: Paste in the server java arguments (this example uses the advanced ZGC arguments)

`-XX:+UseZGC -XX:+ZGenerational -XX:SoftMaxHeapSize=6g -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:+PerfDisableSharedMem -XX:+UseDynamicNumberOfGCThreads`

* **Java Version**: `Java 21`

<details open>

<summary>Note</summary>

If `Java 21` is not in the dropdown list, you need to close AMP completely, install `Java 21` on the server, then restart AMP.

</details>

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS9.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS9.png)

***

#### Server and Startup <a href="#server-and-startup" id="server-and-startup"></a>

* **Server type**: `NeoForge`
* **Enable TPS Monitoring**: `Off`
* **NeoForge Version**: Change to current NeoForge version.
  * For this example the current version is `21.1.119`.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS5.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS5.png)

***

#### Network <a href="#network" id="network"></a>

Make no changes

***

#### Gameplay and Difficulty <a href="#gameplay-and-difficulty" id="gameplay-and-difficulty"></a>

* **Difficulty**: Normal (or personal preference)
* **Op permission level**: `3: Kick/ban/op players`
* **Spawn Protection Radius**: `1` (or personal preference)
* **Allow Flight**: `on`
* **Allow Command Blocks**: `on`

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS6.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS6.png)

***

#### Security <a href="#security" id="security"></a>

Make no changes

***

#### Sleep Mode <a href="#sleep-mode" id="sleep-mode"></a>

* **Enable sleep mode**: `off`

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS7.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS7.png)

***

#### System Settings <a href="#system-settings" id="system-settings"></a>

* **Console Scrollback Period**: `120`

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS8.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS8.png)

***

### Installing Server NeoForge <a href="#installing-server-neoforge" id="installing-server-neoforge"></a>

Click the **Back** arrow at the top of the left menu.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS11.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS11.png)

Select **Console** from the left menu and then click the orange **Update** icon from the middle screen.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS12.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS12.png)

Wait while the server downloads and installs the selected NeoForge version.

This can take several minutes depending on your server specs and internet connection.

When it finishes, it should say **The server installed successfully**. If it doesn’t, please doublecheck the above settings and verify you have selected the appropriate NeoForge Version.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS13.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS13.png)

***

### Importing the Server Files <a href="#importing-the-server-files" id="importing-the-server-files"></a>

**1.** On the left menu, select **File Manager**.

**1.1** The easiest way to import the server files is to unzip the files and create a new zip.

<details open>

<summary>Removing Double-Wrapping</summary>

To remove the double-wrapping (zipping a folder instead of a group of files) of the files:

* **Extract** the server files you downloaded from CurseForge into a folder.
* Go into the folder inside that folder and then select **all the files** and re-zip them without the containing folder.

</details>

I recommend using **7zip** as this is what I have used for testing.

Make sure you save as .zip and not .7z

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS14.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS14.png)

***

**2.** Drag the newly created zip file into the **File Manager window**. Once it finishes you may need to refresh the page to see the file in the file list.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS15.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS15.png)

***

**3.** Right click the .zip file in the list and chose **Extract Here**.

This may take several minutes depending on your server specs and storage speed.

**4.** Once it finishes you may need to **refresh** the page to see the newly extracted files populated in the list.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS16.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS16.png) [![](https://allthemods.github.io/alltheguides/help/server/img/ampSS17.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS17.png)

***

### Starting the Server <a href="#starting-the-server" id="starting-the-server"></a>

Select **Console** from the left menu and click the green **Start** icon.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS18.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS18.png)

* Accept the EULA that pops up.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS19.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS19.png)

***

The server will now start. This can take several minutes depending on your server specs and storage speed.

<details open>

<summary>Note</summary>

Errors are normal and to be expected as long as it continues loading. Be patient as the first startup usually takes time while it creates all the needed files/configs/folders/etc.

</details>

You will know it is finished when the notification window in the bottom right disappears and the server says **Dedicated server took XXX.XX seconds to load**.

[![](https://allthemods.github.io/alltheguides/help/server/img/ampSS20.png)](https://allthemods.github.io/alltheguides/help/server/img/ampSS20.png)

***

It is recommended after the first startup, to stop the server using the red **Stop** button at the top, and then start it again.

* Try to connect to the server and verify operation.
* If you need to add server admin mods, you would place them inside the **mods** folder under **File Manager** while the server is _**stopped**_; you can edit files directly from within the file manager in AMP for making changes to the txt config files.

Only edit, add, or remove files WHILE THE SERVER IS STOPPED!

***

### Changing Server Properties <a href="#changing-server-properties" id="changing-server-properties"></a>

CHANGES TO `server.properties` FILE WILL NEVER SAVE!

All settings within `server.properties` are in independent tabs in the various settings in AMP and it is recreated every server startup.

<details open>

<summary>Changing Server Type</summary>

If you need to edit the world type for example, to run a **Skyblock** server, you would change it under `Configuration > Minecraft > Server and Startup`.

</details>
