# iusmaris.com

Static website for **Ius Maris Climaticum** — a closed workshop on the 2024 and 2025 climate advisory opinions, against the practice of maritime law. Lund and Malmö, 8–9 June 2026.

## Structure

```
.
├── index.html         Home (hero + lede)
├── programme.html     Two-day programme, four sessions, fourteen papers
├── participants.html  Bios — to be added
├── practical.html     Venue, travel, accommodation — to be added
├── style.css          Shared stylesheet
├── assets/            Logos (LU Faculty of Law, WMU, MMW)
└── README.md
```

## Stack

Static HTML + CSS. No build step. Fonts loaded from Google Fonts:

- **Cormorant** — display serif (title, session names)
- **Source Serif 4** — body
- **JetBrains Mono** — small caps, labels, times

## Deployment

Drop the contents of this folder onto any static host (GitHub Pages, Netlify, Vercel, S3). The domain `iusmaris.com` should resolve to whichever host you choose.

For GitHub Pages: push this folder to `main` and enable Pages from the repo settings.

## Design notes

The visual language is a hybrid: dark navy canvas with a faint nautical grid for the hero and footer ("Monument + Atlas"), shifting to a warm cream paper canvas for body content ("Manuscript"). The dark band returns at the foot of the page as a closing register that also carries the institutional credits.

Hierarchy:

- **Organised by** the Faculty of Law, Lund University
- **In collaboration with** the World Maritime University, Malmö
- **Funded by** the Rune and Lena Lavin Foundation for Legal Research
- **Auspices** in part of the CCSlaw project (Lund), funded by the Marianne and Marcus Wallenberg Foundation
