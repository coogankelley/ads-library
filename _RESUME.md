# Resume — Next Wave Ads Library build

## GHL GATE — DONE + TESTED LIVE (2026-06-26)
- Funnel "Ads Library Gate" → form "Ads Library Opt In" (First Name + Email) at
  kchealthwellness.com/ads-library. On Submit → Redirect to https://coogankelley.github.io/ads-library/.
- This GHL form version has NO inline add-tags, so the tag is applied by a workflow:
  trigger "Form Submitted" (filtered to THIS form) → Add Tag `ads-library-access`
  (tag id OwxziDcrisBskPT0rqPn, created via API with GHL_API_KEY; OAuth token lacks the tags scope).
- Tested end-to-end 2026-06-26: submit → lands on library + contact gets the tag. Workflow Published.
- Note: it's a capture/tracking gate, not a lock. The Pages URL is public (noindex only).

## PICK UP HERE (2026-06-24 eve) — DEPLOYED LIVE
- Pushed to main 2026-06-24 (auto-deploys ~1 min). Strict build passed, no em dashes.
- This deploy bundled: the morning's 11 edits + recording.md, PLUS the mentorship-call changes:
  (1) recording.md = film VERTICAL now (4:5 & 16:9 beat 1:1; discernment per ad; leave live
  horizontal/1:1 ads alone); Amazon gear links added (tripod B0F21SDXR2, laptop/eyeline stand
  B0D1N12YH5, lavalier mic B0FQBSMB4H).
  (2) editing-capcut.md = ratio step now 4:5/16:9 (1:1 dropped); added the "build in 16:9 with a
  4:5 guide frame so you can crop to 4:5 without rebuilding" tip; export step updated.
  (3) testing.md = NEW phased rollout (Phase 1 V1 all hooks 7d → Phase 2 V2 retest losers, V1
  still running → 3-5 winners → Phase 2.5 V3 = one ad set per winner re-recorded in new
  settings/outfits → Phase 3 ride top 2-3); added WEBCLASS registrations to winner criteria.
  (4) strategy.md = reconciled its Phase 1/2 with the V1/V2/V3 rollout (fixed old "3-5 rounds"
  to V1 then V2; Phase 2 now flagged as the V3 settings test).
  (5) hook-test-tracker.md = documented new WEBCLASS columns + UTM attribution explanation.
- TRACKER BUILD (done 2026-06-24, separate from the site):
  - Lead sheet "Next Wave - Kelley lead sheet" (17Sjb5MhmL_gFsFfbbCPXYQFFyaBlJiA2GE7hjhNbfQg):
    added cols D-G = DATE | UTM SOURCE | UTM CAMPAIGN | HOOK. GHL workflow now maps Latest
    Attribution UTM fields into them (Kelley updated the workflow 2026-06-24). Only stamps NEW
    regs going forward.
  - Live hook tracker (1ZhyUnMYlPiBgVosthZDDd8udfS66D1rbuK0RXMIju_k) + template
    (11opibDetlxnYH1UqB28eldr0s96nPuPnDAJGCuPEjbA): added WEBCLASS group cols O-Q =
    Registrations | Reg Rate | Cost/Reg. LIVE one auto-counts via
    COUNTIF(IMPORTRANGE(lead sheet G:G), hook id); TEMPLATE Registrations is manual (partners
    have own lead sheets). Reg Rate %-formatted, Cost/Reg $-formatted.
  - Meta UTMs were ALREADY wired in scripts/meta/build_campaign.py (utm_content={hook}).

## (history below) PICK UP HERE (2026-06-24 afternoon) — edits applied, NOT pushed yet
- 11 content edits applied this morning + recording.md drafted. Strict build passes, no em dashes.
  NOTHING pushed/committed yet — site is unchanged live. Push all as ONE deploy once recording
  is finalized (Kelley still needs to read recording.md + give 2 Amazon links).
