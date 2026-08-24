# 🥣 Borscht – Saving Profiles, Sharing Setups, and Adding Your Own Mods

Borscht is designed to be highly modular. Mod Organizer 2 (MO2) makes it easy to:

- Enable or disable optional Borscht mods
- Save your personal setup in a separate Profile
- Preserve your enabled/disabled choices across Borscht updates
- Share your exact toggled setup with another Borscht user
- Add your own compatible S.T.A.L.K.E.R. 2 mods without touching the vanilla game directory

This guide covers all of that in one place.

---

# Part 1 – Save Your Enabled & Disabled Mods for Future Borscht Updates

When updating Borscht, the official/default MO2 Profile may be replaced or refreshed by the list.

If you have:

- Enabled optional mods
- Disabled mods you do not want
- Changed variants
- Customized your personal Borscht setup

...create your own copied Profile before updating.

This only takes about a minute and can save you from having to redo your mod toggles after future updates.

---

## Why This Matters

MO2 stores your enabled and disabled mod selections inside your Profile.

Borscht's official Profile is intended to remain the known-good configuration used for testing and troubleshooting.

Your personal configuration should live in a separate Profile.

For example:

```text
Borscht
[NoDelete] My Borscht
```

The original **Borscht** Profile remains available as your clean reference.

Your `[NoDelete]` Profile becomes your personal configuration.


You must also put `[NoDelete]` in front of every mod you add from outside of the list. 

This is the only way off-list mods you add will remain after you update the list through Wabbajack!

---

## Step 1 – Open the Profile Menu in MO2

At the top-left of MO2, locate the **Profile dropdown menu**.

Open it and select:

**Manage...**

---

## Step 2 – Copy the Borscht Profile

Inside the Profile Manager:

1. Select the **Borscht** Profile.
2. Click **Copy**.
3. Give the new Profile a recognizable name.

Example:

```text
[NoDelete] My Borscht
```

or:

```text
[NoDelete] CoolGuy84
```

---

## Step 3 – Keep `[NoDelete]` at the Beginning

Place:

```text
[NoDelete]
```

at the beginning of your custom Profile name.

Example:

```text
[NoDelete] My Borscht
```

This makes your personal Profile clearly identifiable and helps distinguish it from Profiles supplied by the official list.

> [!IMPORTANT]
> Do **not** overwrite the official `Borscht` Profile.
>
> Keep it available as a clean troubleshooting reference.

---

## Result

You now have:

```text
Borscht
[NoDelete] My Borscht
```

Use:

- **Borscht** when testing the official list
- **[NoDelete] My Borscht** for your personal mod configuration

---

# After Future Borscht Updates

If new mods are added to Borscht in a future revision, they may appear at the **bottom of the MO2 left pane** when using an older custom Profile.

This is normal.

After updating:

1. Select your `[NoDelete]` Profile.
2. Scroll to the bottom of the MO2 left pane.
3. Look for newly added Borscht mods.
4. Drag them into the appropriate Separator/category if needed.
5. Enable or disable them according to your preference.
6. Read their MO2 Notes before changing unfamiliar options.

> [!TIP]
> Before making changes after a major Borscht update, briefly select the official **Borscht** Profile first. This lets you see how the new revision is intended to be configured.

---

# Part 2 – Share & Import Borscht MO2 Profiles

Want to share your exact **enabled/disabled Borscht setup** with another user?

This can be useful for:

- Friends who want the same setup
- Streamers sharing their configuration
- Players comparing different Borscht builds
- Multiplayer groups if the relevant mods require matching setups
- Troubleshooting a known configuration

---

## ⚠️ Before Sharing a Profile

Both users should be running the **same Borscht revision**.

For example:

```text
Exporter: Borscht 1.2.4
Importer: Borscht 1.2.4
```

This process does **not** install or download mods.

It only tells MO2 which already-installed mods should be enabled or disabled.

---

## 📤 EXPORTER – Sharing Your Profile

1. Select the MO2 Profile you want to share.
2. Confirm your desired mods are enabled and disabled.
3. Open the Borscht installation folder.
4. Open:

```text
profiles\Your Profile Name\
```

5. Locate:

```text
modlist.txt
```

6. Copy `modlist.txt`.
7. Send that file to the other Borscht user.

That's it.

---

## 📥 IMPORTER – Using a Shared Profile

1. Confirm you are using the **same Borscht revision** as the Exporter.
2. Open MO2.
3. Create a **new Profile**.
4. Give it a recognizable name.
5. Close MO2.
6. Open the Borscht installation folder.
7. Navigate to:

```text
profiles\Your New Profile Name\
```

8. Replace the existing:

