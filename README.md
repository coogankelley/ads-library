# The Next Wave Ads Library

Internal project doc. The partner-facing library lives in [`docs/`](docs/) and renders as a browsable MkDocs site once we push.

## What this is

A reference library for Kelley's enrolled business partners on running Meta ads for The Next Wave, from scratch. Not a course you finish in order. A searchable reference. Built off the 8-week Grow with Nat mentorship plus Kelley's own applied work on The Next Wave, adapted into her voice. Proprietary phrasing never gets pasted.

## Structure (5 stages, in order)

The library follows the real workflow: discover your avatar, write the script, record it, post it, track it.

**Start here**

| Page | Status |
|------|--------|
| [docs/index.md](docs/index.md) | done (the 5-stage map) |
| [docs/foundations.md](docs/foundations.md) | done |

**1. Discovering your ICA**

| Page | Status |
|------|--------|
| [docs/finding-your-ica.md](docs/finding-your-ica.md) | done (replaces the old audience.md) |
| [docs/conversion-quadrant.md](docs/conversion-quadrant.md) | done |

**2. Building your script**

| Page | Status |
|------|--------|
| [docs/ad-anatomy.md](docs/ad-anatomy.md) | done |
| [docs/writing-the-body.md](docs/writing-the-body.md) | done |
| [docs/hooks.md](docs/hooks.md) | done |
| [docs/headlines-and-text.md](docs/headlines-and-text.md) | done |
| [docs/compliance.md](docs/compliance.md) | done |

**3. Recording**

| Page | Status |
|------|--------|
| [docs/recording.md](docs/recording.md) | essentials (no filming-specific source doc yet) |
| [docs/editing-capcut.md](docs/editing-capcut.md) | done (built from the CapCut checklist) |
| [docs/creative-broll.md](docs/creative-broll.md) | done |

**4. Posting in Meta**

| Page | Status |
|------|--------|
| [docs/posting-meta.md](docs/posting-meta.md) | done (Claude builds the campaign paused, partner publishes) |

**5. Tracking data**

| Page | Status |
|------|--------|
| [docs/testing.md](docs/testing.md) | done |
| [docs/understanding-kpis.md](docs/understanding-kpis.md) | done (baselines, glossary, formulas, the two trackers) |
| [docs/metrics.md](docs/metrics.md) | done (keep/kill/scale; links to the KPI reference) |

**Templates**

| Page | Status |
|------|--------|
| [docs/swipe-files/body-script.md](docs/swipe-files/body-script.md) | done |
| [docs/swipe-files/hook-bank.md](docs/swipe-files/hook-bank.md) | done |

## Source material

The reference docs live in Kelley's Google Drive folder **"ADS REFERENCES - NEXT WAVE"** (inside the Next Wave folder), plus the local `ad-scripts/` files. See [`sources.md`](sources.md) for the full mapping. Nothing from those is pasted verbatim into `docs/`; it is adapted into Kelley's voice.

The one page still thin on source is **recording** (filming guidance). If Kelley adds filming material, drop it in [`_intake/`](_intake/) and that page fills out.

## Voice rules (apply to every page)

- Warm, direct, real, big-sister honest. Written for **capable partners, not beginners.**
- **No em dashes anywhere** in `docs/`. Commas, colons, periods, parentheses.
- No banned words (full list in `ABOUT ME/anti-ai-writing-style.md`).
- Cost-of-entry $ figures OK ("$5/day spend"). Income $ figures banned.
- Some source material breaks these rules (the "Financial" results examples, a few second-person "you make good money" call-outs, em dashes throughout). The framework gets kept; those specifics get cleaned to stay compliant and on-brand.
- Proprietary mentorship phrasing never gets pasted verbatim. Meta platform facts reproduce as-is.
- Every page ends with a clear next step inside the library.

## Publishing and the gate

End state: hosted on **GitHub Pages**, built from `docs/` by **MkDocs (Material theme)**. The publish files (`mkdocs.yml`, `requirements.txt`, `.github/workflows/deploy.yml`) make it turnkey: push to the repo and the Action builds and deploys.

Access is gated through GoHighLevel, not a password:

1. A partner hits the opt-in at **kchealthwellness.com/ads-library** (a GHL page, no password).
2. Submitting the form **tags the contact** in the CRM.
3. The form **redirects to the live GitHub Pages URL** for the library.

Repo creation, first push, and the live Pages URL all wait for Kelley's go-ahead.

## The old scaffolds

The old 11-topic stubs and the earlier 5-week course version live in [`_archive/`](_archive/). Kept for reference, not active.
