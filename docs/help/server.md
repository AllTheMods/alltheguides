# Server

This guide will explain how to setup an AllTheMods server locally, or with a server host.

---

## Prerequisites

- Server with at-least **8GB**+ RAM (As required for most ATM packs).
- Specific [Java](java.md) version, based on pack **Minecraft** version.
    - _Azul Zulu, Adoptium, Eclipse Temurin, Amazon Corretto, or Oracle JDK works_
- CPU that's atleast **3.5Ghz** of speed.

---

## Installation

- Download pack Server-Files from **CurseForge**.

--- 

### Local Installation

!!! Warning "**Windows**: If you have 3rd party Anti-Virus installed, exclude the folder the server will be installed in, as files may get remove or corrupted after extracting Server-Files."

- Extract downloaded Server-Files to a folder.
- **Window**: Do not unzip files under **OneDrive** or any other cloud folder, as this can potentially remove / corrupt files.
- **Linux**: Ensure server folder has read/write permissions, and the script has execute permissions,
    - `sudo chmod -R 775 /path/to/server/`
    - `sudo chmod +x startserver.sh`
- Starting Server: 
    - **Windows**: Run `startserver.bat`
    - **Linux**: Run `./startserver.sh`

After running, you would be required to accept [Minecraft Eula](https://www.minecraft.net/en-us/eula) in the `eula.txt` file.

??? Note "There's no `startserver.bat/sh` script?"
    Install **Forge** first,

    - `java -jar forge-installer*.jar --installServer`
    - You will then instead `run.bat/sh` to start server.

    ??? Tip "There's no `run.bat/sh`?"
        Expecting this is an older Forge version, you'll need to create a script that launches Forge.
        ``` title='run.bat/sh'
        java -Xms4G -Xmx8G -jar forge-*universal.jar
        ```

??? Note "How to allocate RAM or add Arguments?"
    Allocating RAM and or adding Arguments are applied within `usr_jvm_args.txt`. Older versions of **Forge** will require adding arguments in the script file, if that file doesn't exist.

---

### Server Host Installation

Most server host has a one-click server installer you can use, otherwise

- Setup a fresh **Forge** server based on the current **Forge** version of the pack.
    - If host has no **Forge** installer, read [Server Host Custom Jar](#server-host-custom-jar)
- Upload extracted Server-Files to host, via **FTP** or **STFP**.
    - If there's no **FTP** or **SFTP**, you may be able to upload the zip file, and extract on server host. 
 

---

## Server Host Custom Jar

If server host requires a `.jar` file, later **Forge** versions cannot be ran directly. If older, you can upload and run the `forge-*universal.jar` file. Otherwise,

- Download [ServerStarter](https://github.com/BloodyMods/ServerStarter/releases) jar and upload to server root folder and select this as the custom jar.
- Download Server Files from CurseForge, extract, and upload files to server.

Create a file named (`server-setup-config.yaml`), and copy / paste the config example below. 

Modifiy config for pack if necessary, specifically the `mcVersion` and `loaderVersion`, and place config in server root then start server as normal.

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

    
!!! Tip "Performance Tips: Check out [Lag / Profiling](lag.md)"
---

## Updating

Updating ATM servers is pretty simple. There's 3 ways you can accomplish this. Make sure you **BACKUP** world folder before proceeding.

### **Automatic**

1. If you have a server host with a modpack installer, usually you can do a one click pack update within your control panel.

### **Manually**

1. Delete `kubejs`, `defaultconfigs`, `mods`, and `config` folder.
    - Download Server Files from CurseForge
    - If previous pack forge version is different, delete `libraries` folder, and copy over new `startserver.bat/sh` from Server Files, and `forge-installer.jar` if exists.
    - Extract the deleted folders from Server Files into your server folder.

2. Download Server Files from CurseForge.
    - Extract Server Files into a new folder.
    - Copy your `world` folder, and `server.properties` to new folder.
    - If JourneyMap exists, copy `journeymap` folder aswell.

---

#### Other Stuff

- Importing a single player world
    - Shut off the server.
    - Delete `world` from the server.
    - Copy your save into the server directory, and rename it to `world`.
    - Delete `world/icon.png` (single player worlds can sometimes generate icons that are too large for the server)

> All The Mods | [GitHub](https://github.com/AllTheMods) | [Discord](https://discord.com/invite/allthemods) | [Akliz Server Hosting](https://www.akliz.net/allthemods)
