# Fix common issues

Most problems come from one of three things: the wrong object is selected, the Wardrobe index is out of date, or the outfit does not match the avatar.

## An outfit is missing from Wardrobe

1. Click **Index changes** in Wardrobe.
2. If it is still missing, click **Rebuild**.
3. Turn on the option to show items with no preview if you want to inspect those assets.

Wardrobe can list assets that it cannot render a preview for, but it may hide them by default.

## “Add to Avatar” does not work

Check the **Install target** in the Avatar Wardrobe Unity window. It should be a scene avatar instance from the Hierarchy, not an avatar prefab selected in the Project window.

If the outfit is marked **Not compatible**, choose a compatible variant or deliberately enable **Advanced install (allow incompatible)**.

## The Outfit Toggles command is greyed out or shows an error

Make sure:

- the selected object is below the avatar root;
- every selected object belongs to the same avatar;
- you selected the outfit parent rather than the avatar itself; and
- multiple selected outfits have a common parent.

If you selected both a parent and one of its children, select only the parent.

## I have duplicate or outdated controls

Select the same outfit root again and run **Create or Update Outfit Toggles**. It updates the generated menu for that outfit. Avoid deleting the whole avatar to fix a menu problem; use Unity Undo if you need to step back.

## The outfit is visible in Unity when I expected it to hide

This is expected for Wardrobe-installed outfits. They stay visible while you edit the avatar. The generated Wardrobe menu controls which outfit is active when the avatar is running in VRChat.

## The toggle icons look old

Select the outfit or generated submenu and choose **Tools → Avatar Outfit Toggles → Refresh Toggle Icons**.

## Apple Intelligence options are unavailable

Name cleaning and toggle grouping are optional helpers. They need macOS 26 or newer, Apple Silicon, and Apple Intelligence enabled. You can continue with the ordinary toggle commands and rename or organize controls yourself.

## I am not sure what to select

Go back to [Before you begin](before-you-begin.md) and look for the **outfit root**: the top-level object under the avatar that contains the clothing pieces.