- Edits applied (all done):
  - index.md: (1) worked-example line now says Next Wave = Kelley's branch of Team Overflow,
    "the team" = Team Overflow; (2) added winning-ad reassurance para to "Why this matters now"
    ("if you have a winning ad running, don't change anything"); (3) deleted "The plan, before you
    build anything" section, folded a tighter version into end of "Why this matters now"
    (her wording: "we don't just make ads and hope, we're building off a strategy..."); (4) cut
    "A few ground rules" section; (5) cut "Templates" section from homepage body (still in nav).
  - foundations.md: 3 example lead-ins "Don't say" -> "Don't just say"; "show this instead" ->
    "show this as I say it"; added "## Two ground rules" (hard work / done beats clever) before Next.
  - strategy.md: line 3 "know the plan" -> "know the strategy".
  - compliance.md: replaced "No fake scarcity" section with "## Scarcity: use the real kind, never
    the fake kind" (explains the psychology, says fake scarcity gets flagged); added a Claude
    compliance-check paragraph after the 7-point sweep.
  - hooks.md: stripped the "500-hook pattern library" reference (we're NOT giving partners the doc);
    kept the 24-patterns teaching. Decision: most partners will AI-generate hooks anyway.
- recording.md: REWRITTEN from placeholder into a full researched best-practices page (setup once,
  eyeline, horizontal, lighting, audio, gear, teleprompter apps, reading-without-looking-like-reading
  = sit back + glance-and-grab + read at top, delivery/pace-up, batch hooks, b-roll). STILL OPEN:
  Kelley to (a) read + edit, (b) supply 2 Amazon links (phone tripod + eyeline/laptop stand) that
  replace the two "*(Amazon link to add)*" placeholders in "### The gear".
- THEN: push all to main (auto-deploys ~1 min). Confirm em-dash-free + `mkdocs build --strict` first.

---


## Open thread for next session (Kelley reading through 2026-06-23 eve)
- Kelley is reading every page and tracking edits; she'll report a batch back. Wait for her list.
- Done 2026-06-23 eve: (1) Hook test tracker TEMPLATE created = a COPY of her live tracker,
  blanked inputs (formulas kept), shared reader, /copy link on new page
  `docs/swipe-files/hook-test-tracker.md`. Template sheet id 11opibDetlxnYH1UqB28eldr0s96nPuPnDAJGCuPEjbA.
  HER ORIGINAL (1ZhyUnMYlPiBgVosthZDDd8udfS66D1rbuK0RXMIju_k) was NOT touched.
  (2) Team-wide language: removed "your ADS REFERENCES folder" refs (partners lack it) ->
  point to Templates / generic. Worked-example "Next Wave" refs kept (they're labeled examples).
  (3) Added "Why this matters now" intro on the home page (Meta AI delivery / creative-led).
- CAUTION (Kelley): never edit her live trackers; work on copies or build new.
- Open Q for tomorrow: the "500 universal hooks" doc isn't shared with partners yet (hooks.md
  now just describes it). Decide whether to share/copy it as a template too.
- Latest design: blue-teal palette (page #e4f1f8, panel #d4e7f2, accent #1273a0), white content
  card, navy header, Georgia. Left nav decluttered (removed toc.integrate). Templates now LAST
  (both nav section and on the homepage body).
- STILL PENDING (the real last milestone): the GHL gate — opt-in at kchealthwellness.com/ads-library
  that tags the contact + redirects to https://coogankelley.github.io/ads-library/.
- Stylesheet cache note: reusing a filename made Safari serve stale CSS; fixed by renaming to
  brand-v2.css. If a CSS change ever "doesn't show," rename the file (or hard-refresh).

## Styling + structure (2026-06-23, post-launch tweaks)
- Brand: teal frame + navy + Georgia. Page bg #e6f4f1 (matches KPI tracker band), deeper-teal
  left menu panel #cfe6e0, WHITE content card, navy header. Vars set on
  `[data-md-color-scheme="default"]` (NOT :root, which Material's scheme block beats).
  nav features: sections + expand + toc.integrate so all links live in the left panel.
- Nav order: Start here, Foundations, Compliance, then stages 1-5. Headlines moved to stage 4
  (Posting). KPI trackers page added under Templates (`docs/swipe-files/kpi-trackers.md`).
- KPI tracker sheets shared link-sharing=reader; page uses `/copy` links so partners copy their
  own. NOTE: these are the blank template copies — Kelley keeps real data in a separate sheet.
- "Kelley" name removed from all library content (reframed to "The Next Wave" / "what works").

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
