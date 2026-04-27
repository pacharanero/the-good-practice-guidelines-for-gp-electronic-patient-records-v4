# Queries for Async Review

## Formatting and Content

1. **Chapter 8 sub-sections (8b-8f) — should these be nested under Chapter 8 in the nav?**
   Currently they appear as top-level nav items alongside the main chapters. The original structure had them flat. A nested nav under "8. Data Transfer and Interoperability" might be cleaner but would change the URL structure.

2. **Chapter 7 and Chapter 11 have empty `###` headings** (blank subheading elements with no text). These appear to be conversion artefacts from the original Word docs. Removed from ch-7 during this pass but ch-11 still has one — should all empty headings be stripped?

3. **`gpgv4-appendix.docx.md` and `gpgv4-glossary.docx.md` — rename to drop `.docx` from filenames?**
   The `.docx.md` extension is a leftover from the Word-to-Markdown conversion. Renaming would break any existing links/bookmarks but would be tidier. Suggest `appendix-contributors.md` and `glossary.md`.

4. **Chapter 8e has pandoc-style attributes** like `{#e.1-introduction .ListParagraph}` on heading lines. These are conversion artefacts and could be removed if not needed.

5. **Chapter 8c and 8f have bold-wrapped sub-headings** (e.g. `### **8c.1 ...**`, `**8f.1** **Introduction**`) instead of clean markdown headings. These could be normalised in a second pass.

6. **Copyright notice** — currently says "Copyright RCGP, BMA and HSCIC". HSCIC became NHS Digital in 2016 and was then merged into NHS England in 2023. Should this be updated?

7. **The `site/` directory is committed to the repo** and contains stale build output from the old mkdocs-material setup. Should it be added to `.gitignore` and removed from version control? (The new GitHub Actions workflow deploys from artifacts, not from this directory.)
