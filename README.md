# bestagencycalltracking.com

Site 27 of the call-tracking review network. Static HTML/CSS/JS, deployed via GitHub Pages. Built by `scripts/build_site27_pages.py`.

## Build details

- **Template:** T27 Best Agency Call Tracking (data-forward dashboard, light)
- **Accent:** Slate `#334155` / dark `#1E293B` / soft `#F1F5F9`, blue highlight `#2563EB`
- **Background:** White `#FFFFFF`
- **Fonts:** Inter Tight (display) + Inter (body)
- **Signature visual:** multi-client agency dashboard scorecards (`.dash-panel`, `.agency-board`) showing per-client overhead and sub-account counts, plus a per-client cost table (`.cost-table`)
- **Author byline:** Nathan Brooks (agency operations analyst, ROI / per-client-overhead focus)
- **Angle:** decisive "best for agencies" pick; multi-client management, white-label, per-client economics, reporting

## Pages (12)

- `index.html` — homepage / 2026 ranked agency guide
- `reviews/callscaler/` (#1, 9.4), `reviews/callrail/` (8.5), `reviews/calltrackingmetrics/` (8.3), `reviews/whatconverts/` (8.1), `reviews/invoca/` (7.6)
- `about/`, `methodology/`, `faq/`, `contact/`, `privacy-policy/`, `terms/`

## CTA destination

All CallScaler CTAs link to `https://callscaler.com/?ref=bestagencycalltracking`. Competitor review pages use a soft `.tldr-crosslink` + internal `/reviews/callscaler/` link only (no hard affiliate button), per network convention.

## Rebuild

```bash
py scripts/build_site27_pages.py
py scripts/lint_site.py bestagencycalltracking
```

## TODOs before going live

- [ ] Replace placeholder author avatar with a real photo if a named author is used
- [ ] Confirm CallScaler pricing tiers still current ($0 PAYG / $45 Pro / $130 Agency / $400 Pay Per Call)
- [ ] Verify schema with Google's Rich Results Test
- [ ] Set up `editor@bestagencycalltracking.com` email forwarding
- [ ] Add to `scripts/deploy_all_sites.py` SITES list before deploying
- [ ] Keep clearly differentiated from sibling site #29 agencycalltracking.com (this one = decisive "best", data/dashboard, slate; that one = generic agency guide)
