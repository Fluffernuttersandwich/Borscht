# 🥣 Borscht Mod List -- Installation Guide

## 📌 Overview

Welcome to the **Borscht Mod List Installation Guide** for
**S.T.A.L.K.E.R. 2: Heart of Chornobyl**.

Borscht is a modular **Vanilla+ Wabbajack Mod List** using **Mod
Organizer 2 (MO2)**. It is designed to improve and expand the Zone while
keeping the experience recognizable as S.T.A.L.K.E.R. 2.


> [!CAUTION]
>
> **Borscht expects a clean, unmodded S.T.A.L.K.E.R. 2 installation.**
>
> Mods left behind by **Steam Workshop, Vortex, or manual installation**
> can load outside of Borscht's MO2 setup and cause conflicts that MO2
> cannot properly manage or troubleshoot.

------------------------------------------------------------------------

## ⚙️ System Requirements

If you can comfortably run vanilla **S.T.A.L.K.E.R. 2**, you should have
a reasonable starting point for Borscht.

Some optional mods may be more demanding than the vanilla game.

### Recommended

-   Windows 10 / 11
-   SSD strongly recommended
-   16 GB RAM minimum; more is recommended for S.T.A.L.K.E.R. 2
-   Enough free disk space for S.T.A.L.K.E.R. 2, Borscht, and Wabbajack
    download archives
-   A legal, supported copy of **S.T.A.L.K.E.R. 2: Heart of Chornobyl**

------------------------------------------------------------------------

# 🧹 BEFORE INSTALLING -- CLEAN YOUR GAME

This section is **mandatory**, especially if you have ever modded
S.T.A.L.K.E.R. 2 before.

Borscht cannot reliably manage mods that are being loaded outside of its
MO2 environment.

## 🔵 Step 1 -- Remove Steam Workshop Mods

If you have ever subscribed to S.T.A.L.K.E.R. 2 mods through Steam
Workshop:

1.  Open **Steam**.
2.  Go to **S.T.A.L.K.E.R. 2: Heart of Chornobyl → Workshop**.
3.  Open **Your Files / Subscribed Items**.
4.  Unsubscribe from **all S.T.A.L.K.E.R. 2 Workshop mods and
    collections**.
5.  Allow Steam to finish processing the changes.

Steam Workshop files for S.T.A.L.K.E.R. 2 are normally stored beneath:

``` text
<Steam Library>\steamapps\workshop\content\1643320\
```

After unsubscribing, inspect that location for leftover Workshop
content.


> [!WARNING]An empty `~mods` folder does **not** by itself prove that
> your game is unmodded. Steam Workshop content is stored separately.

Do not subscribe to Steam Workshop mods while using the official Borscht
configuration unless Borscht specifically instructs you to do so.


<img width="1652" height="570" alt="image" src="https://github.com/user-attachments/assets/bf5d9c36-7174-4d32-a3c4-65aaa1a23eee" />


------------------------------------------------------------------------

## 🟠 Step 2 -- Remove Vortex Mods

If you have **ever used Vortex** to mod S.T.A.L.K.E.R. 2:

1.  Open **Vortex**.
2.  Select **S.T.A.L.K.E.R. 2: Heart of Chornobyl**.
3.  Disable **all** S.T.A.L.K.E.R. 2 mods.
4.  Use **Purge Mods**.
5.  Apply/Deploy the disabled state if Vortex prompts you to deploy
    changes.
6.  Confirm that Vortex is no longer deploying S.T.A.L.K.E.R. 2 mods.
7.  Close Vortex.


> [!CAUTION]
> Do not use Vortex to manage S.T.A.L.K.E.R. 2 while using Borscht.
>
> Files deployed by Vortex exist outside Borscht's MO2 management and
> can create conflicts that are difficult to identify.

<img width="2652" height="1118" alt="image" src="https://github.com/user-attachments/assets/1446e6d3-4d3e-4f4d-bf1c-3c7613226d26" />


------------------------------------------------------------------------

