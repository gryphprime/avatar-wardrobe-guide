# Add an outfit with Avatar Wardrobe

Avatar Wardrobe searches the outfit assets already in your Unity project. It does not download clothing from a shop or invent a new outfit; it helps you find and install what is already available locally.

## 1. Select your avatar

In Unity’s **Hierarchy**, click the avatar instance you are editing.

## 2. Open Avatar Wardrobe

From Unity’s top menu, choose:

**Tools → Avatar Wardrobe**

In the small Unity window:

1. Check that **Install target** shows the avatar you selected.
2. Click **Open Wardrobe**.
3. Keep the Unity window open while you browse. Installs are sent to the target shown there.

## 3. Let the list update

The first time you use Wardrobe, it may need to index the prefab assets in the project. An index is simply a searchable list of what is available.

- Click **Index changes** after adding or changing outfit assets.
- Click **Rebuild** if an outfit is missing or the list seems stale.

You do not need to rebuild every time you open Wardrobe.

## 4. Search and check an outfit

Use the search box for an outfit name, color variant, or folder path. You can narrow the list with:

- **Compatible** — the best choices to try first.
- **Installed** — outfits already on this avatar.
- **Unknown** — outfits Wardrobe could not confidently test.
- **Hair**, **Outfits**, or **Gimmicks** — categories of assets.

Open an outfit card to review its variants, compatibility, parts, materials, and performance details.

Compatibility labels mean:

| Label | What it means |
| --- | --- |
| **Compatible** | Wardrobe found a good match. |
| **Likely compatible** | The match looks promising, but is not fully confirmed. |
| **Not compatible** | The outfit was made for a different avatar setup or does not match well. |
| **Untested** | Wardrobe could not test enough information to decide. |

## 5. Add it to your avatar

Choose the variant you want and click **Add to Avatar**.

Leave **Create toggles** checked if you want Wardrobe to create menu controls automatically. The outfit is added to the selected scene avatar and becomes the default outfit. Its main menu control is labeled **Wear This Outfit**.

!!! warning "Advanced install"
    **Advanced install (allow incompatible)** lets you add an outfit marked as incompatible. Try a compatible variant first. If you use Advanced install, expect that the outfit may need manual adjustment.

## What happens next?

When installation succeeds, Wardrobe creates controls for the outfit if **Create toggles** was enabled. Installed outfits stay visible while you edit the avatar in Unity; they switch through the menu when the avatar is running in VRChat.

If you want to create or rebuild controls yourself, continue with [Make outfit toggles](outfit-toggles.md).
