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

## Audit

The source was surveyed across all 96 physical PDF pages. A 22-page canonical
pilot covered front matter, chapter openers, regular lessons, activities,
tables, illustrations, summaries, and final pages. The final packaged book was
then opened in the ADT reader and every page was captured in sequence from page
1 through page 96. All pages loaded, retained the source page frame and running
furniture, and exposed semantic text and reader navigation.

The print PDF contains unusually fragmented InDesign artwork. ADT Studio was
adjusted locally to batch large caption sets and to avoid duplicate semantic
paint over composite raster regions. A few isolated exercise lines retain
minor raster/semantic overlap; this is recorded as a non-blocking fidelity
limitation rather than concealed.

Speech generation was excluded for this conversion profile. The HTML text,
image captions, glossary, and accessibility assessment remain present.

## Local artifacts

- Durable ADT book directory: `books/english-form-two-2025-updated/`
- Final HTML package: `books/english-form-two-2025-updated/adt/`
- Browser audit captures: `books/english-form-two-2025-updated/audit/browser-pages/`
- Audit contact sheet: `books/english-form-two-2025-updated/audit/all-pages-contact-sheet.jpg`
- Canonical pilot: `books/english-form-two-2025-updated/pilot/canonical/`

These paths are intentionally ignored by Git because the generated directory
contains the source copy, database/cache, and tens of thousands of extracted
assets.