## 🟡 Step 3 -- Empty the Vanilla `~mods` Folder

Manually open your S.T.A.L.K.E.R. 2 installation directory.

For a typical Steam installation:

``` text
...\SteamLibrary\steamapps\common\S.T.A.L.K.E.R. 2 Heart of Chornobyl\
```

Navigate to:

``` text
Stalker2\Content\Paks\~mods\
```

The vanilla game's `~mods` folder should contain **no manually installed
mods** before using Borscht.

Look for files such as:

``` text
*.pak
*.ucas
*.utoc
```

and any mod folders/packages you previously installed manually.


> [!CAUTION]
>
> Do **not** simply assume this folder is clean because
> Vortex says your mods are disabled.
>
> **Open the folder and check it yourself.**


Borscht will manage its own mod files through MO2. Do not manually copy
Borscht's PAK files into the vanilla `~mods` directory.


<img width="2432" height="586" alt="image" src="https://github.com/user-attachments/assets/60f9d9ac-0a34-4119-bd5e-bc862f6ee826" />


------------------------------------------------------------------------

## 🟢 Step 4 -- Verify the Vanilla Game

After removing Steam Workshop, Vortex, and manually installed mods:

1.  Open **Steam**.
2.  Right-click **S.T.A.L.K.E.R. 2: Heart of Chornobyl**.
3.  Select **Properties**.
4.  Select **Installed Files**.
5.  Select **Verify integrity of game files**.
6.  Allow Steam to complete the verification.
7.  Launch S.T.A.L.K.E.R. 2 **directly from Steam once**.
8.  Reach the main menu.
9.  Exit the game.

If the vanilla game does not launch correctly, **stop here and fix the
vanilla installation before installing Borscht**.

This gives us a known-good baseline for troubleshooting.


<img width="3762" height="1334" alt="image" src="https://github.com/user-attachments/assets/a71df74c-0663-4026-8e14-58256475b74c" />


------------------------------------------------------------------------

# 🌐 Step 5 -- Nexus Mods Account

Create or sign into your Nexus Mods account:

https://users.nexusmods.com/register

### 💎 Nexus Mods Premium

-   Automatic downloads through Wabbajack
-   Faster installation
-   Strongly recommended for large mod lists

### 🆓 Free Nexus Mods Account

-   Wabbajack can still be used
-   Nexus downloads require manual confirmation
-   Installation will take considerably longer

------------------------------------------------------------------------

# 📦 Step 6 -- Install Wabbajack

Download Wabbajack from:

https://www.wabbajack.org/

Open Wabbajack and sign into **Nexus Mods** when prompted.

> [!TIP]
> Keep Wabbajack and your mod list outside Windows-protected folders.

Avoid installing Borscht into locations such as:

``` text
C:\Program Files\
C:\Program Files (x86)\
C:\Users\<You>\Documents\
C:\Users\<You>\Desktop\
C:\Users\<You>\OneDrive\
```

Do **not** use your S.T.A.L.K.E.R. 2 game directory as the Borscht
installation location.

------------------------------------------------------------------------

# 📁 Step 7 -- Create the Borscht Installation Folder

A simple folder near the root of an SSD is recommended.

Example:

``` text
D:\Wabbajack_ModLists\Borscht
```

Your Borscht installation and vanilla S.T.A.L.K.E.R. 2 installation are
**separate locations**.

------------------------------------------------------------------------

# ⬇️ Step 8 -- Install Borscht

### If Borscht is available in the Wabbajack Gallery

1.  Open **Wabbajack**.
2.  Browse Modlists.
3.  Make sure the Include -> Non-featured is checked.
4.  Use the Dropdown Arrow to select **Stalker 2**
5.  Locate **Borscht**.
6.  Select **Download & Install**.

Recommended:

``` text
D:\Wabbajack_ModLists\Borscht
```

Wabbajack will automatically populate a **Download Location** for the original mod
archives.

Example:

``` text
D:\Wabbajack_ModLists\Borscht\downloads
```

