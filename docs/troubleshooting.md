# Fix common issues

For installation problems, start with the VPM checks below. For outfit problems, check the selected object, the Wardrobe index, and avatar compatibility.

## The VPM installation link does not open

The **Open in VCC / ALCOM** link uses the `vcc:` URL scheme. An installed app must handle that scheme, and your browser must allow it to open.

Use the [manual repository steps](before-you-begin.md#add-the-vpm-repository) if the link does nothing. If ALCOM settings offer **Use ALCOM for vcc: URL Scheme**, enable it and select **Register URL Scheme Handler Now**. These controls depend on your platform; use manual entry if they are absent.

## Avatar Wardrobe is missing from Manage Packages

Confirm that you added the [Avatar Wardrobe repository](before-you-begin.md#add-the-vpm-repository), then refresh the package list for the target project and search for **Avatar Wardrobe**. Regular releases do not require prerelease packages to be enabled.

If installation reports that Modular Avatar cannot be found, add its repository using the [Modular Avatar installation page](https://modular-avatar.nadena.dev/docs/intro), then refresh and retry.

## The Avatar Wardrobe command is missing in Unity

Check that Avatar Wardrobe is installed in the correct project and that you applied the package changes in VCC or ALCOM. Reopen Unity, wait for compilation to finish, and look for **Tools → Avatar Wardrobe**. If compilation fails, open the **Console** and resolve the reported errors before trying again.

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
