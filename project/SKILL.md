---
name: mygig-design
description: Use this skill to generate well-branded interfaces and assets for MyGig (Australia's AI-powered Workforce-as-a-Service platform and Employer of Record), either for production or throwaway prototypes/mocks/decks. Contains essential design guidelines, colours, type, fonts, assets, and UI kit components for the marketing site, business platform, and worker mobile app.
user-invocable: true
---

Read the `README.md` file within this skill, and explore the other available files.

If creating visual artifacts (slides, mocks, throwaway prototypes, etc), copy assets out and create static HTML files for the user to view. If working on production code, you can copy assets and read the rules here to become an expert in designing with this brand.

If the user invokes this skill without any other guidance, ask them what they want to build or design, ask some questions, and act as an expert designer who outputs HTML artifacts _or_ production code, depending on the need.

## Quick orientation for the brand
- **MyGig** is a workforce platform and EOR. Voice is plain-spoken Aussie, confident, evidence-led. Sentence case in UI. "Work your Way" is the public tagline (lowercase "your").
- **The system has three voices**, mirroring the wordmark: a heavy display sans (Sora), a utility body (Manrope), a hand-painted accent (Permanent Marker — hero only, never UI).
- **The accent is MyGig violet `#6C60FF`** — the brand colour pulled straight from mygig.com.au. Used confidently on primary CTAs, key brand moments, info chips, and selection states. White text reads cleanly on top.
- **The "stamp" motif** — violet fill + 3px ink border + hard 4px offset shadow — is the heaviest visual moment. Used for the primary CTA, hero badges, and the EOR compliance callout. Once per screen, max.
- **Backgrounds are warm paper (`#FAF8F4`)**, not cool grey. Cards sit in pure white on top.
- **Never use pure `#000`** — the brand black is `#0E0D0B`.

## Files in this skill
| Path | What it is |
|---|---|
| `README.md` | The full strategy document — voice, visual foundations, iconography, every token. Read this first. |
| `colors_and_type.css` | Drop-in stylesheet with every design token and semantic classes (`.mg-display`, `.mg-h1`, `.mg-card`, etc.) |
| `assets/` | Logos in three forms. |
| `preview/` | Standalone HTML cards for each token cluster — use as a reference. |
| `ui_kits/marketing/` | Marketing site recreation. |
| `ui_kits/business/` | Business dashboard recreation (with Amy AI). |
| `ui_kits/business-mobile/` | Business mobile app — 4 manager screens (dashboard, post a shift, on their way, Amy). |
| `ui_kits/worker/` | Worker mobile app recreation (4 screens). |
| `ui_kits/jobboard/` | Casual Job Board — interactive UI kit (5 screens + apply flow). Open `JobBoard.dc.html`. |

## Working pattern
When building anything for MyGig, **always** link `colors_and_type.css` first. Then pull markup patterns from the closest UI kit. The kits are designed to be cannibalised — copy a card, a pill, a worker chip, the stamp CTA, and adapt.
