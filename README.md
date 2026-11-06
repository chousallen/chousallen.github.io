# CARES weekly reports

Weekly progress reports for the CARES senior project: the ReXNet-150 audio classifier on the
FINALE accelerator chip design, on a DE10-Pro FPGA board.

Site: https://chousallen.github.io/cares-weekly-reports/

**This repo and its site are public.** Anyone can read every file and every past version.

## Layout
- `index.html` — list of reports, newest first, plus reference pages.
- `YYYY-MM-DD/index.html` — one report per week, a single self-contained page.
- `reference/` — pages that several reports link to (for example the datapath map).
- `.nojekyll` — GitHub Pages serves the files as they are, with no build step.

## Adding next week's report
1. Copy the latest week's folder: `cp -r 2026-11-06 2026-11-13`.
2. Edit `2026-11-13/index.html`: dates in the header, then each section.
3. Add a line at the top of the "Weekly reports" list in `index.html`.
4. Preview: open the file in a browser (light and dark mode, narrow window).
5. Check for private details (see `CLAUDE.md`), then commit and push. The site updates
   about a minute after the push.