```text
modlist.txt
```

with the shared file.
9. Start MO2 again.
10. Select the new Profile.

MO2 should now display the same enabled/disabled mod configuration as the Exporter's Profile.

> [!IMPORTANT]
> Never replace the `modlist.txt` inside the official **Borscht** Profile.
>
> Always import another user's setup into a **new Profile**.

---

# Part 3 – Adding Your Own Mods to Borscht

Advanced users are welcome to add their own compatible S.T.A.L.K.E.R. 2 mods.

However:

> [!WARNING]
> **Support is provided against the official Borscht configuration.**
>
> If you encounter a problem after adding your own mods, you may be asked to reproduce the issue using the official/default **Borscht** Profile before troubleshooting continues.

---

## Rule #1 – Keep the Vanilla Game Clean

Do **not** manually install your personal mods into:

```text
Stalker2\Content\Paks\~mods\
```

Do **not** use Vortex or Steam Workshop to add extra mods alongside Borscht unless specifically instructed.

Keep your personal additions inside the **Borscht MO2 installation** so MO2 can see and manage them.

---

## Step 1 – Use Your Personal Profile

Before adding mods, select or create a personal Profile such as:

```text
[NoDelete] My Borscht
```

Do not use the official **Borscht** Profile as your experimental sandbox.

---

## Step 2 – Download the Mod

You can either:

### Option A – Download Through MO2 / Nexus

If Nexus integration is configured:

1. Open the mod's Nexus Mods page.
2. Select **Mod Manager Download** when supported.
3. Allow the download to open in Borscht's MO2.
4. Install the archive from the **Downloads** tab.

### Option B – Manual Download

1. Download the mod archive manually from Nexus Mods.
2. Open Borscht's MO2.
3. Drag the downloaded archive into the **Downloads** pane.

Or place the archive into:

```text
Borscht\downloads\
```

Then install it through MO2.

---

# Step 3 – Check the Mod's Folder Structure

S.T.A.L.K.E.R. 2 mods are not all packaged consistently.

Some archives will install correctly immediately.

Others may show in *italics* or display an invalid-content warning because the archive contains extra wrapper folders.

Do **not** blindly move files around until you understand what type of mod you are looking at.

---

## Common Type A – Standard PAK / IoStore Mod

If the archive ultimately contains ordinary files such as:

```text
ExampleMod.pak
ExampleMod.ucas
ExampleMod.utoc
```

the typical Borscht/MO2 structure is:

```text
Your Mod Name\
└── Content\
    └── Paks\
        └── ~mods\
            ├── ExampleMod.pak
            ├── ExampleMod.ucas
            └── ExampleMod.utoc
```

If the mod only has a `.pak`, that is fine:

```text
Your Mod Name\
└── Content\
    └── Paks\
        └── ~mods\
            └── ExampleMod.pak
```

> [!IMPORTANT]
> Keep matching `.pak`, `.ucas`, and `.utoc` files together.

---

## Common Type B – Archive Wrapper Folder

A mod may arrive like this:

```text
Your Mod Name\
└── RandomAuthorFolder\
    ├── ExampleMod.pak
    ├── ExampleMod.ucas
    └── ExampleMod.utoc
```

If `RandomAuthorFolder` is only an organizational wrapper, normalize it to:

```text
Your Mod Name\
└── Content\
    └── Paks\
        └── ~mods\
            ├── ExampleMod.pak
            ├── ExampleMod.ucas
            └── ExampleMod.utoc
```

Then remove the empty wrapper folder.

This is similar to fixing a badly packaged mod in other MO2-supported games: the goal is to make the installed MO2 mod mirror the path expected by the game.

---

## Common Type C – Multiple Optional Components

A download may contain folders such as:

```text
Better Stamina\
Better Vaulting\
Fall Damage Protection\
```

If those folders only contain independent `.pak` / `.ucas` / `.utoc` files, you have two reasonable choices:

### Keep Them Together

Place all intended components under:

```text
Content\Paks\~mods\
```

### Split Them Into Separate MO2 Mods

This is often better if each feature can be toggled independently:

```text
Better Stamina
Better Vaulting
Fall Damage Protection
```

Each can still come from the same original Nexus download archive.

This gives you cleaner control in MO2.

---

## Common Type D – ZoneKit / DLC-Style Package

Some newer S.T.A.L.K.E.R. 2 mods have structures such as:

```text
PackageName\
└── Windows\
    ├── NewContent\
    │   └── Windows\
    │       └── Stalker2\
    └── OverrideContent\
        └── Windows\
            └── Stalker2\
```

You may also see:

```text
Manifest_UFSFiles_Win64.txt
```

