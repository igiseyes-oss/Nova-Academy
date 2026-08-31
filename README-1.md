# Nova Academy — Website

A complete, static, GitHub-ready website for **Nova Academy** — "Empowering
Youth With Skills". Built as plain HTML/CSS/JS (no build step, no backend,
no Replit dependencies) so it deploys directly on Cloudflare Pages.

## Project structure

```
/
├── index.html                          Main site (single page, all sections)
├── css/
│   └── style.css                       All styling (Navy / Gold / White / Light Gray theme)
├── js/
│   └── main.js                         Mobile nav toggle only — no libraries
├── assets/
│   ├── logo.png                        Nova Academy logo (transparent background)
│   └── certificates/
│       ├── certificate-template.jpg    Official certificate design (featured sample)
│       └── README.md                   How to add more certificate images
└── README.md                           This file
```

## Sections included

Home (hero) · Courses (all 10 courses) · About Us · Certificates · Contact,
all on one page with smooth-scrolling navigation, plus a sticky header and
mobile hamburger menu.

## Replacing the logo

Swap `assets/logo.png` with your own file — keep the same filename and the
site will pick it up automatically. A transparent PNG works best since the
logo appears on both light and navy backgrounds.

## Adding certificates

See `assets/certificates/README.md` for exact filenames and instructions.
The official certificate template is already included and shown as a
featured sample on the Certificates section.

## WhatsApp / contact behaviour

- The WhatsApp phone number is **not displayed anywhere** as visible text.
- Every course's "Register / Details" button opens a WhatsApp chat
  (`wa.me` link) with a pre-filled message naming that specific course.
- The Contact section's "Contact Us on WhatsApp" button opens a general
  enquiry chat.
- "Join WhatsApp Channel" and "YouTube Channel" buttons link to the
  academy's channel and YouTube page.
- "Email Us" uses a `mailto:` link to `nova.learn253@gmail.com`.

## Deploying to Cloudflare Pages

1. Push this project to a GitHub repository (root of the repo should
   contain `index.html` directly — no extra nested folder).
2. In Cloudflare Pages, create a new project and connect that GitHub repo.
3. Use these settings:

   | Setting | Value |
   |---|---|
   | Framework preset | **None** |
   | Build command | *(leave empty)* |
   | Build output directory | `/` |
   | Environment variables | None required |
   | Root directory | `/` (repo root) |

4. Deploy. No build step runs — Cloudflare Pages serves the static files
   directly.

## Notes

- No frameworks, no npm packages, no build tools — plain HTML/CSS/JS only,
  so there is nothing to install and nothing that can fail to build.
- All links/paths are relative and production-safe.
- Tested layout: 1-column (mobile), 2-column (tablet), 3-column (desktop)
  for course cards; responsive throughout.