> [!WARNING]
>
> The **Installation Location must not be your
> S.T.A.L.K.E.R. 2 game directory** and must not be the same folder as
> another Wabbajack list.

Click **Install** and allow Wabbajack to complete.

------------------------------------------------------------------------

## ⏳ Download Expectations

### 💎 Premium

-   Downloads are largely automated
-   Installation speed depends on your connection, storage, and hardware

### 🆓 Free

-   Nexus downloads require manual interaction
-   Expect considerably more clicking and installation time

------------------------------------------------------------------------

# 🛠️ Wabbajack Download Troubleshooting

## 🔴 A Mod Failed to Download

First:

1.  Wait a few minutes.
2.  Run the Borscht installation again using the **same installation and
    download paths**.

Wabbajack can reuse files that were already downloaded successfully.

If a required archive has been removed or replaced by a mod author,
Borscht itself may need an update before Wabbajack can complete the
installation.

## ❌ Game File Source Missing

A missing game-file/source error can indicate that the installed game
version does not match the version expected by the current Borscht
release.

Confirm:

-   Steam has finished updating S.T.A.L.K.E.R. 2
-   You own a legitimate copy of the game
-   The Borscht release supports your currently installed game version
-   Steam verification completed successfully

------------------------------------------------------------------------

# ✅ Installation Complete

When Wabbajack reports that installation completed successfully, close
Wabbajack.

Navigate to your Borscht installation and run:

``` text
ModOrganizer.exe
```

------------------------------------------------------------------------

# ▶️ Step 9 -- Launch Borscht Through MO2

On first launch, MO2 may ask about Nexus/NXM integration. Accept the
association when appropriate.

In MO2:

1.  Confirm the **Borscht** profile is selected.
2.  Confirm **S.T.A.L.K.E.R. 2: Heart of Chornobyl** is selected in the
    executable dropdown.
3.  Click **Run**.

> [!IMPORTANT]
>
> ALWAYS launch Borscht through Mod Organizer 2.
>
> Steam may be running in the background,
> but **MO2 should initiate the Borscht game launch**.
>
> Do _not_ launch the game from a normal Steam shortcut, desktop
> S.T.A.L.K.E.R. 2 shortcut, or the game's executable when you intend to
> play Borscht.

💡 You may want to pin Borscht's `ModOrganizer.exe` to your taskbar or
create a convenient shortcut.

------------------------------------------------------------------------

# 🎮 MO2 Profiles

Borscht is designed to be modular, and MO2 profiles make experimentation
much safer.

### **Borscht**

This is the official configuration shipped with the list. Keep this
profile available as your clean reference configuration.

## 🛠️ Create a Personal Profile

In MO2:

``` text
Profile Dropdown → Manage
```

Copy the supplied **Borscht** profile and rename it.

Examples:

``` text
Borscht
Borscht - Personal
Borscht - Testing
```

This gives you a sandbox for enabling, disabling, or experimenting with
mods while preserving the official Borscht configuration.

------------------------------------------------------------------------

# ⚙️ Understanding the Borscht Mod List

Borscht is intended to be more modular than a traditional locked-down
overhaul.

Pay attention to:

-   MO2 separators/categories
-   Mod names
-   The **Notes** column
-   Compatibility warning Pop-Ups
-   Required dependencies
-   Optional variants
-   Mods marked as unsafe to change during an existing playthrough

Cursor-hover over MO2 Notes when additional information is available.

> [!TIP]
> Read highlighted warnings before enabling or disabling unfamiliar mods.

------------------------------------------------------------------------

# 🧪 Customizing Borscht

You are welcome to customize the list.

However, some mods:

-   Require other mods
-   Conflict with alternatives
-   Replace the same S.T.A.L.K.E.R. 2 assets
-   Are intended as mutually exclusive variants
-   May not be safe to add/remove from an existing save

### Best Practices

-   Never enable/disable mods while the game is running
-   Prefer making major mod changes before starting a serious
    playthrough
-   Use a test save when experimenting
-   Keep the official **Borscht** profile intact
-   Use **Borscht - Personal** or another copied profile for
    customization

