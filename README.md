# Dalbitskills

Codex skills for Dalbit Studio, a Korean inspired jewelry shop on Etsy. Together they take a new product from a folder of photos to a reviewed Etsy listing, with a person approving each stage.

## How the skills fit together

`dalbitworkflow` runs the other four in order for one product, identified by its full SKU. It stops after each stage with a short review packet and only continues once the owner approves. Silence never counts as approval, and a resumed run picks up at the first unapproved stage.

1. `dalbitmaster`
2. `dalbitsize`
3. `dalbitcard`
4. `dalbitlisting`

## The skills

### dalbitworkflow
Coordinates the whole run. It resolves the SKU against the live Product Master, scopes each stage to the active product or a small batch, and keeps the Product Master as the single record of product facts. It never claims the workflow is complete until each stage is approved and its output verified.

### dalbitmaster
Adds missing products to the Product Master sheet. It finds SKU folders that have no row yet, looks at the photos to identify the meaningful charm or bead, and researches its Korean cultural connection in reliable museum and cultural sources. It separates documented symbolism from a modern Dalbit interpretation and never invents either. It asks the owner once for size and price, then writes and reads back the new row without creating duplicates.

### dalbitsize
Makes the bracelet size photo. It picks a full bracelet shot and adds three lines of black serif text, which are size, closure and visible materials. Size and closure come only from the Product Master row, and materials are described from what is visible, never guessed. It checks the saved image character by character and skips products that already have a size photo.

### dalbitcard
Creates the Korean cultural symbol card for a product. It reads the verified motif from the Product Master, checks local and Drive folders for an existing card, and reuses one when it fits. A new card follows the approved Dalbit brand layout with one flat emblem, a title, and exactly three meanings. It never uses a motif guessed from a photo, and it saves the card locally and to Drive.

### dalbitlisting
Prepares and updates the Etsy listing. It reads the keyword database and the keyword market sheet, then drafts a title of at most 140 characters, a warm description and exactly 13 tags. It prepares a photo faithful hero thumbnail, picks a five second video clip, and plans the photo order. It logs new keywords and uses the Etsy API to read live listings. Etsy is only changed after the owner approves the exact copy and thumbnail, and nothing is published without explicit authorization.

## Rules shared by every skill
- The full SKU, including variant suffixes, is the identity key. Facts and assets are never carried between similar products.
- A missing fact gets a question, never a guess.
- Cultural claims need reliable sources, and estimates are labeled as estimates.
- Existing files and previously approved assets are preserved.
- Nothing is written to Etsy or published without the owner's approval.

## Notes
Local folder paths, Google Sheet links and account IDs are replaced with placeholders such as `<DALBIT_ROOT>` and `private-google-link`. The card and thumbnail reference images are not included. Add your own sheets, folders and Etsy connection to run the skills.
