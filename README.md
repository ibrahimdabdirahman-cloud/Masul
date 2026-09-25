# Masul Conservation Fund — website & brand

The public website and brand kit for **Masul Conservation Fund**, the conservation and donor-funded pillar of Masul Group (Hargeisa, Somaliland).

It is a static site with no build step: plain HTML, one stylesheet and one small script. It can be hosted on GitHub Pages, Fasthosts, Netlify or any static host.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | Home: the problem, species at stake, the five programmes, the founder's track record, how we work |
| `about.html` | Mission, values, founder profile and timeline, place in Masul Group |
| `programmes.html` | Detail on each programme, what partners can fund, and where the Fund works |
| `approach.html` | Principles, the shared operating stack, and safeguards |
| `partner.html` | Ways to partner, the Fund's current stage, reporting commitments, and the enquiry form |
| `concept-note.html` | One-page donor concept note, formatted to print to A4 or save as a PDF |
| `404.html` | Page-not-found page (GitHub Pages uses it automatically) |
| `brand/index.html` | Brand guidelines: logo, anatomy, colour, type and voice |

## Brand at a glance

The Fund uses the **Masul Group brand system V3.0** with its approved unit accent.

- **Mark:** the Cradle, in Conservation Green. Subsidiaries do not create their own icons.
- **Primary:** Conservation Green `#2E5E2E`. Deep `#1C3B1C`, Night `#132813` and Mist `#CFE0CF` are used for backgrounds and tints.
- **Parent:** Masul Red `#9B1C2E`, used for endorsement only. Ink `#111111`, Stone `#555555`, Light Grey `#EFEFEF`.
- **Type:** EB Garamond for display and quotations. Poppins (300/400/500) for the brand name and interface.
- **Voice:** professional, calm and precise, with evidence behind every claim and no exclamation marks.

Logo files are in `assets/img/`:

- `logo-horizontal.svg` and `logo-horizontal-reversed.svg`
- `logo-stacked.svg`
- `cradle-{green,white,ink,red}.svg`
- `favicon.svg`

> The Cradle SVG was rebuilt from the anatomy spec in the Brand & Market Presentation (MG-BRAND-2026-001). If a locked master vector exists, replace the `<path>` geometry in the `cradle-*.svg` and `logo-*.svg` files with it.

## Editing

- The header and footer are repeated in each HTML file. If you change them, change every page.
- The enquiry form (`partner.html`) opens the visitor's email client, addressed to `ibrahim@masulgroup.com`. To receive submissions directly, point the form at a form service such as Formspree or Resend. See `assets/js/main.js`.
- Figures on the home and about pages describe the founder's work at CCF Somaliland under LICIT II (2022–2025). They are labelled as prior delivery, not as Fund outputs. Keep that attribution when you edit them.

## Sharing and search

- Each page includes a social preview image (`assets/img/og-image.png`, 1200×630) and structured data describing the Fund.
- Once the site has a domain, change the `og:image` URL in each page to the full address, for example `https://conservation.masulgroup.com/assets/img/og-image.png`. Most social networks ignore relative image paths.
- The links in `404.html` assume the site is served from the root of its domain.

## Publishing on GitHub Pages

Go to **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` / `(root)`, and save. A `.nojekyll` file is already included.

To use a custom domain such as `conservation.masulgroup.com`, add a `CNAME` file containing the domain and create a DNS CNAME record pointing to `<user>.github.io`.
