# Paper thumbnails

Media shown as the left panel beside each "Selected Publications" entry on the home page.

Currently wired up in _pages/about.md:

| Paper      | File referenced by the site   | Source you provided |
|------------|-------------------------------|---------------------|
| MS-Temba   | ms-temba-web.mp4 (autoplay)   | ms-temba.mp4        |
| TimeProVe  | timeprove.png                 | timeprove.pdf       |
| UniEgo     | uniego.png                    | uniego.pdf          |
| LLAVIDAL   | llavidal.png                  | llavidal.pdf        |
| SKI Models | ski-models.png  (add this)    | —                   |
| DiffSwap++ | diffswap.png    (add this)    | —                   |
| Quo Vadis  | quo-vadis.png   (add this)    | —                   |

Notes:
- PDFs were rendered to PNG (first page) for display; the site uses the .png, not the .pdf.
- ms-temba.mp4 (69 MB) was re-encoded to ms-temba-web.mp4 (~0.5 MB, 480px, muted, no audio) for fast loading. The site uses the -web version.
- You can safely delete the source ms-temba.mp4 and the *.pdf files — the site does not load them. (Keeping them is fine too.)
- If a referenced file is missing, that paper's panel hides automatically (no broken icon).
- To re-render a PDF after updating it: pdftoppm -png -r 200 -singlefile NAME.pdf tmp && convert tmp.png -background white -alpha remove -resize 800x800\> NAME.png
- To use a different file/extension, edit that paper's <img>/<video> src line in _pages/about.md.
