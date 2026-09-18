# Borscht --- Standard Update Warning & Backup Procedure

> \[!WARNING\] **There is no guarantee that updating Borscht will be
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

`[NoDelete] Borscht 2.0.5.2`

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
