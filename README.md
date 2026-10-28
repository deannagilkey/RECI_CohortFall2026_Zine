# From Awareness to Action — My RECI Zine

A personal reflection zine for the Racial Equity Consciousness Institute (RECI)
Virtual Cohort, Fall 2026 — University of Pittsburgh, Center on Race and Social
Problems.

## What's in here

- **`index.html`** / **`reci-zine.html`** — the zine itself. Same file twice,
  under two names: `index.html` so GitHub Pages can serve it directly if you
  turn Pages on for this repo, `reci-zine.html` as a plain descriptive copy.
  Open either one in a browser.
- **`reci-zine.pdf`** — a ready-to-submit PDF snapshot, generated directly
  (not through a browser print dialog), so all colors and checked
  checkboxes/radio buttons render correctly regardless of any browser's print
  settings.
- **`reci-zine.docx`** — the same content as a Word document, in case you'd
  rather edit it there or generate your own PDF from it.

## How the interactive zine works

- It's a single self-contained HTML file — no build step, no dependencies.
  Just open it in any browser.
- Every answer you type autosaves to that browser's local storage a moment
  after you stop typing (watch the "saved just now" indicator in the top
  toolbar). Nothing is sent anywhere else.
- Text boxes auto-expand to fit what you've typed, on screen and when printed.
- **Print / Save as PDF** in the toolbar gives you a snapshot any time —
  colors are forced on by default, but if they don't show up, check that
  "Background graphics" (Chrome) / "Print backgrounds" (Firefox) is enabled
  in the print dialog's "More settings."
- **Backup / Restore** in the toolbar lets you copy all your answers as
  text (for a manual backup) and paste them back in later. Known limitation:
  this has not proven fully reliable across browser sessions — treat
  `reci-zine.pdf` and `reci-zine.docx` as the durable records, not the live
  HTML's local storage.

## Structure

Cover, Why I Joined, My Journey (progress tracker + six-spheres diagram),
Navigating Racial Anxiety (companion chapter), Sphere 1: Oppression &
Liberation, Sphere 2: Identities & Biases, Scripts for Hard Conversations,
Sphere 3: Diversity & Literacy, Session 7 Workbook: Diversity Audit,
Sphere 4: Empathy & Stamina, Sphere 5: Trauma & Healing, Sphere 6:
Inequities & Justice, Through an Instructional Designer's Lens, Teaching
the Next Generation, Readings That Stood Out, Commitments, What I'll
Carry Forward, My Reading List.

Each of the six spheres has its own accent color, used consistently across
its stamp, icon, and position on the six-spheres wheel diagram.

## Sources drawn on

See the My Reading List page inside the zine for full attribution to every
article, worksheet, and resource this zine pulls from.

## Regenerating the PDF/Word doc from the HTML

If you update the HTML and want the PDF/docx to match, the content was
extracted and rebuilt using a small Python + Node pipeline (BeautifulSoup to
parse the HTML into JSON, the docx npm package to build the Word file, then
LibreOffice headless to export to PDF). Ask Claude to regenerate them from
the latest HTML if needed.
