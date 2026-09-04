# Add an outfit with Avatar Wardrobe

Avatar Wardrobe searches the outfit assets in your Unity project. It does not download clothing from a shop or create a new outfit. It helps you find and install outfits that are already available in the project.

## Select the avatar instance

Before you open Avatar Wardrobe, select the avatar instance that you are editing in the **Hierarchy**.

## Open Avatar Wardrobe

From the **Tools** menu, select **Avatar Wardrobe**.

In the Avatar Wardrobe window:

1. Check that **Install target** shows the avatar you selected.
2. Select **Open Wardrobe**.
3. Keep the Unity window open while you browse. Avatar Wardrobe installs outfits on the target shown in **Install target**.

## Update the outfit list

Before you search for an outfit, update the list if this is the first time you have opened the project or if you recently added outfit assets. The index is a searchable list of the assets in the project.

- Select **Index changes** after you add or change outfit assets.
- Select **Rebuild** if an outfit is missing or the list is out of date.

You do not need to rebuild the list every time you open Avatar Wardrobe.

## Search for an outfit

Enter an outfit name, color variant, or folder path in the search box. Use the following filters to narrow the list:

- **Compatible** — outfits that are the best choices to try first.
- **Installed** — outfits already on this avatar.
- **Unknown** — outfits that Avatar Wardrobe could not confidently test.
- **Hair**, **Outfits**, or **Gimmicks** — categories of assets.

Select an outfit card to review its variants, compatibility, parts, materials, and performance details.

| Label | Meaning |
| --- | --- |
| **Compatible** | Avatar Wardrobe found a good match. |
| **Likely compatible** | The match looks promising, but is not fully confirmed. |
| **Not compatible** | The outfit was made for a different avatar setup or does not match well. |
| **Untested** | Avatar Wardrobe could not test enough information to decide. |

## Add the outfit to the avatar

After you choose a variant, select **Add to Avatar**.

If you want Avatar Wardrobe to create menu controls automatically, leave **Create toggles** selected. Avatar Wardrobe adds the outfit to the selected scene avatar and makes it the default outfit. The main menu control is named **Wear This Outfit**.

!!! warning "Install an incompatible outfit"
    **Advanced install (allow incompatible)** lets you add an outfit marked as incompatible. Try a compatible variant first. If you use this command, you might need to adjust the outfit manually.

## After installation

When installation succeeds, Avatar Wardrobe creates controls for the outfit if **Create toggles** was selected. Installed outfits remain visible while you edit the avatar in Unity. The generated menu controls which outfit is active when the avatar is running in VRChat.

To create or update controls yourself, see [Create outfit toggles](outfit-toggles.md).
