# Before you begin

Make sure you have the following software before you start. If someone gave you a complete avatar project, some of these packages might already be installed.

## Confirm the required software

| You need | Version | Why you need it |
| --- | --- | --- |
| Unity | 2022.3 or later | You use Unity to open and edit the avatar project. |
| VRChat Avatars | 3.10.4 or later | This package provides the avatar components used by VRChat. |
| Modular Avatar | 1.18.3 or later | This package adds the generated menus and controls to the avatar. |
| VRChat Outfit Tools | The version you received | This package adds Avatar Wardrobe and Avatar Outfit Toggles to Unity. |

Install the VRChat Outfit Tools package by following the instructions that came with it. You might install it through VCC or VPM, or import a `.unitypackage`. After Unity finishes importing the package, the commands are available in the **Tools** menu.

## Select the avatar instance

1. Open the Unity project that contains your avatar and outfit assets.
2. In the **Hierarchy**, find the avatar placed in the scene.
3. Select the avatar.

The avatar in the **Hierarchy** is the scene avatar instance. It is different from the saved avatar asset in the **Project** window.

!!! important "The tools edit the scene avatar"
    Avatar Wardrobe installs outfits on the selected scene avatar. It does not directly change the original prefab asset in the **Project** window.

## Select an outfit root for toggles

When you create outfit toggles, select the outfit object under the avatar in the **Hierarchy**. Do not select the avatar root.

The outfit root is usually the parent object that contains the whole outfit, such as `Casual Outfit`, `Jacket Set`, or `Summer Dress`.

If you are unsure which object is the outfit root, expand the outfit once. Select the object that contains the clothing pieces.
