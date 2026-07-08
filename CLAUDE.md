# Portfolio Demo2 — CLAUDE.md

## Project Overview
Static portfolio website for **Didla Jayaraj** — Data & AI Leader with 20+ years of experience.
Hosted on GitHub Pages at: https://didlaai2027.github.io/portfolio-demo2/

## Repository
- **GitHub:** https://github.com/didlaai2027/portfolio-demo2
- **Live URL:** https://didlaai2027.github.io/portfolio-demo2/
- **Branches:** `main` (source), `gh-pages` (deployed)

## Folder Structure
```
portfolio-demo2/
├── index.html               ← Single-page portfolio (all sections)
├── _config.yml              ← GitHub Pages config
├── .nojekyll                ← Disables Jekyll processing
├── CLAUDE.md                ← This file
├── css/
│   └── style.css            ← All styles (dark theme, responsive)
├── js/
│   └── main.js              ← Animations, typing effect, nav, filters
├── images/
│   └── profile.jpg          ← ADD YOUR PHOTO HERE (replaces placeholder)
├── resume/
│   └── Didla_Jayaraj_Resume.pdf  ← ADD YOUR RESUME HERE
├── assets/                  ← Reserved for additional icons/media
├── temp/
│   └── notes.md             ← Dev notes
└── .github/
    └── workflows/
        └── deploy.yml       ← GitHub Actions deploy workflow (optional)
```

## Sections in index.html
| Section | ID | Description |
|---|---|---|
| Navigation | `nav` | Sticky navbar with smooth scroll |
| Hero | `#hero` | Name, animated title, stats, floating badges |
| Stats Banner | — | 4 key metrics counter |
| About | `#about` | Bio, highlights, social links |
| Experience | `#experience` | 5-role timeline (2004–Present) |
| Skills | `#skills` | 6 skill categories with progress bars |
| Projects | `#projects` | 6 AI/ML projects with filter |
| Achievements | `#achievements` | 8 awards and milestones |
| Certifications | `#certifications` | 9 cloud/AI certifications |
| Contact | `#contact` | Form + contact details |
| Footer | `footer` | Links + copyright |

## Key Design Tokens (css/style.css `:root`)
```css
--primary: #0f172a        /* Dark navy background */
--accent: #6366f1         /* Indigo accent */
--gold: #f59e0b           /* Gold highlights */
--text-primary: #f1f5f9   /* Main text */
--text-secondary: #94a3b8 /* Muted text */
```

## How to Customise
- **Name/title:** Search & replace `Didla Jayaraj` in `index.html`
- **Photo:** Drop `profile.jpg` into `images/` folder
- **Resume:** Drop `Didla_Jayaraj_Resume.pdf` into `resume/` folder
- **Colors:** Edit CSS variables in `css/style.css` under `:root`
- **Content:** Edit sections directly in `index.html`

## Deployment Workflow
Changes go to `main` branch. To update the live site:
```bash
# Make changes, then:
git add .
git commit -m "your message"
git push origin main

# Sync gh-pages branch (deployed branch):
git checkout gh-pages
git merge main
git push origin gh-pages
git checkout main
```

## Contact Details in Site
| Field | Value |
|---|---|
| Email | didla.jayaraj@techleader.ai |
| Location | Austin, TX |
| LinkedIn | linkedin.com/in/didla-jayaraj-ai |

## Dependencies
- No npm / no build step — pure HTML, CSS, JS
- Google Fonts (Inter) loaded via CDN
- No external JS libraries
- Works offline after first load (fonts cached)
