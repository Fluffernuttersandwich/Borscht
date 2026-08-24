# 🍲 Borscht Troubleshooting

This guide covers basic troubleshooting and support for **Borscht**, a
Wabbajack Mod List for **S.T.A.L.K.E.R. 2: Heart of Chornobyl**.

## 💬 Getting Support

Borscht support is provided through the **Smörgåsbord Discord Server**
under the **Borscht** category and its related support channels.

**Discord:** https://discord.gg/Ay2pVZHE7S

Before requesting help, please work through the basic troubleshooting
steps below and collect the appropriate logs. Providing useful
information and logs makes it much easier to identify the problem.

------------------------------------------------------------------------

## ✅ Before You Ask for Help

Please check the following first:

-   🎮 Make sure **S.T.A.L.K.E.R. 2** is fully updated through Steam.
-   🍲 Make sure you are using the current version/revision of
    **Borscht**.
-   🚀 Launch the game through **Mod Organizer 2 (MO2)** using the
    Borscht installation.
-   🔄 Restart MO2 and the game and try again.
-   📝 If the problem is repeatable, note exactly what you were doing
    when it occurred.
-   🧩 If you added, removed, updated, or changed any mods, mention this
    when requesting support.

### 🛠️ Modified Borscht Installations

Borscht is designed to be customized, but troubleshooting a modified
installation is naturally more difficult.

If you have:

-   ➕ Added mods
-   ➖ Removed mods
-   ⬆️ Updated individual mods yourself
-   🔀 Changed the load order
-   ⚙️ Changed mod configuration files
-   📁 Manually installed files into the STALKER 2 game directory

...please tell us when requesting support.

When possible, determine whether the problem also occurs with the
**default Borscht configuration**.

------------------------------------------------------------------------

## 📜 Finding Your STALKER 2 Logs

STALKER 2 stores its logs under your Windows user profile.

### 📄 Normal Game Logs

Press **Win + R**, paste the following path, and press **Enter**:

``` text
%LOCALAPPDATA%\Stalker2\Saved\Logs
```

The full path normally looks like:

``` text
C:\Users\Username\AppData\Local\Stalker2\Saved\Logs
```

For most problems, the file we are interested in is:

``` text
Stalker2.log
```

If you are requesting support for a problem that did **not** crash the
game, please provide the most recent `Stalker2.log`.

------------------------------------------------------------------------

## 💥 Finding Crash Reports

If STALKER 2 crashes, additional diagnostic information is normally
created here.

Press **Win + R**, paste:

``` text
%LOCALAPPDATA%\Stalker2\Saved\Crashes
```

and press **Enter**.

The full path normally looks like:

``` text
C:\Users\Username\AppData\Local\Stalker2\Saved\Crashes
```

You may see files such as:

``` text
CrashContext.runtime-xml
CrashReportClient.ini
Stalker2.log
UE*.dmp
```

### 📦 If the Game Crashed

Find the **newest crash folder**, ZIP the entire folder, and upload the
ZIP when requesting support.

This is preferable to selecting individual crash files because the
complete crash folder provides more diagnostic information.

------------------------------------------------------------------------

## 🚫 Game Crashes on Startup

If Borscht crashes before reaching the main menu:

1.  🔄 Restart your computer.
2.  🍲 Start Borscht's Mod Organizer 2.
3.  👤 Make sure you are using the intended Borscht profile.
4.  🚀 Launch STALKER 2 through MO2.
5.  💥 Reproduce the crash once.
6.  📁 Collect the newest crash report from:

``` text
%LOCALAPPDATA%\Stalker2\Saved\Crashes
```

7.  📦 ZIP the newest crash folder and provide it when requesting
    support.

If you have changed the Borscht mod configuration, also test with the
**default Borscht configuration** if possible.

------------------------------------------------------------------------

## 💥 Crashes During Gameplay

For crashes that occur after successfully entering the game, please note
what was happening immediately before the crash.

Useful information includes:

-   📍 Location
-   🎮 What you were doing
-   🔫 Weapon/item being used
-   👤 NPC or mutant involved
-   🎒 Opening an inventory/container
-   🚪 Entering or leaving an area
-   💾 Loading a save
-   🔁 Whether the same action causes the crash again

A crash that occurs **repeatedly under the same circumstances** is
particularly useful for troubleshooting.

Please provide the newest crash folder from:

``` text
%LOCALAPPDATA%\Stalker2\Saved\Crashes
```

------------------------------------------------------------------------

## 🧪 Test Whether the Problem Happens Without Borscht

