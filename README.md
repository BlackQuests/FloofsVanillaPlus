# Floof's Vanilla+
This repository contains a Quilt-based modpack managed via Packwiz.

**Minecraft version**: 1.19.2

**Quilt loader version**: 0.17.3

## Installation

### Installing a fresh instance
Below are instructions on how to add the modpack as a **new** instance to [MultiMC](https://multimc.org/). If you would like to add this modpack to an already existing instance please check the next section.

1. Download [MultiMC](https://multimc.org/) and make sure you are able to run minecraft (install java version 17, login, etc.)
2. Download the latest Floof's Vanilla+ modpack instance from [the latest release](https://github.com/BlackQuests/FloofsVanillaPlus/releases/latest) (download the zip file).
3. Add a new instance to MultiMC, select "Import from zip" and browse to the Modpack .zip from step 2.
4. Add a suitable name to the instance if you want and press "ok" to create the instance. Now every time you launch it should install/update the latest mods.

### Installing to an existing instance
Below are instructions on how to add the modpack to an **existing** [MultiMC](https://multimc.org/) instance. This _should_ allow mods within this modpack to auto-update while you maintain your settings and other mods.

1. Make sure that the instance is running the same _Minecraft_ and _Quilt Loader_ version as detailed above (also make sure that _Intermediary Mappings_ is the same version as _Minecraft_).
2. Download [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap/releases) and place it in the instance Minecraft folder (.minecraft folder where saves, resourcepacks, etc. are stored).
3. Go to Edit Instance -> Settings -> Custom commands, then check the Custom Commands box and paste the following command into the pre-launch command field:
`"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://blackquests.github.io/FloofsVanillaPlus/pack.toml`
4. Launch the instance and it should start downloading/updating the mods! If you get any error about missmatching versions that need to be updated, please re-check step 1.