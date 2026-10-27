# CUS EPK viewer

Shows `epk.pdf` as a plain webpage (no PDF toolbar), with all links clickable. Built on Mozilla PDF.js v6.4.299 (legacy build, in `pdfjs/`).

On top of the links saved in the PDF, the page adds:
- **Nav buttons**: Bio / Videos / Music / Live / Contact on every slide jump to their page. The targets are set in `NAV` near the top of the script in `index.html`.
- **Email**: any email address written on a slide becomes a tap-to-email link.

## Squarespace
Paste the contents of `squarespace-code-block.txt` into a Code block on the EPK page, after replacing `USERNAME` with your GitHub username.

If your Squarespace header stays fixed at the top and covers part of a page after a button jump, set `HEADER_OFFSET` in that snippet to the header's height in pixels.

## Update the EPK
1. Export the new PDF and name it exactly `epk.pdf`.
2. Replace the `epk.pdf` file in this folder.
3. In GitHub Desktop, commit, then **Push origin**.
4. Wait 1–2 minutes, then hard-refresh the EPK page (Ctrl+F5).

If the slide order changes, update the `NAV` page numbers in `index.html`. If the number of slides changes, update the `aspect-ratio` in the Squarespace snippet: `1920 / (1080 × number of slides)`.
