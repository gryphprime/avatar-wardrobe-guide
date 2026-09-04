# Fix common issues

Most problems have one of three causes: the wrong object is selected, the Wardrobe index is out of date, or the outfit does not match the avatar.

## An outfit does not appear in Wardrobe

1. In Avatar Wardrobe, select **Index changes**.
2. If the outfit is still missing, select **Rebuild**.
3. If you want to inspect assets without a preview, turn on the option to show them.

Avatar Wardrobe can list assets that it cannot preview, but it might hide them by default.

## Add to Avatar does not work

Check **Install target** in the Avatar Wardrobe window. It must be a scene avatar instance from the **Hierarchy**, not an avatar prefab selected in the **Project** window.

If the outfit is marked **Not compatible**, choose a compatible variant. If you still want to use the outfit, select **Advanced install (allow incompatible)**.

## The Outfit Toggles command is disabled or shows an error

Check the following conditions:

- The selected object is under the avatar root.
- Every selected object belongs to the same avatar.
- You selected the outfit parent, not the avatar root.
- Multiple selected outfits have a common parent.

If you selected both a parent and one of its children, select only the parent.

## The controls are duplicated or out of date

Select the same outfit root again, then select **Create or Update Outfit Toggles**. The command updates the generated menu for that outfit. To reverse a change, select **Edit**, then **Undo**.

## The outfit is visible in Unity

This is expected for outfits installed by Avatar Wardrobe. They remain visible while you edit the avatar. The generated menu controls which outfit is active when the avatar is running in VRChat.

## The toggle icons are out of date

Select the outfit or generated submenu. From the **Tools** menu, select **Avatar Outfit Toggles**, then select **Refresh Toggle Icons**.

## The Apple Intelligence commands are unavailable

Name cleaning and toggle grouping are optional helpers. They require macOS 26 or later, Apple Silicon, and Apple Intelligence enabled. You can use the regular toggle commands and rename or organize controls yourself.

## You are unsure what to select

See [Before you begin](before-you-begin.md) and look for the outfit root: the top-level object under the avatar that contains the clothing pieces.
