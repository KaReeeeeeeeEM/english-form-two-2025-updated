# Conversion report

## Result

- Book: **English Form Two (2025 Updated)**
- Source pages: **96**
- Strategy: **fixed layout**
- Page structuring: **96/96**
- Web rendering: **96/96**
- Image captioning: **96/96**
- Glossary generation: **10/10 batches**
- Accessibility assessment: **96/96**
- Packaged entry point: `books/english-form-two-2025-updated/adt/index.html`
- Published reader: <https://kareeeeeeeeem.github.io/english-form-two-2025-updated/>

## Audit

The source was surveyed across all 96 physical PDF pages. A 22-page canonical
pilot covered front matter, chapter openers, regular lessons, activities,
tables, illustrations, summaries, and final pages. The final packaged book was
then opened in the ADT reader and every page was captured in sequence from page
1 through page 96. All pages loaded, exposed semantic text, and passed reader
navigation checks.

The print PDF contains unusually fragmented InDesign artwork: individual
header and footer designs contain hundreds of overlapping masks and image
shards. Browser compositing of those fragments caused a clipped cover title and
duplicated dark furniture. The final fixed-layout package therefore uses each
ADT-extracted full-page render as the authoritative visual layer and keeps the
positioned semantic text as an invisible accessibility layer. All 96 bundled
page rasters were byte-compared with their extracted source renders, and all
96 matched. A second 96-page browser pass confirmed that every page has both
the authoritative visual layer and semantic text.

The read-aloud accessibility pass excludes repeated running-title decoration,
printer furniture, and standalone printed folios from narration on all 96
pages. Table-of-contents dot leaders remain visual but are silent; terminal
Roman folios use explicit spoken labels (for example, `v` as “Roman numeral
5” and `vi` as “Roman numeral 6”). A packaged-runtime scan found no exposed
running furniture or printed page numbers.

Image descriptions are included in read-aloud and enabled by default for new
reader sessions. The package contains audio for all 92 meaningful raster-image
descriptions across 29 illustrated pages; decorative page crops, running
furniture, and vector ornaments are not narrated. The cover Certificate of
Approval is described in detail, including certificate number 1583, issuing
ministry, publication title, author and publisher, ISBN, approval date,
curriculum context, and signatory. The packaged certificate description has a
matching audio file and remains available as image alternative text without
duplicating the authoritative visual page layer.

## Local artifacts

- Durable ADT book directory: `books/english-form-two-2025-updated/`
- Final HTML package: `books/english-form-two-2025-updated/adt/`
- Browser audit captures: `books/english-form-two-2025-updated/audit/browser-pages/`
- Audit contact sheet: `books/english-form-two-2025-updated/audit/all-pages-contact-sheet.jpg`
- Canonical pilot: `books/english-form-two-2025-updated/pilot/canonical/`

These paths are intentionally ignored by Git because the generated directory
contains the source copy, database/cache, and tens of thousands of extracted
assets.