One of the most useful troubleshooting questions is:

**Does the same problem happen when running unmodded STALKER 2?**

If the problem also occurs completely unmodded, it may be a STALKER 2,
driver, hardware, Steam, or game-installation problem rather than a
Borscht problem.

If the problem occurs **only with Borscht**, we can begin investigating
the mod list.

⚠️ **Do not delete your Borscht installation just to perform this
test.**

------------------------------------------------------------------------

## 🖼️ Missing Textures, Icons, Models, or Other Visual Problems

If something appears visually broken:

-   📸 Take a screenshot.
-   📍 Note where the problem occurs.
-   🔁 Note whether it happens consistently.
-   🍲 Test whether the problem occurs using the default Borscht
    configuration.
-   🧪 If practical, check whether the same problem occurs in unmodded
    STALKER 2.

Please include the screenshot and your latest:

``` text
Stalker2.log
```

A visual problem that continues to occur without Borscht may indicate a
problem with the base game rather than the mod list.

------------------------------------------------------------------------

## 🧩 A Mod Does Not Appear to Be Working

Check the following:

-   🚀 Are you launching STALKER 2 through Borscht's MO2?
-   ☑️ Is the mod enabled in MO2?
-   🔗 Are its required mods also enabled?
-   🔀 Did you change the load order?
-   ⬆️ Did you manually update the mod?
-   📁 Did you install another version of the same mod manually?
-   🍲 Does the problem occur with the default Borscht configuration?

If you customized your mod selection, include those changes when
requesting support.

------------------------------------------------------------------------

## 📉 Performance Problems

STALKER 2 can be demanding even without mods. If reporting a significant
performance problem, please include:

-   🧠 CPU
-   🎨 GPU
-   💾 Amount of RAM
-   🖥️ Screen resolution
-   ⚙️ Graphics preset
-   🖼️ DLSS / FSR / XeSS setting
-   🎞️ Frame Generation enabled or disabled
-   📊 Approximate FPS
-   📍 Location where the problem occurs
-   🧪 Whether the same performance problem occurs without Borscht

If possible, compare vanilla STALKER 2 and Borscht in approximately the
**same location and conditions**.

------------------------------------------------------------------------

## 🔧 Steam Verify Files

Steam's **Verify integrity of game files** feature can repair damaged or
missing base-game files.

⚠️ However, do **not** use Steam verification as a universal first
troubleshooting step unless instructed to do so.

Borscht or other modding tools may intentionally interact with files
associated with the game installation. Verification can therefore
complicate troubleshooting in some situations.

If support asks you to verify the game, follow the provided instructions
and then retest the problem.

------------------------------------------------------------------------

## ⛔ Things You Should NOT Do

Please avoid drastic troubleshooting steps before asking for help.

Do **not**:

-   🗑️ Delete your entire Borscht installation before collecting logs.
-   🗑️ Randomly delete files from the STALKER 2 directory.
-   ⬆️ Manually update individual Borscht mods unless you understand the
    consequences.
-   📦 Install another copy of a Borscht mod manually over the existing
    version.
-   🔀 Use Vortex to manage the same Borscht installation.
-   🌐 Download random DLL files or "fixes" from videos or unknown
    websites.
-   🧹 Use registry cleaners or similar "PC repair" utilities.
-   💻 Reinstall Windows because a modded game crashed.

Many problems can be diagnosed from the logs. **Collect the evidence
before deleting it.**

------------------------------------------------------------------------

## 🆘 What to Include When Requesting Support

When posting in the **Borscht support channels** on the Smörgåsbord
Discord, please include:

-   🍲 **Borscht version/revision**
-   📝 **Description of the problem**
-   🎮 **What you were doing when it happened**
-   🔁 **Whether the problem is repeatable**
-   ⚙️ **Whether you are using the default Borscht configuration**
-   🧩 **Any mods you added, removed, updated, or changed**
-   📄 **`Stalker2.log` for normal problems**
-   📦 **Newest zipped crash folder for crashes**
-   📸 **Screenshot or video if the problem is visual**

For crashes, please upload the **ZIP of the newest crash folder** rather
than screenshots of the crash reporter.

------------------------------------------------------------------------

## 💬 Borscht Support

Support is provided through the **Smörgåsbord Discord Server**.

Join the server and look for the **Borscht** category and its related
channels:

**https://discord.gg/Ay2pVZHE7S**

📜 Please provide logs whenever possible. A useful log is usually much
more helpful than a screenshot of an error message.
