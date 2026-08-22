# Kim Formanes Affiliate Lab — Original Funnel

This is an original two-page funnel inspired only by the overall structure of your reference screenshots.
It does not copy the reference site's wording, branding, graphics, colors, or product offer.

## Branding
- Deep ink navy
- Warm cream
- Muted coral
- Teal + mint accents
- "Affiliate Lab" positioning: practical, organized, data-aware, beginner friendly

## Pages
- `/` → opt-in landing page
- `/start/` → free Affiliate Starter Class + roadmap
- `/resources` → keep your existing resources/shop page
- `/affiliate-starter-roadmap.pdf` → keep your existing PDF at the repo root

## Upload to your existing GitHub repo
Replace your current root `index.html` with the new one.
Create `start/index.html` using the included file.
Keep your existing `resources/index.html`.
Keep `affiliate-starter-roadmap.pdf` at the repo root.

Expected structure:

```
affiliate-roadmap/
├── index.html
├── affiliate-starter-roadmap.pdf
├── resources/
│   └── index.html
└── start/
    └── index.html
```

Vercel will redeploy automatically after you commit.

## Optional free Google Sheets lead capture
The landing page already redirects to `/start/` after submission even before Google Sheets is connected.

To save leads:
1. Create a Google Sheet named `Affiliate Roadmap Leads`.
2. Row 1: `Timestamp | First Name | Email | Source`
3. Extensions → Apps Script
4. Paste `google-apps-script.js`
5. Deploy → New deployment → Web app
6. Execute as: Me
7. Who has access: Anyone
8. Copy the `/exec` URL
9. In `index.html`, replace `PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE` with that URL.

## Future option
If you later record actual video lessons, the `/start/` page can be upgraded with video embeds without changing the branding or funnel.
