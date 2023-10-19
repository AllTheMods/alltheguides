# Updating

!!! Warning "Some information below is only for packs on 1.16 and below"

#### Client: How do I transfer maps/settings/servers when I upgrade the pack?

Copy the relevant files from your old instance to the new one.

- `saves` - Stores your worlds.
- `local` - Stores your FTB Chunks map/waypoints.
- `options.txt` - Stores your graphical, keybinds, and other settings.
- `servers.dat` - For multiplayer, stores your saved servers.

#### Server: How do I upgrade my server to a new pack version?

The initial steps are the same for all hosts.

- BACKUP.
- Download the latest server files zip and extract it to an empty folder.
- Run the `startserver` script and follow the installation instructions.
- Once the installation completes, close the window and delete the newly created `world` folder.

---

#### If you are hosting the pack yourself:

- Follow the initial steps above.
- Go back to your old server folder, and copy `world` to the new server folder.
- If you have customized any configs or `server.properties`, you can copy them also.
    - **WARNING**: Do not copy the entire config folder from your old instance.
We update many configs with each release, some of which will cause crashes or other issues if they are different than what the client has.
We recommend you keep separate documentation of all changes you make to configs, so that you can apply them easily to new versions.

---

#### If you are renting a server from a provider:

- Follow the initial steps above.
- Turn off your old server.
- Delete the Forge jar and the following folders from your old server:
    - configs
    - defaultconfigs
    - kubejs
    - libraries
    - mods
- From the new server folder, upload the Forge jar and that list of folders to your old server.
- If your old server contains server-setup-config.yaml, you should also:
    - Delete the following files from the old server:
        - `server-setup-config.yaml`
        - `serverstarter.lock`
        - `startserver.bat`
        - `startserver.sh`
    - Upload those same files from the new server folder.
- Most providers launch the server with the Forge jar. This is only needed for providers that use the serverstarter script.

> All The Mods | [GitHub](https://github.com/AllTheMods) | [Discord](https://discord.com/invite/allthemods) | [Akliz Server Hosting](https://www.akliz.net/allthemods)