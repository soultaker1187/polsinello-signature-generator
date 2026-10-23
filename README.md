# Polsinello Team Signature Generator

A self-contained branded email signature generator for The Polsinello Real Estate Team — eXp Realty Brokerage.

Built to deploy as a single static HTML file on Vercel. Zero build step. Zero dependencies.

## What it does

- Generates on-brand HTML email signatures for any team member
- Produces personalized markdown install guides (Gmail / FUB / Apple Mail)
- Locks all team-wide content (brokerage, phone, social links, review URL, trust bar)
- Smart input handling: `(R)` → ®, `|` → proper spacing, phone auto-formats and builds tel: link
- Live preview before download
- Validates phone numbers to catch typos

## Deployment

### Option A — drop into existing Vercel project (recommended)

If you already have `polsinelloteam.ca` connected to Vercel:

1. Go to `github.com/Soultaker1187/polsinelloteam.ca`
2. Click **Add file** → **Upload files**
3. Either:
   - Upload `polsinello-signature-generator.html` to the root → accessible at `/polsinello-signature-generator.html`, OR
   - Create a folder called `signature-generator` and upload as `index.html` → accessible at `/signature-generator`
4. Commit. Vercel auto-deploys within 30 seconds.

### Option B — standalone Vercel project

1. Create new GitHub repo
2. Upload `index.html` to the root
3. Connect repo to Vercel as new project
4. Deploy

## Files

- `index.html` — the entire app (HTML + CSS + JS in one file)
- `vercel.json` — Vercel config (optional, for clean URLs)
- `README.md` — this file

## Brand-locked content (do not edit)

All of these are hard-coded into the generator. If they change team-wide, edit `index.html` and redeploy:

- Team name: The Polsinello Real Estate Team
- Brokerage: eXp Realty, Brokerage
- Website: GreaterTorontoHomePros.com
- Review URL: g.page/r/CROgSV4IGVV4EBM/review
- Social: Facebook, Instagram, LinkedIn, X, YouTube (team accounts)
- Trust bar: 5,000+ Homes Sold · $3B+ in Sales · 37+ Years · 1,230+ Google Reviews
- Colours: Deep Navy `#0B1E3B` · Metallic Gold `#C5A059` · White `#FFFFFF`

## License

Internal use only — The Polsinello Team.
