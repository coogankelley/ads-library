# Resume — Next Wave Ads Library build

## LIVE as of 2026-06-23
- Site: https://coogankelley.github.io/ads-library/ (public repo `coogankelley/ads-library`,
  free plan so public; `noindex` on every page via `overrides/main.html` keeps it un-Googleable).
- Edit loop: change a file in `docs/` → commit + push to `main` → GitHub Action rebuilds &
  redeploys in ~1 min. URL never changes, so the GHL gate won't break.
- Build verified locally + on first deploy (`mkdocs build --strict`, all links resolve).
- Gotcha encoded: a docs folder literally named `templates` is auto-excluded by MkDocs, so the
  template pages live in `docs/swipe-files/` (nav label still "Templates").
- NEXT (not done): the GHL gate — opt-in page at kchealthwellness.com/ads-library that tags the
  contact and redirects to the live URL above. Minor: deploy.yml actions warn Node20-deprecated
  (still works); bump to newer action versions sometime.


Plan (approved): `/Users/kelleycoogan/.claude/plans/okay-i-want-to-sprightly-frost.md`
Format = browsable reference library (MkDocs Material). Gate = GHL opt-in at
`kchealthwellness.com/ads-library` (no password) → tags contact → redirects to GitHub Pages.

## Library structure (5 stages, 2026-06-22 restructure — Kelley's order)
1. Discovering your ICA → `finding-your-ica.md`, `conversion-quadrant.md`
2. Building your script → `ad-anatomy`, `writing-the-body`, `hooks`, `headlines-and-text`, `compliance`
3. Recording → `recording` (essentials), `editing-capcut`, `creative-broll`
4. Posting in Meta → `posting-meta.md` (Claude builds paused, Kelley publishes)
5. Tracking data → `testing`, `understanding-kpis` (NEW: baselines+glossary+formulas from
   the "Understanding KPI Tracker" doc), `metrics` (keep/kill/scale, links to the KPI ref)
Plus front matter: `index.md` (5-stage map), `foundations.md`.

## Done so far
- All pages built/adapted from the Drive "ADS REFERENCES - NEXT WAVE" folder + ad-scripts sources.
- NEW this session: `finding-your-ica.md` (from ICA doc, replaces old audience.md),
  `conversion-quadrant.md`, `headlines-and-text.md`, `posting-meta.md` rewritten as the
  Claude-uploads-Meta workflow (grounded in scripts/meta/build_campaign.py: paused build,
  one ad per hook, Kelley publishes), `editing-capcut.md` rewritten from CapCut checklist
  (no longer a stub), KPI-tracker section added to `metrics.md`, 24-pattern library added to
  `hooks.md`, script-format note added to `writing-the-body.md`.
- index.md, mkdocs.yml nav, README.md, sources.md all updated to the 5-stage order.
- audience.md deleted; all links repointed to finding-your-ica.md.
- Verified: all internal links resolve, no em dashes, nav matches files.
- Publish scaffolding (mkdocs.yml, requirements.txt, .github/workflows/deploy.yml) in place.

## Still to do
1. `recording.md` is still filming-essentials only — no filming-specific source doc exists.
   If Kelley adds filming material to `_intake/`, flesh it out.
2. Optional local render: `pip install -r requirements.txt && mkdocs build --strict`.
3. Repo creation + first push + team access — WAIT for Kelley's go-ahead.

## Waiting on Kelley
- (Optional) filming guidance for `recording.md`.
- Confirm repo name + go-ahead before any GitHub repo creation/push.
- Confirm live Pages URL so the GHL `/ads-library` form can redirect to it.
- Posting-in-Meta-with-Claude is net-new and her specific vision — worth her read first.
