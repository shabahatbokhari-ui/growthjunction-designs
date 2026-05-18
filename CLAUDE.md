# Growth Junction · Design Direction Repo

## Purpose

Single working repo for **all** Growth Junction work. Design mockups, copy iterations, future production site code, all deliverables shared with Sulemen.

Client folder at `G:\My Drive\Claude\Clients\sulemen-khan-growthjunction\` is for **non-code artefacts only** — meeting runsheets, audio, transcripts, contracts, status.md. Anything that becomes HTML, CSS, JS, or markdown content shared via URL belongs here.

## Repo

- **GitHub:** https://github.com/shabahatbokhari-ui/growthjunction-designs
- **Cloudflare Pages:** https://growthjunction-designs.pages.dev (manual connect required once, then auto-deploys on push)
- **Local clone:** `c:\Dev\ClaudeCode\projects\websites\growthjunction-designs\`
- **Owner:** Shabahat Bokhari (@shabahatbokhari-ui)

## Workflow

Auto-deploy via Git is **NOT reliable** (CF Workers/Pages merge broke webhook 2026-05-18). Use Wrangler CLI instead.

1. Edit files in `public/`
2. `npm run deploy` to ship to `https://growthjunction-designs.shabahat-bokhari.workers.dev` in ~10s
3. Or `npm run ship` to commit + push + deploy in one command
4. Git push is for version history only, not for deploys

Requires `wrangler` installed globally + authed: `npm i -g wrangler && wrangler login`

## Current state (as of 2026-05-18)

| File | Purpose |
|---|---|
| `index.html` | Review hub. Side-by-side comparison of 3 directions. Opens first. |
| `01-editorial-premium.html` | Direction 01 — serif, HBR-style, long-form |
| `02-boutique-advisory.html` | Direction 02 — clean sans, procurement-friendly |
| `03-human-first.html` | Direction 03 — warm palette, faces, founder voice |
| `README.md` | Public-facing repo readme |

## Brand cues

- **Logo:** blue figure reaching for star (keep). Source: `https://growthjunction.ae/storage/2024/02/rsz_gjlogo.webp`
- **Logo blue:** ~`#3B6CB1` / `#2B5BA9` / `#3E6CA8` — variants used across mockups
- **Two practice pillars:** People & Org Development + Mental Health & Well-being
- **15 industries** served (see existing site)
- **Locations:** Dubai (HQ), Karachi, Bangkok
- **Founder:** Sulemen Ansar Khan, Marshall Goldsmith certified, 2000+ coachees, ex-Group HR PureHealth

## Carve-outs (from client memory)

- PureHealth / PureCS off-limits both directions — never reference as case study
- Pakistan banking / MFB carved out 60-90 days (Elevantel/Ant obligations)
- UAE healthcare deferred to Sulemen's Fakeeh board call

## Conventions

- Self-contained HTML files, inline CSS, no CDN dependencies (Sulemen may open on weak wifi)
- Wireframe-fidelity, not pixel-perfect — clearly mark placeholders
- Never use `—` (em dash). House rule.
- Logo blue must appear in every mockup, even if subtle
- All new directions get an entry in `index.html` review hub

## Don't

- Don't add real client logos or testimonials without Sulemen's written approval
- Don't reference PureHealth, PureCS, Fakeeh in copy
- Don't push to `main` without committing the matching `index.html` row update
- Don't drop client meeting notes here — those go to the Drive client folder
