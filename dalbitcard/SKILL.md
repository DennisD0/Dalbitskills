---
name: dalbitcard
description: Create Dalbit Studio cultural symbol cards using each product's Korean design element/inspiration in the Product Master, its photos, and approved brand references.
---

# Dalbit card

Create one finished square cultural symbol card for a Dalbit product. Use the matching Product Master row to identify its Korean design element/inspiration, and use that SKU's product photos as appearance references for the featured element. A close-up may show only part of the object or incidental cord, beads, or background; it is not a card template. An older Dalbit card can also supply content, but its styling is not automatically approved.

## Sources and priorities

1. Follow the user's current instructions and supplied facts.
2. Match the SKU to a fresh row in the live [Dalbit Product Master](https://docs.google.com/spreadsheets/d/194QEkWHyWEDdsgV_nMvJk_IGOhl4ZsZ2L4TwpJ7NLUE/edit) and read its `Korean design element/inspiration` field. This field identifies the card's subject; use the matching photos in `C:\Users\sshoo\Dalbit\<SKU>` for its visible form, colors, and details. Follow the user's correction or chosen label when it supersedes the recorded inspiration; otherwise do not substitute a motif guessed from a photo.
3. In the active Dalbit workspace, read `DalbitCardDesign.md` if present. Otherwise read [the bundled guide snapshot](references/DalbitCardDesign.md). Use its card-design sections through **Pre-publish checklist**; its Etsy listing workflow does not apply to card creation.
   Also read [dalbitbrand.md](C:/Users/sshoo/OneDrive/Documents/ChatGPT/Dalbit/dalbitbrand.md) for brand voice, cultural evidence boundaries, and owner-approved motif labels when present.
4. Use the user-approved images in [assets/approved-cards](assets/approved-cards), including [Blue Stone](assets/approved-cards/blue-stone.png), as visual references for the recurring Dalbit logo, layout, typography, corner frame, and footer treatment. Adapt the palette and central emblem to the element; never copy the Blue Stone palette or stone icon onto a different subject by default.

## Determine the card content

- For each bracelet, review the meaningful decorative piece or pieces, such as a focal charm, stone, bead, or pendant, and describe their visible shape and details. Do not assign symbolism to incidental hardware or every bead. Suggest a motif name when one is not already confirmed; the user's correction or chosen name is the final product label. Research each proposed cultural connection using reliable museum or cultural sources. Separate documented traditional symbolism from a modern Dalbit interpretation. If the exact motif, material, or species is unclear, flag that briefly. Never invent symbolism or claim a motif is uniquely Korean.
- Write a short cultural brief before designing the card: `Korean Cultural Element — [English name] ([Korean name])`, followed by one concise sentence explaining the supported cultural connection in warm, natural English. Keep the brief and its source in the card review packet; use it to ground the card's title and meanings. The one-sentence brief does not replace the card's three meaning labels.
- Before generating, inspect `C:\Users\sshoo\Dalbit\Stone Cards` and the Dalbit Studio Google Drive `Design Assets` folder for an existing card about the same featured element. Compare the title, subtitle, central emblem, palette, and three meanings with the proposed card. Reuse a suitable existing card unless the user asks for a revision; when a new card is needed, make its element and visual treatment distinct while keeping the approved Dalbit brand structure. The shared corner frame, moon header, and footer layout are intentional consistency, not a duplicate by themselves.
- Match the requested SKU to its Product Master row and inspect multiple clear photos from its SKU folder when available. Let `Korean design element/inspiration` determine the featured motif; let the photos determine its distinctive silhouette, colors, and intentional details. Ignore incidental jewelry, props, and background; include a cord or attachment only when it is integral to the named element. A low-resolution crop is not evidence for details it does not show. If the input is an older card, read its title, subtitle, and three meaning labels; preserve user-supplied wording unless asked to change it.
- If the SKU is unclear, the master field is blank or ambiguous without a user-chosen label, or the recorded inspiration conflicts with the photos and the user has not resolved it, ask the user to identify the intended element before generating. A photo alone does not establish its Korean name, origin, or symbolism. Do not invent those facts.
- When the user supplies a title or meaning labels, use that wording verbatim. Do not replace a requested English title with an inferred Korean color or motif name, or replace the user's meanings with researched alternatives.
- Prefer a verified Korean name or established romanization for the uppercase title, followed by a plain-English uppercase subtitle. Verify uncertain spelling.
- Use exactly three concise, distinct meanings. If the image or user supplies them, retain them. For newly proposed cultural meanings, verify unfamiliar symbolism with authoritative sources and present uncertain interpretations as editorial choices.

## Design the card

- Make a 1:1 card, targeting the production size of 1254 × 1254 px when the tool allows.
- Use a light hanji-like paper background, restrained Korean lattice-inspired corner geometry, the approved soft crescent-and-cloud header, and the small centered `Dalbit Studio` wordmark. Reproduce the recurring brand mark from the approved references; do not invent a new moon or logo.
- Place a large uppercase title and smaller tracked uppercase English subtitle directly below it. Keep `DALBIT STUDIO` vertical on both sides.
- Center **one standalone flat, clean vector-style emblem** of the featured element directly on the paper. Make it readable at thumbnail size. Do not use a product photograph, bracelet, unrelated gem or flower, circle, medallion, plate, halo, or layered badge behind it. A pearl or stone may appear when that material itself is the element.
- Use an element-led, soft pastel palette with muted dark type and restrained antique-gold accents. Avoid neon colors, harsh gradients, reflective gold tubing, and dense ornament.
- Add a wide rounded footer panel with three even columns. Give each meaning a different, simple, coordinated colored vector icon and a legible one-to-three-word label. Match the approved examples' icon weight and scale, not outline emoji or generic clip art.
- Maintain balanced symmetry and breathing room. Match the shared brand structure without forcing another card's color palette onto this element.

### Approved Blue Stone design language

The user approved [Blue Stone](assets/approved-cards/blue-stone.png) on 2026-10-01 as a style reference. Carry forward its **clarity and finish**, not its specific subject: a single strong emblem with a clean silhouette and restrained internal planes or linework; gentle texture and depth that still read as a flat illustration; ample clear space around the emblem; confident dark title with a smaller tracked subtitle; and three distinct, coordinated footer icons with labels that remain readable when one is longer. In this card, the smooth asymmetric blue stone replaced an overly literal stack of cylindrical beads. For future stones or objects, choose the object's own recognizable form instead of repeating either icon. Keep the existing moon-and-cloud header, frame, side lettering, and rounded footer as the consistent brand system.

## Produce and check

- Use the available image-generation/editing workflow. State the verified Product Master inspiration as the **element identity** in the prompt, label the matching SKU photos as **element appearance references**, and label selected approved cards as **style references**. Transform the physical object's recognizable shape into a clean standalone symbol; do not paste the source photo into the card. Include the exact title, subtitle, side lettering, and three labels verbatim in the generation prompt. The built-in image tool accepts at most five image paths in one call; choose the most informative product photo and relevant approved references within that limit.
- Inspect the result at full size. Check element identity, title spelling, subtitle placement, the Dalbit header, corner frame, both side labels, exactly three distinct footer icons, readable text, and the guide's no-badge central-emblem rule. Make targeted corrections if needed.
- Save the final PNG in `C:\Users\sshoo\Dalbit\Stone Cards` with a descriptive `Dalbit_<Element>_Symbol_Card.png` name. Preserve existing files by choosing a versioned sibling name on collision. Upload that same finished PNG to the Dalbit Studio Google Drive `Design Assets` folder that holds the approved symbol cards; verify the folder identity before upload and read back the uploaded file's name, MIME type, and parent. Check both locations for an existing copy first so reruns do not create duplicates. Show the saved image and provide both the local file link and Drive link in the final response.
- Do not add the card to the guide's **Approved examples** or revise reusable rules before the user accepts the card. After approval, follow the guide's living-document update protocol if the user asks to maintain it.
