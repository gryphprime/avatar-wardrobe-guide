# Make outfit toggles

An outfit toggle is a menu button that turns an avatar object on or off. Avatar Outfit Toggles creates those buttons from the objects you select in Unity.

Use this page when:

- an outfit is already in your scene;
- you want to create controls without using Avatar Wardrobe; or
- you changed an outfit and want to update its generated controls.

## 1. Select the outfit root

In the **Hierarchy**, select one or more top-level outfit objects below the same avatar.

Select the large parent object for each outfit, not the avatar itself and not every individual mesh piece.

Good selection:

```text
My Avatar
└── Casual Outfit        ← select this
    ├── Jacket
    └── Shoes
```

You can select multiple outfits if they belong to the same avatar and share a common parent.

## 2. Create or update the toggles

Choose:

**Tools → Avatar Outfit Toggles → Create or Update Outfit Toggles**

You can also right-click the selection in the Hierarchy and open **Avatar Outfit Toggles**.

The tool creates a submenu and adds controls for renderable outfit parts. If a generated menu already exists for that outfit, the command updates it instead of making a second one.

## 3. Test the result

The generated submenu is added to the avatar’s expression menu. Build or upload the avatar, open the menu in VRChat, and try the outfit on and off.

With one outfit, the submenu uses that outfit’s name. With multiple outfits, the shared submenu is named **Outfits**.

!!! tip "Seeing the outfit in Unity is normal"
    Installed outfits stay visible while you edit. The generated menu controls the outfit when the avatar is running in VRChat.

## Optional commands

Start with **Create or Update Outfit Toggles**. The other commands are helpers for an existing generated menu:

| Command | Use it when |
| --- | --- |
| **Refresh Toggle Icons** | The outfit’s appearance changed and the icons are out of date. |
| **Clean Up Toggle Names** | You want friendlier toggle labels. |
| **Group Similar Toggles With Apple Intelligence** | Several generated parts should be grouped into one related control. |

The Apple Intelligence helpers are optional. They require macOS 26 or newer, an Apple Silicon Mac, and Apple Intelligence enabled. Regular Wardrobe and toggle generation work without them.

## Updating an existing menu

If you select an existing submenu that uses **MA Menu Item → Children**, the Outfit Toggles commands can work with that menu directly. Generated controls are updated; manual controls are left alone by the grouping helper.
