# Magic Board Builder

Make Magic: The Gathering game boards for your AO3 fic by clicking and typing. No code to write.

**Open the builder:** `index.html` (or the GitHub Pages site once this repository is published).

## What it does

- Shows the whole table: both players' life and poison counters, hands, Library, Graveyard and Exile, the command zone for Commander, two rows of permanents per player, the phase track, whose turn it is, and the stack.
- Three kinds of game:
  - **One against one.**
  - **Two-Headed Giant** (two against two). Each partner has their own library, graveyard, hand and battlefield, sitting on the outside of their team. Each team can share one life total and poison count, as the official rules have it (one plate with both names, starting at 30), or every player can keep their own.
  - **Free-for-all** with four players, each on their own, with a colour each: purple, red, blue and gold, top to bottom.
- **Look up** fills in a card's mana cost, type line, rules text, flavour text, power/toughness or loyalty and its picture, by name, from [Scryfall](https://scryfall.com/docs/api)'s free card database. **Choose another printing** lets you pick the art you want.
- Cards can be **tapped** (turned sideways), face-down, attacking or blocking, and carry a small label for counters ("+1/+1 ×2").
- Cards in hand can be kept secret or **revealed** face-up.
- When a reader points at a card (or taps it on a phone), its details panel or its big picture opens right under it, across the board. A card has one or the other, so a picture never covers the panel's text.
- **Copy board code** gives you HTML to paste into your chapter (in AO3's HTML mode). Paste a board back in to keep editing it next turn.

## Using it on AO3

1. **Once per work:** copy the Work Skin (the button in the builder, or `ao3-work-skin.css`), create it under *Dashboard → Skins → My Work Skins → Create Work Skin*, and select it on your work's Edit page.
2. Build your board, press **Copy board code**, and paste it into your chapter with the editor in **HTML** mode.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The builder. Everything it needs is inside this one file, including a copy of the Work Skin. |
| `ao3-work-skin.css` | The AO3 Work Skin, with comments explaining every part. If you change it, paste the same CSS into the `skin-css` block near the top of `index.html` too. |
| `duel-board-template.html` | A hand-written, commented example board, for anyone who wants to edit the HTML directly. |

## Pictures

AO3 can't store images, so boards link to pictures hosted elsewhere. **Look up** fills in the card's picture link from Scryfall's image server (about 90 KB per picture), which is allowed to show on other sites.

Scryfall asks that card pictures are never cropped, stretched, recoloured, or covered where the artist's name and copyright line are printed. The Work Skin follows that: tapped cards are the whole picture turned sideways, and the badges stay clear of the bottom of the card.

To use a different picture, upload it to an image host and paste the **direct** link (it usually ends in `.jpg` or `.png`).

---

Unofficial Fan Content permitted under the Wizards of the Coast Fan Content Policy. Not approved or endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast. ©Wizards of the Coast LLC. Card data and pictures come from Scryfall, which is not affiliated with this project.
