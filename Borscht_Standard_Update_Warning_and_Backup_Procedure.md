# Borscht --- Standard Update Warning & Backup Procedure

> [!WARNING] **There is no guarantee that updating Borscht will be
> safe for an existing save.**
>
> Borscht updates can add, remove, or change mods, frameworks, scripts,
> and gameplay systems. STALKER 2 itself may also receive updates that
> affect existing saves. If your current playthrough is working well,
> **you do not need to update simply because a new Borscht revision is
> available.**

If you want to update Borscht **and continue your current playthrough**,
we strongly recommend doing **both** of the following first.

## 1. Preserve Your Current MO2 Profile

In MO2, select the **Borscht** profile, then go to:

**Profile Dropdown → Manage → Copy**

Rename the copy to something you'll recognize and **include `[NoDelete]`
in the profile name**, for example:

`[NoDelete]CoolGuy87BowlOfBorscht`

The `[NoDelete]` tag protects that profile from being removed during a
future Wabbajack update. This gives you a preserved copy of your
previous mod configuration that you can return to if the new revision
causes problems with your existing playthrough.

## 2. Back Up Your STALKER 2 Save Files

Before updating, make a copy of your current STALKER 2 save folder and
store it somewhere safe outside the game's normal save location.

This is important because simply switching back to an older MO2 profile
**does not roll back your save**. If you load and save your game after
updating Borscht, the save itself may be changed by the new mod
configuration.

Having a separate backup lets you restore both sides of the equation:

-   **Your previous Borscht mod configuration** using the preserved
    `[NoDelete]` MO2 profile.
-   **Your previous save state** using the backup created before the
    update.

## 💾 How to Back Up Your STALKER 2 Saves

Before updating Borscht, we strongly recommend making a manual backup of your current save files—especially if you plan to continue an existing playthrough after the update.

### 1. Completely Exit STALKER 2

Make sure **STALKER 2 is closed** before making your backup.

### 2. Open Your Save Location

Press:

**`Windows Key + R`**

Paste the following into the Run box:

`%LOCALAPPDATA%\Stalker2\Saved\STEAM`

Press **Enter**.

This will take you directly to your STALKER 2 Steam save directory.

The full location is normally:

`C:\Users\<Your Windows Username>\AppData\Local\Stalker2\Saved\STEAM\`

### 3. Back Up the `SaveGames` Folder

Inside the `STEAM` folder, locate:

`SaveGames`

**Copy the entire `SaveGames` folder** somewhere outside of the STALKER 2 directory.

For example, you could create:

`Documents\Borscht Save Backups\`

Then rename the copied folder so you know exactly when and why it was created:

`SaveGames - Before Borscht 2.0.5.3`

That's it. You now have a complete backup of your save from **before the Borscht update**.

---

## 🔄 If You Need to Restore the Backup

If the updated Borscht revision causes problems with your existing playthrough:

1. **Exit STALKER 2 completely.**

2. Return to:

   `%LOCALAPPDATA%\Stalker2\Saved\STEAM`

3. Make another copy of the current `SaveGames` folder first if there's anything in it you may want to preserve.

4. Remove the current `SaveGames` folder.

5. Copy your backed-up `SaveGames` folder back into the `STEAM` folder.

6. Make sure the restored folder is actually named:

   `SaveGames`

You can then switch MO2 back to the matching **`[NoDelete]` Borscht profile** you preserved before the update.

### ⚠️ Important

Your **MO2 profile backup and save backup go together.**

The `[NoDelete]` MO2 profile preserves the **old mod configuration**.

The `SaveGames` backup preserves the **save before it was loaded or modified by the new configuration**.

If you update Borscht, load your existing game, discover something is wrong, and then continue saving over that game, simply switching back to your old MO2 profile may **not** undo whatever happened to the save.

**When testing an existing save after a Borscht update, keep your pre-update save backup untouched until you're confident everything is working correctly.**

## Recommended Update Procedure

1.  **Copy your current Borscht MO2 profile.**
2.  **Add `[NoDelete]` to the copied profile's name.**
3.  **Back up your STALKER 2 save files.**
4.  **Update Borscht through Wabbajack.**
5.  **Launch the updated list and test your existing save.**
6.  If anything appears broken or unusual, **do not continue saving over
    your existing game.**
7.  Exit the game, restore your backed-up save if necessary, and return
    to your preserved `[NoDelete]` profile.

> \[!IMPORTANT\] For significant Borscht or STALKER 2 updates,
> **starting a new game remains the safest option.**
