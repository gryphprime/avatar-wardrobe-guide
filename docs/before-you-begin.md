# Before you begin

Install Avatar Wardrobe through VRChat Creator Companion (VCC) or ALCOM. These apps use VRChat Package Manager (VPM) to install the package and its required dependencies.

Installation and use require separate permission from gryphprime. See the [VPM repository and license](https://github.com/gryphprime/avatar-wardrobe-vpm).

!!! important "Try a test project first"
    The [VPM installation page](https://gryphprime.github.io/avatar-wardrobe-vpm/) currently reports that compilation and package checks passed, but fresh Unity installation testing is pending. Start with a separate test project before installing in your main avatar project.

## Confirm the required software

| You need | Version | Why you need it |
| --- | --- | --- |
| Unity | 2022.3 | You use Unity to open and edit the avatar project. |
| VCC or ALCOM | An installed package manager | You use it to add the repository, install Avatar Wardrobe, and apply updates. |
| VRChat SDK Avatars | 3.10.5 or later | This package provides the avatar components used by VRChat. |
| Modular Avatar | 1.18.7 or later | This package adds the generated menus and controls to the avatar. |
| Avatar Wardrobe | Latest regular release in the repository | This package adds Avatar Wardrobe and Avatar Outfit Toggles to Unity. |

The dependency requirements above come from the [VPM package manifest](https://gryphprime.github.io/avatar-wardrobe-vpm/index.json). VPM resolves the required VRChat SDK Avatars and Modular Avatar packages when you install Avatar Wardrobe. If Modular Avatar cannot be found, add its repository from the [Modular Avatar installation page](https://modular-avatar.nadena.dev/docs/intro), then refresh the package list.

## Add the VPM repository

1. Open the [Avatar Wardrobe VPM installation page](https://gryphprime.github.io/avatar-wardrobe-vpm/).
2. Select **Open in VCC / ALCOM**.
3. Allow your browser to open the app, then confirm the repository in the app.

If the app does not open, add the repository manually. In ALCOM, select **Repositories → Add Repository**, paste the following URL, and confirm:

```text
https://gryphprime.github.io/avatar-wardrobe-vpm/index.json
```

Use the `index.json` URL for the repository, rather than the installation page URL. You can also copy it with **Copy repository URL** on the installation page.

## Install Avatar Wardrobe

1. Save your scene and close the target project in Unity.
2. In VCC or ALCOM, open the project's **Manage Packages** page.
3. Refresh the package list and search for **Avatar Wardrobe**.
4. Install Avatar Wardrobe, then review and apply the package changes.
5. Reopen the project in Unity and wait for compilation to finish.
6. Select **Tools → Avatar Wardrobe**.

Regular releases appear without enabling prerelease packages.

### Move from an older installation

VPM automatically migrates an existing `Assets/OutfitToggleGenerator` installation. Back up your project before migrating, then follow the installation steps above. Use the VPM package for future updates instead of importing another `.unitypackage` over it.

## Update Avatar Wardrobe

1. Save your scene and close the project in Unity.
2. In VCC or ALCOM, open the project's **Manage Packages** page and refresh the list.
3. Update **Avatar Wardrobe** to the latest version, then review and apply the changes.
4. Reopen Unity and wait for compilation to finish.

If installation does not work, see [Fix common issues](troubleshooting.md#the-vpm-installation-link-does-not-open).

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