Do **not** automatically extract the nested `.pak/.ucas/.utoc` files from these packages.

For mods documented to use this packaging style, preserve the package structure and place the complete package beneath:

```text
Content\Paks\~mods\
```

Example:

```text
Your Mod Name\
└── Content\
    └── Paks\
        └── ~mods\
            └── PackageName\
                └── Windows\
                    ├── NewContent\
                    └── OverrideContent\
```

> [!CAUTION]
> If you are unsure whether a mod is a normal PAK mod or a ZoneKit/DLC-style package, **stop and check the mod author's installation instructions before restructuring it**.

---

## Common Type E – LogicMods or Other Special Mod Types

If a mod specifically instructs you to use:

```text
Content\Paks\LogicMods\
```

or another special path, do not convert it into a normal `~mods` mod just because most Borscht mods use `~mods`.

Follow the mod's intended structure.

The same applies to framework or loader mods that belong under locations such as `Binaries`, `Plugins`, or another special game path.

---

# Step 4 – Refresh MO2

After correcting a mod's structure:

1. Return to MO2.
2. Refresh the mod list if needed.
3. Confirm the mod no longer appears invalid.
4. Enable it in your personal Profile.

For normal PAK mods, check the **PAK Files** tab if appropriate and confirm the mod appears there.

---

# Step 5 – Pay Attention to Load Order

S.T.A.L.K.E.R. 2 PAK conflicts are not always obvious from MO2's normal left-pane conflict indicators.

Borscht uses the **PAK Files** tab to manage relevant PAK priority.

If a mod author says:

> Load this after X

or:

> This compatibility patch must overwrite Y

make sure the PAK order reflects that requirement.

Do not assume that MO2 left-pane position alone determines every S.T.A.L.K.E.R. 2 conflict.

---

# Step 6 – Protect Personal Mods During Updates

Give personal mods a clear naming convention.

Recommended:

```text
[NoDelete] Your Mod Name
```

Examples:

```text
[NoDelete] My Flashlight Tweaks
[NoDelete] Extra Weapon Pack
[NoDelete] Personal Weather Mod
```

This makes it immediately obvious which mods are yours and which belong to the official Borscht list.

Keep them inside an appropriate custom separator if desired:

```text
──────── YOUR PERSONAL MODS ────────
[NoDelete] My Flashlight Tweaks
[NoDelete] Extra Weapon Pack
```

> [!IMPORTANT]
> A naming convention does not magically make every file immune to every possible Wabbajack update behavior.
>
> Keep backups of anything you created or manually modified and review your personal additions after major Borscht updates.

---

# Step 7 – Test Before Starting a Serious Playthrough

After adding a new mod:

1. Launch Borscht through MO2.
2. Use a test save when possible.
3. Confirm the game reaches the main menu.
4. Load into the Zone.
5. Test the feature you added.
6. Check for obvious missing assets, crashes, or unexpected behavior.

Avoid adding a large batch of unknown mods all at once.

Adding one or a few at a time makes troubleshooting much easier.

---

# ⚠️ Updating Your Personal Mods

Do not automatically install every Nexus update MO2 reports.

A new mod release may:

- Target a different S.T.A.L.K.E.R. 2 version
- Change from standard PAK packaging to ZoneKit packaging
- Rename its files
- Add dependencies
- Remove dependencies
- Change load-order requirements
- Become incompatible with Borscht

Read the mod's changelog and installation instructions first.

For mods already included in Borscht, it is generally safer to wait for the **Borscht update** to provide the tested version.

---

# Quick Reference

## Save Your Personal Borscht Profile

```text
Profile Dropdown
→ Manage
→ Copy Borscht
→ Rename to [NoDelete] My Borscht
```

## Share Your Enabled/Disabled Setup

```text
Borscht\profiles\Your Profile\modlist.txt
```

Share that file with another user running the **same Borscht revision**.

## Add a Typical PAK Mod

```text
Your Mod\
└── Content\
    └── Paks\
        └── ~mods\
            ├── Mod.pak
            ├── Mod.ucas
            └── Mod.utoc
```

## Keep Personal Mods Easy to Identify

```text
[NoDelete] Your Mod Name
```

---

# 🥣 Final Recommendation

The safest way to customize Borscht is:

1. Keep the official **Borscht** Profile untouched.
2. Create **[NoDelete] My Borscht**.
3. Add personal mods only through MO2.
4. Keep the vanilla game directory clean.
5. Change only a few things at a time.
6. Test your changes.
7. If something breaks, switch back to the official **Borscht** Profile and compare.

Borscht provides the ingredients.

**What you add to the bowl is up to you.**
