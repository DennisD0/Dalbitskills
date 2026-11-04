# Dalbit keyword database

Spreadsheet ID: `1gg7k46Hmakfw_Z08T07y0Wsx9qLNX2GtSUW1dqLbYoM`

URL: https://docs.google.com/spreadsheets/d/1gg7k46Hmakfw_Z08T07y0Wsx9qLNX2GtSUW1dqLbYoM/edit

Use the connected Google Drive / Google Sheets tools and their range safety guidance. Read metadata and headers before reading or updating records. Sheet and table IDs are discoverable; never assume previous row positions or used bounds are current.

## Schema

- `Keywords`: header row 7, data begins row 8. A Keyword, B Characters, C Tag length fit, D Observed uses, E Draft uses, F Reuse guidance, G Last checked, H Notes. One row per normalized keyword. B:E are formulas. F options are Check product fit, Avoid generic wording, Review wording, Do not use.
- `Usage`: header row 1. A Keyword, B Listing / draft ID, C Placement, D Evidence, E Source URL, F Checked / drafted, G Notes. Placement options are Title, Tag, Description. Evidence options are Observed, Draft, Retired.
- `Listings`: header row 1. A Listing ID, B Observed title, C Listing URL, D Checked, E Seller tag coverage, F Exact seller tags, G Notes. Coverage options are Pending sign in, Verified, Partial. Keep exact title/tag text here; do not replace observed content with proposals.

The initial import on September 24, 2026 contains 38 public shop titles, 222 distinct normalized keywords and phrases, and 415 usage records. It also contains 13 earlier draft tags, identified separately. This is historical import context, not a current count. The connected Etsy API can now verify current listing titles and exact seller tags, including drafts and inactive listings. It does not provide Listadum metrics. Public related searches and recommendation chips must not be treated as exact seller tags.

## Read and choose

Read current Keywords headers and a bounded populated range on every skill launch. Once the product is available, inspect relevant Usage and Listings rows by keyword or listing ID. Use current table bounds to page if needed. Check Do not use, Review wording and historical generic phrases before selecting terms. The library is a reusable starting point, not a restriction against introducing a relevant new phrase.

Normalize keyword keys to lowercase, trim outer whitespace, collapse repeated spaces, and standardize dash separators to spaces. Preserve the exact displayed copy in listing records or usage notes where necessary. Do not stem distinct terms or combine different listing IDs. Counts measure matching usage records, not impressions, demand, competition or conversion. Never fill missing research metrics with estimates presented as measured values. When actual research is available, retain its source, metric definition, period and retrieval date in notes or a clearly defined future research extension.

## Maintain after drafting

1. Re-read affected rows and the last populated bounds immediately before writing. Reuse the current draft's stable ID for revisions; for a new product without an identified Etsy listing, create a draft ID from the user-supplied SKU and creation date/time. The SKU is required to locate and verify the exact product master row before drafting. Include a known Etsy listing ID in notes or use it directly when the draft applies to that verified listing.
2. Add or update one Usage record per keyword + listing/draft ID + placement + evidence. Newly generated phrases are Draft even if the listing already exists. Write the generated title in the notes of its draft Title entries so the selected wording is recoverable. Never call a generated tag Observed until it is actually verified in Etsy, Listadum or a supplied seller export. Date the read or draft accurately and leave unavailable source URLs blank with the reason in Notes.
3. Preserve verified historical evidence and user notes. For changed drafts, retain previous terms as Retired instead of silently treating them as current. Avoid duplicate log rows when rerunning the same draft. Observed records describe the last verified state; do not claim continuous synchronization.
4. Add missing normalized terms to Keywords. Copy formula and formatting conventions from an adjacent data row. Maintain `LEN` and the 20-character length check. Observed and Draft counts use `COUNTIFS` against Usage A and D. Extend BOTH formula ranges to cover every used Usage row for ALL keyword rows when records are appended. Do not leave older keyword counts bounded to the initial import.
5. Expand native table ranges to include appended rows; preserve dropdowns, formulas, column names, widths and source links. Dates should remain typed dates. Read back the affected entries and a representative count before reporting the database saved.
6. Update Listings observed titles or exact seller tags only when verified. `etsy_get_listing` is an authenticated source for both. Keep the API's `tags` and `materials` separate; do not copy material values into seller tags. If the API returns an empty tags array, record that as a verified empty array with source and retrieval date, distinct from a blank cell meaning unavailable. Observed keyword Usage rows should reflect exact API tags/title, while proposed replacements remain Draft until an Etsy update is applied and read back.

Etsy guidance checked September 24, 2026:

- Tags: https://help.etsy.com/hc/en-us/articles/360000336307-How-to-Use-Tags-to-Get-Found-in-Search
- Keyword relevance: https://www.etsy.com/seller-handbook/article/keywords-101-everything-you-need-to-know/382774281517
- Title readability: https://www.etsy.com/seller-handbook/article/1399426136697

Recheck official guidance if platform limits change. Usage history alone does not establish which terms perform best.
