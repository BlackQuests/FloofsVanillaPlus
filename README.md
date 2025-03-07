# Floof's Vanilla+
This repository contains a Fabric-based modpack managed via Packwiz.

**Latest supported Minecraft version**: 1.21.4

**Fabric loader version**: 0.16.10

~~**Quilt loader version**: 0.17.8~~ (previous versions)

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
    1. If you made any changes to your versions make sure to close the instance editing screen for changes to apply.
2. Download [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap/releases) and place it in the instance Minecraft folder (.minecraft folder where saves, resourcepacks, etc. are stored).
3. Go to Edit Instance -> Settings -> Custom commands, then check the Custom Commands box and paste the following command into the pre-launch command field:
`"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://blackquests.github.io/FloofsVanillaPlus/pack.toml`
4. Launch the instance and it should start downloading/updating the mods! 
    1. If you get any error about duplicate mods please make sure to delete any older versions of mods you already had installed.
    2. If you get any error about missmatching versions that need to be updated, please re-check step 1.

## Selecting a different version

You can check what versions are available under this repositories' [Branches](https://github.com/BlackQuests/FloofsVanillaPlus/branches/all)

If you wish to use any other version that the latest you can do the following:

1. In MultiMC, click "Edit Instance" on your instance of Floof's Vanilla+
2. In the window that pops up, go to the "Settings" page
3. In the Settings page, go to the "Custom commands" tab
4. Replace the URL in the pre-launch command input (by default this is "https://blackquests.github.io/FloofsVanillaPlus/pack.toml") with the following: 
`https://raw.githubusercontent.com/BlackQuests/FloofsVanillaPlus/<your-desired-version>/pack.toml` where `<your-desired-version>` is the branch name you selected. As an example, this would be the URL for 1.20.2: `https://raw.githubusercontent.com/BlackQuests/FloofsVanillaPlus/1.20.2/pack.toml`
