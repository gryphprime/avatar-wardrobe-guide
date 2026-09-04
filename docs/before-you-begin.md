# Before you begin

You only need a few things ready. If someone gave you a complete avatar project, some of these may already be installed.

## Software checklist

| You need | Version | Why it matters |
| --- | --- | --- |
| Unity | 2022.3 or newer | This is the editor where you open the avatar project. |
| VRChat Avatars | 3.10.4 or newer | This provides the avatar components used by VRChat. |
| Modular Avatar | 1.18.3 or newer | This builds the generated menus and toggles into the avatar. |
| VRChat Outfit Tools | The version you received | This adds Avatar Wardrobe and Avatar Outfit Toggles to Unity. |

Install the Outfit Tools package using the method that came with it, such as VCC/VPM or a `.unitypackage`. After Unity finishes importing it, the new commands are under the **Tools** menu.

## Open the right avatar

1. Open the Unity project that contains your avatar and outfit assets.
2. In the **Hierarchy**, find the avatar placed in the scene.
3. Click that avatar once.

The avatar in the Hierarchy is sometimes called a **scene avatar instance**. It is different from the saved avatar asset in the **Project** window.

!!! important "Wardrobe edits the scene copy"
    Avatar Wardrobe installs onto the selected scene avatar. It does not directly rewrite the original prefab asset in your Project window.

## A quick selection check

When you are working with outfit toggles, select the outfit object **under** the avatar in the Hierarchy. Do not select the avatar root itself.

The easiest choice is usually the large parent object that contains the whole outfit, such as `Casual Outfit`, `Jacket Set`, or `Summer Dress`.

If you are unsure which object is the outfit root, expand the outfit once. The object that contains the clothing pieces is usually the right one.
