# Certificates folder

`certificate-template.jpg` is the official Nova Academy certificate design
and is already wired up as the featured "Sample Template" card on the
website — no action needed for that one.

For certificates earned by individual students, place images in this folder
using these exact filenames
so they automatically appear on the website's Certificates section
(replacing the "Certificate coming soon" placeholders):

```


Notes:

- File format: `.jpg` (recommended) — if you use `.png` or `.jpeg` instead,
  update the matching `<img src="...">` path in `index.html` under the
  `#certificates` section to match your filename.
- Recommended image ratio: roughly 4:3 (e.g. 1200×900px) for a consistent
  grid — other ratios will still work but may be cropped slightly.
- You can add more than 6 certificates: copy one `<div class="cert-card">…</div>`
  block in `index.html` and update the filename and `alt` text.
- No code changes are required beyond adding the image files themselves,
  as long as you use the filenames above.