------------------------------------------------------------------------

# ➕ Adding Your Own Mods

Advanced users may add additional mods through MO2.

> [!WARNING]
> Support is provided against the _official_ Borscht Profile configuration only!
>
> You are welcome to customize Borscht, but if you encounter a problem
> you may be asked to reproduce it using the unmodified/default Borscht
> profile before troubleshooting can continue.

Do **not** manually install your additional mods into the vanilla game's
`~mods` folder.

Keep them inside Borscht/MO2 so that their presence is visible and
manageable.

### ⚠️ Do Not Blindly Update Individual Mods

MO2 or Nexus may report that a newer version of an included mod exists.

That does **not** automatically mean you should update it.

A newer release may:

-   Require a newer game version
-   Change its file/package structure
-   Add or remove dependencies
-   Conflict with another Borscht mod
-   Require changes elsewhere in the list

Unless you know what you are doing, use the version supplied by the
current Borscht release and allow the **Borscht list update** to handle
tested mod updates.

------------------------------------------------------------------------

# 🔄 Updating Borscht

Before updating:

1.  Read the Borscht changelog.
2.  Pay attention to warnings about save compatibility.
3.  Close MO2 and S.T.A.L.K.E.R. 2.
4.  Open Wabbajack.
5.  Install the new Borscht release using the **same Borscht
    installation location**.
6.  Allow Wabbajack to update the list.

Wabbajack can reuse archives already present in the download folder, so
an update generally does not require downloading the entire list again.

> [!CAUTION]
>
> Wabbajack updates can remove or replace files that are
> not part of the official list.
>
> Keep personal modifications organized and preserve anything important
> before updating.

------------------------------------------------------------------------

# 🧯 Troubleshooting

See:

➡️ **[TROUBLESHOOTING.md](TROUBLESHOOTING.md)**

When asking for help, first test against the official/default Borscht
profile whenever possible.

## Before Asking for Support

Confirm all of the following:

-   [ ] I am using a supported version of S.T.A.L.K.E.R. 2.
-   [ ] I unsubscribed from S.T.A.L.K.E.R. 2 Steam Workshop mods.
-   [ ] Vortex is not deploying S.T.A.L.K.E.R. 2 mods.
-   [ ] The vanilla game's `Stalker2\Content\Paks\~mods\` folder
    contains no manually installed mods.
-   [ ] I verified the game through Steam.
-   [ ] Vanilla S.T.A.L.K.E.R. 2 launches successfully.
-   [ ] Borscht is installed outside Windows-protected folders.
-   [ ] Borscht is **not** installed inside the S.T.A.L.K.E.R. 2 game
    directory.
-   [ ] I launch Borscht through its _included_ Mod Organizer 2.
-   [ ] I tested the issue using the official/default Borscht profile.

------------------------------------------------------------------------

# 🗑️ Uninstalling Borscht

Because Borscht is managed separately from the vanilla game, removing
the list should generally be straightforward.

1.  Close S.T.A.L.K.E.R. 2.
2.  Close Mod Organizer 2.
3.  Delete the Borscht installation folder.

If your download archives are stored elsewhere, delete those separately
only if you no longer want them.

Your vanilla S.T.A.L.K.E.R. 2 installation should remain separate.

If you manually changed the vanilla game directory outside of Borscht,
those changes are **not** automatically removed by deleting Borscht.

------------------------------------------------------------------------

# 🧠 Final Notes

Borscht is built around a simple idea:

> **Keep the vanilla game clean. Let MO2 manage the mods in its virtual file system.**

For the smoothest experience:

-   Keep Steam Workshop mods unsubscribed
-   Keep Vortex away from the Borscht setup
-   Keep manually installed mods out of the vanilla `~mods` folder
-   Launch through Borscht's MO2
-   Use copied MO2 profiles when experimenting
-   Read mod Notes before changing unfamiliar options
-   Let Borscht updates handle tested mod-version changes

Welcome to the Zone.

🥣 **Enjoy your Borscht.**
