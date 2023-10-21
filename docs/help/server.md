# Server
> _This is not meant to be a comprehensive guide, just a general overview of the process._

---

This guide is targeted for **Windows**, and **Linux** Distributions.

---

#### Prerequisites

- Depending on Minecraft version, make sure the proper [Java](java.md) version is being used.
    - _Azul Zulu OpenJDK, Adoptium, Amazon Corretto, or Oracle JDK all works._
- Ensure any third-party antivirus programs are disabled or uninstalled.
    - _**Avast**, **AVG**, and **BitDefender** are known to interfere in the process - others are also likely to cause problems._

---

#### Installation

- Go to the CurseForge page for the pack version you want to install, and download the Server Files
- Unzip these to an empty folder.
    - **Windows**: Make sure you do **NOT** install server under a **OneDrive** directory or other synced folder, as this can break installers and corrupt server files
    - **Linux**: Make sure server folder/files have read/write permissions.
- Run `startserver.bat/sh` and wait for it to complete. When the installation is complete, you should see a prompt to accept the **EULA**.
    - If there's no `startserver` script, install **Forge** that comes with the pack.
        - `java -jar forge-installer*.jar --installServer`
    - **Linux**: Sometimes files don't have executable permissions when running `./script.sh`. To fix, run `sudo chmod +x script.sh` once, then run `./script.sh`  
    - Some cases with servers having multiple [Java](java.md) versions installed, the server may not run with the correct version, instead another version defined in **System Environment Variables**. You could,
        - Edit the script(s) to reflect the correct Java path/binary file.
        - Update **System Environment Variables**, or **Linux** configure Java.
    - Do **NOT** run server as an **Administrator**, or with **sudo** / **root** privileges.
- Once you've accept **EULA** in `eula.txt` file, the server will start running. Startup will typically take 3-5 minutes.
- Make any changes needed to `server.properties`, `configs`, and or `world/serverconfigs`, and run `startserver.bat/sh` again to start the server.
    - You may want to delete `world` folder to regenerate world again if changes made. 
    - If importing a world, delete `world` folder, copy your world folder over, and rename it `world`.
    - _Many guides tell you to edit `server-ip` or `server-port`. In most cases you **DO NOT** need to edit these, especially `server-ip`. This can prevent your server from starting._
    
!!! Tip "Performance Tips: Check out [Lag / Profiling](lag.md)"
---

#### Updating

Updating ATM servers is pretty simple. There's 3 ways you can accomplish this.

##### **Automatic**

1. If you have a server host with a modpack installer, usually you can do a one click pack update within your control panel.

##### **Manually**

1. Download Server Files from CurseForge
    - Delete `kubejs`, `defaultconfigs`, `mods`, and `config` folder.
    - If previous pack forge version is different, delete `libraries` folder, and copy over new `startserver.bat/sh` from Server Files, and `forge-installer.jar` if exists.
    - Extract the deleted folders from Server Files into your server folder.

2. Download Server Files from CurseForge.
    - Extract Server Files into a new folder.
    - Copy your `world` folder, and `server.properties` to new folder.
    - If JourneyMap exists, copy `journeymap` folder aswell.


---

#### Server Host Custom Jar

If your host requires a `.jar` file, in later versions you cannot run forge directly from a `.jar` file. You would need to use [ServerStarter](https://github.com/BloodyMods/ServerStarter/releases). 

Download and upload this to your host. Additionally, you'll need to create a config for **ServerStarter** for it to know how to properly install and run your server.

??? Info "Config Example | ATM9"

    !!! Warning "Highlighted lines are imported to be configured"

    ```yaml title='server-setup-config.yaml' hl_lines="4 5 7 8 30"
    # Version of the specs, only for internal usage if this format should ever change drastically
    _specver: 2
    modpack:
        name: ATM9
        description: All The Mods 9
    install:
        mcVersion: 1.20.1
        loaderVersion: 47.1.3
        installerUrl: "https://files.minecraftforge.net/maven/net/minecraftforge/forge/{{@mcversion@}}-{{@loaderversion@}}/forge-{{@mcversion@}}-{{@loaderversion@}}-installer.jar"
        installerArguments:
            - "--installServer"
        modpackFormat: zip
        baseInstallPath: ~
        checkFolder: true
        installLoader: true
        connectTimeout: 30
        readTimeout: 30
    launch:
        crashLimit: 10
        maxRam: 8
        minRam: 4
        crashTimer: 60min
        preJavaArgs: ~
        startFile: "forge-{{@mcversion@}}-{{@loaderversion@}}.jar"
        startCommand:
            - "@user_jvm_args.txt"
            - "@libraries/net/minecraftforge/forge/{{@mcversion@}}-{{@loaderversion@}}/{{@os@}}_args.txt"
            - "nogui"
        forcedJavaPath: ~
        supportedJavaVersions: [17]
    ```

    ###### mcVersion
    : Minecraft Version

    ###### loadVersion
    : Forge Version

    ###### supportedJavaVersions
    : Support Java Version(s)

---

#### Other Stuff

- Importing a single player world
    - Shut off the server.
    - Delete `world` from the server.
    - Copy your save into the server directory, and rename it to `world`.
    - Delete `world/icon.png` (single player worlds can sometimes generate icons that are too large for the server)

> All The Mods | [GitHub](https://github.com/AllTheMods) | [Discord](https://discord.com/invite/allthemods) | [Akliz Server Hosting](https://www.akliz.net/allthemods)