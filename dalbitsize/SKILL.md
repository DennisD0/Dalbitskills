---
name: dalbitsize
description: Add concise three-line bracelet details to Dalbit product photos by matching each photo's SKU to the live Product Master for size and closure, then describing visible materials from the photo. Use for Dalbit size-info photo edits, not Etsy listing copy or cultural symbol cards.
---

# Dalbit size-info photos

Work through the SKU folders under `<DALBIT_ROOT>` end to end: find an eligible full-bracelet photo, get its facts, and save an edited copy with three short lines of black serif text in the upper-left corner. Follow the user's current instructions if they change the wording, layout, or sources.

## Source of each detail

| Detail | Source | Rule |
| --- | --- | --- |
| SKU | The photo's SKU folder under `<DALBIT_ROOT>`, or a SKU supplied by the user | Use the entire folder name to locate the product row; do not print it on the image. |
| Bracelet Size | The matching row in the live [Dalbit Product Master](private-google-link) | Preserve the recorded measurement and range; do not estimate size from the photo. |
| Closure | The same matching Product Master row | Use the recorded closure type; do not infer it from a cropped or unclear photo. |
| Material | The supplied product photo | Briefly describe visible beads or cord **and the key decorative piece or pieces** (such as a butterfly, disk, fish, moon, or star charm). Do not name a specific gemstone, metal, plating, or fiber unless it is verified. |

The SKU is an **internal match key**, not one of the three displayed lines. For a source path shaped like `<DALBIT_ROOT>\<SKU>\<photo>.jpg`, read `<SKU>` from the directory immediately under the Dalbit root. Keep the complete name, including a color or variant suffix: `b01blue` is distinct from `b01`. Verify that it identifies exactly one Product Master row and that the photo is consistent with that row. Never silently substitute a similar SKU or assume `p02` means `b02`.

## Photo style and selection

Use the user's three examples as the reference for **which photo to edit**, not as sources of measurements:

- `<DALBIT_ROOT>\b01\_MG_3652.jpg` — full green-and-white bracelet with a gold sliding closure and both chain tails visible.
- `<DALBIT_ROOT>\b01blue\_MG_3647.jpg` — the similar blue-and-white variant, with its gold sliding closure and both chain tails visible. Its SKU remains `b01blue`.
- `<DALBIT_ROOT>\b06\_MG_3640.jpg` — a different green-and-white bracelet with a clasp, extension chain, and dangling flower charm visible.

Choose a full-body product shot that shows the entire bracelet and all of its parts, including closures, extension chains, tails, and charms. The bracelet should be the sole subject, with no other objects or props around it. The background will usually be white or very light; preserve its actual color and lighting. Do not select a close-up or a shot that cuts off part of the bracelet. When several photos in one SKU folder look similar, inspect each candidate and select the one meeting these criteria; use visual details to cross-check the folder identity, never to replace the folder SKU.

## Folder scope and existing outputs

- When the user gives the Dalbit root rather than individual images, scan its immediate subfolders and process only folders whose complete names match unique Product Master SKUs. Ignore non-SKU folders such as `Stone Cards`.
- Before editing a SKU, check its folder for an existing finished size photo. Recognize both descriptive filenames such as `*_size_info.png` and older generated filenames whose image visibly contains the three-line `Bracelet Size`, `Closure`, and `Material` overlay. Skip that SKU unless the user specifically asks to revise or replace the existing size photo. This keeps reruns from making duplicates; `b29`–`b32` are examples of already-completed folders.
- Within each remaining folder, inspect the photos and choose the full-body shot yourself. Do not require the user to point out the camera filename when a clear eligible shot exists.

## Step-by-step workflow

1. **Inventory and skip completed SKUs.** List immediate folders under `<DALBIT_ROOT>`, exclude non-SKU folders, and check each SKU folder for a finished three-line size photo. Record which SKUs are already complete, then work only on the remainder.
2. **Select and inspect each source photo.** Review the remaining SKU folder's photos and choose a full-bracelet shot matching the examples above. Check that every component is in frame and the background is plain and light. Distinguish close variants by color, bead arrangement, charms, and closure details, while treating the folder name as the SKU. If an image has lost its original folder path and the user has not supplied the SKU, ask for the original path or SKU.
3. **Match the product.** Read the current Product Master and find the exact SKU in the current sheet structure. Confirm one unique row. If the SKU is missing, duplicated, or conflicts with the photo or user-provided details, ask for clarification before editing that photo. Continue with other photos whose matches are clear.
4. **Read size and closure.** Copy those fields from the verified row. Preserve the Product Master's value, including any size range and units. Do not carry measurements or closures over from another product. If either field is blank or unclear, ask for the missing value rather than inventing it. When the user supplies corrected values and authorizes updating the Product Master, write them to the exact SKU row and verify the saved cells before using them on the image.
5. **Describe visible materials and key pieces.** Inspect the selected photo. Name the main beads or cord and each meaningful focal charm or pendant in the `Material` line, for example `Pink beads and floral charm`. Describe appearance when composition is uncertain; a visual match alone does not establish stone or metal type. Keep the line concise enough to fit cleanly.
6. **Prepare the exact three lines.** Use this order and labels, with no title, SKU, extra claims, or fourth line:

   ```text
   Bracelet Size: 6 3/8"
   Closure: Elastic
   Material: Pink beads and floral charm
   ```

   These values are an example only. Replace all three values with facts for the current photo.
7. **Edit the photo.** Use the available image-editing workflow and treat the selected photo as the edit target. Place the exact text in black serif type in the upper-left with generous margins, using the clear background space without covering any bracelet part. Keep the bracelet, composition, background, lighting, colors, and dimensions as close to the original as the editing tool allows. Add no other objects, logos, watermarks, or text. For a batch, edit each photo separately with its own exact text.
8. **Inspect and correct.** Review each output at readable size. Check all three labels and values character by character, especially fractions, inch marks, ranges, and closure spelling. Check that every bracelet component remains in frame and the text does not cover it. If text is distorted or a detail is wrong, make a targeted correction and inspect again. Do not describe a faulty output as finished.
9. **Save and deliver.** Preserve the original photo. Save each finished edit inside the exact SKU folder that supplied its source photo: `<DALBIT_ROOT>\<SKU>\<SKU>_size_info.png`. Do not leave the deliverable only in a temporary or download folder, and do not place it in a similar SKU's folder. Before finishing, verify that the saved file exists in the correct folder and that there is only one finished size photo for that SKU. If the user explicitly specifies another destination, follow that instruction. Show each edited image and link to its saved file. Briefly identify completed and skipped SKUs, and flag any photos that need source clarification.

If the user asks only for the three-line wording, complete steps 1–6 and return the copy without editing an image.
