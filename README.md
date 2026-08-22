# EDA6427 Fall 2026 — Slide Decks

Public GitHub Pages site for slide decks used in EDA6427 (Applied Education Policy Research), Fall 2026.

**Live site:** https://ehuffaker.github.io/eda6427-fall2026-slides/

## Structure

```
module_N/
  saturday_session/          (or lecture/)
    module_N_session_slides.html
    module_N_session_slides_files/
    images/
    custom.css
```

## Publishing a new / updated deck

1. Render the source Quarto deck (e.g. from `Fall2026/Module 1/saturday_session/quarto/`):
   ```
   quarto render module_1_session_slides.qmd
   ```
2. Copy the rendered output into the matching folder here, and add the deck to `index.html`.
3. Commit and push:
   ```
   git add . && git commit -m "Update Module N slides" && git push
   ```
4. GitHub Pages redeploys in ~30 seconds.

Note: the Canvas copy is a separate `embed-resources` build (`*_STANDALONE.html`). The build mirrored here is the one that depends on its sibling `_files/`, `custom.css`, and `images/`, which is why the whole folder is committed.
