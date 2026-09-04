# Create outfit toggles

An outfit toggle is a menu control that turns an avatar object on or off. Avatar Outfit Toggles creates these controls from the objects that you select in Unity.

Use this procedure in any of the following situations:

- An outfit is already in your scene.
- You want to create controls without using Avatar Wardrobe.
- You changed an outfit and want to update its generated controls.

## Select the outfit root

In the **Hierarchy**, select one or more top-level outfit objects under the same avatar.

Select the parent object for each outfit. Do not select the avatar root or each individual mesh piece.

Good selection:

```text
My Avatar
└── Casual Outfit        ← select this
    ├── Jacket
    └── Shoes
```

You can select multiple outfits when they belong to the same avatar and share a common parent.

## Create or update the controls

From the **Tools** menu, select **Avatar Outfit Toggles**, then select **Create or Update Outfit Toggles**.

You can also open the context menu for the selection in the **Hierarchy**, select **Avatar Outfit Toggles**, and then select **Create or Update Outfit Toggles**.

The tool creates a submenu and adds controls for renderable outfit parts. If a generated menu already exists for the outfit, the command updates it instead of creating a second menu.

## Test the controls

The generated submenu is added to the avatar's expression menu. Build or upload the avatar, open the menu in VRChat, and turn the outfit on and off.

If you create controls for one outfit, the submenu uses that outfit's name. If you create controls for multiple outfits, the shared submenu is named **Outfits**.

!!! note "Outfits stay visible in Unity"
    Installed outfits remain visible while you edit the avatar. The generated menu controls the outfit when the avatar is running in VRChat.

## Use the optional commands

Start with **Create or Update Outfit Toggles**. Use the other commands when you need to update an existing generated menu.

| Command | Use it when |
| --- | --- |
| **Refresh Toggle Icons** | The outfit's appearance changed and the icons are out of date. |
| **Clean Up Toggle Names** | You want friendlier toggle labels. |
| **Group Similar Toggles With Apple Intelligence** | You want to group related generated parts into one control. |

The Apple Intelligence commands are optional. They require macOS 26 or later, an Apple Silicon Mac, and Apple Intelligence enabled. Avatar Wardrobe and regular toggle generation work without them.

## Use an existing menu

If you select an existing submenu with an **MA Menu Item** component that uses **Children** as its menu source, the Avatar Outfit Toggles commands can work with that menu directly. The commands update generated controls. The grouping command leaves manual controls unchanged.
