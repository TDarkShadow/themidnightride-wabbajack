# The Midnight Ride - Wabbajack port <!-- omit in toc -->

## MODLIST SUMMARY <!-- omit in toc -->

 The Midnight Ride is a lite modlist that tries to stay as close as possible to vanilla, but provides a stable, smooth, and most importantly, enjoyable experience. The guide is highly accessible for everyone, no matter your prior modding experience. You can find the manual guide at <https://themidnightride.github.io>. This modlist functions as a one-click install of the guide. The list improves Fallout 4 with increased performance, bugfixes, gameplay improvements, and quality of life tweaks.

## TABLE OF CONTENTS <!-- omit in toc -->
- [REQUIREMENTS](#requirements)
- [PREPARATION](#preparation)
  - [Installing Microsoft Visual C++ Redistributable Package](#installing-microsoft-visual-c-redistributable-package)
  - [Uninstalling the game](#uninstalling-the-game)
  - [Making a new Steam Library](#making-a-new-steam-library)
  - [Set the Game language to English](#set-the-game-language-to-english)
  - [Remove High Resolution Texture Pack DLC](#remove-high-resolution-texture-pack-dlc)
  - [Remove Creation Club Content](#remove-creation-club-content)
  - [Change Steams Update Behavior](#change-steams-update-behavior)
  - [Pre Modlist Installation Instructions](#pre-modlist-installation-instructions)
- [MODLIST INSTALLATION](#modlist-installation)
  - [Modlist Installation Instructions](#modlist-installation-instructions)
  - [Post Installation Instructions](#post-installation-instructions)
- [UPDATING](#updating)
- [FREQUENTLY ASKED QUESTIONS](#frequently-asked-questions)
  - [Why do I get a `Application Load Error 5:0000065434` error message when I try to launch the game?](#why-do-i-get-a-application-load-error-50000065434-error-message-when-i-try-to-launch-the-game)
  - [Why isn't XYZ mod in the list?](#why-isnt-xyz-mod-in-the-list)
  - [I have a bug / question!](#i-have-a-bug--question)
  - [I want to support your work!](#i-want-to-support-your-work)
- [CREDITS AND THANKS](#credits-and-thanks)

## REQUIREMENTS

* Latest version of [Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest).
* A clean **English** installation of Fallout 4, and all DLCs **EXCEPT** the High Resolution Texture Pack DLC.
  * Also known as Fallout 4: Game of the Year Edition.
  * **Acquired through [Steam](https://store.steampowered.com/app/377160/).**
* Around 36 GB of free space.
  * 34.3 GB for Fallout 4 itself.
  * 750 MB for the mod downloads.
  * 1.1 GB for the modlist installation.
* A [Nexusmods](https://www.nexusmods.com/) account.
  * Nexus Premium is not necessary, but is needed for automated downloads and will speed up the process.

## PREPARATION

These steps are only needed if you are installing this Modlist for the first time. If you are updating the Modlist, jump straight to [UPDATING](#updating).

### Installing Microsoft Visual C++ Redistributable Package

You likely already have this installed, but in case you haven't. This package is required for MO2 and you can download it from [Microsoft](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). Download the x64 version under "Visual Studio 2015, 2017 and 2019". [Direct link](https://aka.ms/vs/16/release/vc_redist.x64.exe) if you can't find it.

### Uninstalling the game

If you have the game installed under `C:\Program Files\`, `C:\Program Files (x86)\`, your Desktop, or your Documents folders, follow these steps to remove it.

1. Open **Steam** and go to your **Library**.
2. Find **Fallout 4** in the list.
3. Right-click on it and select **Manage** -> **Uninstall**.
4. Navigate to `Steam\steamapps\common\` and, if present, delete the **Fallout 4** folder.

### Making a new Steam Library

If you already have a Steam library set up outside of any default Windows folder, skip this step.

A new Steam library needs to be set up to install the game on, as the default library is in a default Windows UAC-protected folder (`C:\Program Files (x86)\Steam`).

1. Open **Steam** and select **Steam** -> **Settings** in the top left.
2. In the **Downloads** tab, select **Steam Library Folders**.
3. Select **Add Library Folder** and select a location outside of any default Windows folders.
   * For example, `C:\Games\Steam`.
4. Exit out of the settings when you are finished.

By default, Steam only allows one library per drive, but there is a workaround. If for example you already have the default Steam library at `C:\Program Files (x86)\Steam`, but still want your game on your `C:\` drive, you will need to follow [these instructions](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) to do so.

### Set the Game language to English

This entire Modlist is in English and 99% of all mods you will find are also in English. I highly recommend playing the game in English and support will not be given to people with a non-English game.

1. Open **Steam** and go to your **Library**.
2. Find **Fallout 4** in the list.
3. Right-click on it and select **Properties...**.
4. Click on **Language** and select **English** from the dropdown menu.

### Remove High Resolution Texture Pack DLC

1. Open **Steam** and go to your **Library**.
2. Find **Fallout 4** in the list.
3. Right-click on it and select **Properties...**.
4. Click on **DLC** and untick the checkbox next to **High Resolution Texture Pack**.

### Remove Creation Club Content

At the moment, Creation Club content / mods are not supported. This step is optional but support will not be given.

1. Navigate to your Fallout 4 installation folder and go into the **Data** folder.
2. Remove all files starting with "**cc**", such as "**cc**BGSFO4016-Prey - Main".

### Change Steams Update behavior

Occasionally, Fallout 4 recieves new updates on steam. This can break modded setups, and updating should be avoided until mods can be patched.

1. Open **Steam** and go to your **Library**.
2. Find **Fallout 4** in the list.
3. Right-click on it and select **Properties...**.
4. Under **Updates** select **Only update this game when I launch it**.

### Pre Modlist Installation Instructions

1. Navigate to **Documents\My Games\\** and if present, delete the **Fallout4** folder.
   * This will delete all saves you have, but the modlist requires you to start a new game anyway.
   * If you want to keep your saves, delete all files ending in ***.ini**.
2. Navigate to your Fallout 4 installation folder.
3. Run **Fallout4Launcher.exe**.
4. Click OK to both pop-ups that say **Detecting Video Hardware**.
5. Select **Options** then select the **High** preset option.
   * The high preset is used over the ultra preset because the ultra preset has options that can severely tank FPS without much visual improvement.
   * You can choose a lower preset if you have a lower-end PC, or want to squeeze as much performance out of the game as possible.
6. Set the **Resolution** option to your preference.
7. Click **OK** then **Exit**.

## MODLIST INSTALLATION

### Modlist Installation Instructions

1. Download the latest version of Wabbajack.
2. Create a new folder anywhere that is **NOT** under C:\Program Files, C:\Users or C:\Windows.
3. Place the downloaded Wabbajack.exe into this folder.
4. Download the latest [Wabbajack file](https://github.com/TDarkShadow/themidnightride-wabbajack/releases/latest) of this modlist.
5. Run **Wabbajack.exe**.
6. Select **Install From Disk**. Click on **···** next to **Target Modlist** to browse for the downloaded modlist.
7. In **Installation Location** select an empty folder that is **NOT** under C:\Program Files, C:\Users or C:\Windows.
   * Do **not** install this list in your **Steam**, **Fallout 4** folder or the folder with **Wabbajack.exe**.
8. The downloads location will auto-populate. This can be changed if preferred.
9.  Click the button with the Play Arrow to begin the process.
10. Accept the Nexusmods API request if asked.
11. Wabbajack will now automatically download and install every necessary mod.
    * If you don't have Nexus Premium, you'll have to manually click download for all the mods, but Wabbajack will still install them.
12. When Wabbajack completes you will see either a green **Installation Complete** screen or a red **Installation Failed** screen. If successful, proceed.

### Post Installation Instructions

1. Navigate to The Midnight Ride installation folder.
2. Open the folder named **Game Folder Files**.
3. Copy all files in this folder and paste it into your Fallout 4 installation folder.
   * **COPY _ONLY_ THE FILES IN THE "GAME FOLDER FILES" FOLDER.**
   * If asked, let it overwrite everything.

## UPDATING

When this Modlist receives an update, please check the Changelog before doing anything. Always backup your saves. Start a new game after updating, if noted in the Changelog.

**Wabbajack will delete all files that are not part of the Modlist when updating!** This means that any additional mods you have installed on top of the Modlist will be deleted. Your downloads folder will not be touched!

You can circumvent this behavior by renaming the mod with the prefix **[NoDelete]**. For example, you've added a mod named **[Sim Settlements 2](https://www.nexusmods.com/fallout4/mods/47976)**. In MO2, rename the mod name to **[NoDelete] Sim Settlements 2** so Wabbajack doesn't remove the mod when updating / reinstalling the modlist.

Updating is the same as installing. You only have to make sure that you select the same path and tick the **Overwrite Existing Modlist** checkbox in Wabbajack.

## FREQUENTLY ASKED QUESTIONS

### Why do I get a `Application Load Error 5:0000065434` error message when I try to launch the game?

Run your game directly through Steam once. You may also need to restart Steam and/or your PC.

### Why isn't XYZ mod in the list?

This modlist tries to be as customizable as possible while also fixing as many bugs as possible. That being said, check [Mods to Avoid](https://themidnightride.github.io/avoid-mods.html) to find out what mods you should avoid.

### I have a bug / question!

Ask it in the [Viva New Vegas Discord](https://discord.gg/DhX5S27). The support channel in the Wabbajack Discord is for installation questions, not support for in-game stuff, suggestions, or bug reports.

### I want to support your work!

I thank you for that thought but you should probably donate to Qolore first. You can find his Patreon [here](https://www.patreon.com/vivanewvegas) or his Paypal [here](https://www.paypal.com/paypalme/qolore7). If you want to support Wabbajack, go [here](https://www.patreon.com/user/overview?u=11907933).

## CREDITS AND THANKS

* _YOU_ for actually reading the readme!
* Qolore for creating such an amazing mod guide.
* ALL the mod authors that made the mods featured in this list.
* Halgari and everyone in the Wabbajack Team.
* Trawzified, Lively, and Kaethela for guiding me into this endavour.
* Drazden, the coolest moderator on Wabbajack

##### This readme is based off of [Starstruck Courier's readme](https://github.com/Kaethela/Starstruck-Courier/blob/main/README.md) and [Qwest's readme](https://github.com/SovnSkyrim/QWEST/blob/main/README.md). <!-- omit in toc -->
