# MyGig Design System

> Work your Way.

This is the design system for **MyGig** — Australia's AI-powered Workforce‑as‑a‑Service platform and Employer of Record (EOR). The system is built to serve two very different audiences from a single, coherent brand:

1. **Businesses** — managers and HR teams who post shifts, manage casual workforces, and need to feel that compliance, payroll, and award interpretation are handled.
2. **Workers** — casuals, students, backpackers, and tradies who pick up shifts on their phone, clock in, get paid, and build a profile.

The brand also speaks publicly through a **marketing site** (mygig.com.au) targeting both audiences.

---

## Sources used to build this system

| Source | Where | Notes |
|---|---|---|
| Marketing site | https://www.mygig.com.au/ | Voice, product positioning, EOR/compliance language |
| Worker site | https://www.mygig.com.au/worker | Worker-side value props |
| Business site | https://www.mygig.com.au/business | Business-side value props, "Pool", fill-rate stats |
| Knowledge base | https://help.mygig.com.au/ | Product detail (30 data points, vetting, etc.) |
| Mobile app (worker) | https://play.google.com/store/apps/details?id=au.com.mygig.app | Feature list — "Amy" AI assistant, Wallet, MyGig Training, in-app support |
| Logo files | `uploads/` (copied into `assets/`) | Wordmark, lockup, mark — black + white |
| Figma files | _Pending — user will share later_ | Will reconcile this system with Figma when received |

> ⚠️ **Open items.** This is a v1 system built from logos + marketing copy + product positioning. The user has indicated Figma files will follow. When they arrive we will reconcile colors, type, components, and spacing against the source of truth — anything in this document marked _"v1 inference"_ is a candidate for change.

---

## CONTENT FUNDAMENTALS

### Voice in one sentence
**Plain-spoken, confident, Aussie-flavoured. We talk like a competent operations manager who genuinely respects the worker on the floor.**

We are not corporate HR-speak. We are not Silicon-Valley breezy. We are direct, useful, and a little bit cheeky.

### Audience-shaped tone

| Surface | Tone | Why |
|---|---|---|
| Marketing — Business | **Confident, evidence-led.** Numbers, compliance, time saved. | Decision makers want proof. |
| Marketing — Worker | **Empowering, freedom-first.** "Work Your Way", flexibility, pay-on-time. | Workers want agency. |
| Business app | **Operational, calm.** Short labels, clear states, no jargon. | They're at work, not browsing. |
| Worker app | **Friendly, motivating.** Earnings highlighted, achievements celebrated. | Repeat engagement matters. |
| Knowledge base / compliance | **Plain English regulatory.** Reads like a Fair Work explainer. | Stakes are real. |

### Voice rules

- **Use "you" and "we"**. Never "users" or "the worker". You is whoever is reading.
- **Active voice, present tense**. _"Post a shift in 60 seconds"_, not _"Shifts can be posted in 60 seconds"_.
- **Concrete > clever**. _"90%+ fill rate"_ beats _"unmatched reliability"_. Numbers are the brand's superpower; use them.
- **Aussie English spellings**. _Authorised_, _organisation_, _vetted_, _favourite_. Not _authorized_.
- **Acronyms are explained once, then used freely**. EOR, WHS, NES, WAS. We don't water these down — our audience knows them.
- **Use sentence case for UI labels and buttons**. Not Title Case, not ALL CAPS. _"Post a shift"_, not _"Post A Shift"_. (Exceptions: the wordmark, the eyebrow micro-labels which are uppercase by design.)
- **Don't apologise for being a platform**. We're not "just an app", we're an Employer of Record. Lean into the heavyweight stuff.
- **Money is shown in AUD, in full**. _"$31.19/hr"_ — never _"$31"_, never _"AUD 31.19"_. The cents matter to a worker.
- **Time is local, 12-hour with am/pm lowercase**. _"6:30am – 2:00pm"_.

### Voice examples (real and inferred from the site)

| ✅ Do | ❌ Don't |
|---|---|
| "Post a shift in under 60 seconds." | "Streamline your workforce procurement journey." |
| "No interviews needed." | "Eliminate the candidate evaluation overhead." |
| "We're the Employer of Record — we take the legal weight, you get the workers." | "We provide an EOR layer." |
| "Top workers get first dibs on shifts." | "Premium-tier operatives receive prioritised shift allocation." |
| "Get paid the day after your shift." | "Optimised payout cadences." |
| "Your hours are tracked automatically — no guesswork, no disputes." | "Eliminate ambiguity in workforce time-keeping." |

### Numbers we lean on

- **90%+** fill rate (industry average is 65%)
- **2%** no-show rate
- **30+** data points verified per worker
- **$31.19/hr** national minimum
- States MyGig is an authorised EOR in: **NSW, WA, TAS, NT** (QLD, VIC, SA, ACT pending — _always state this honestly_)

### Tagline use

> **"Work your Way"** is the public-facing tagline. Always lowercase "your".
> It belongs on hero shots, the worker app splash, and the campaign-level layouts — **not** as a button label or in product chrome.

### Emoji

**Used very sparingly, and never in business-facing UI.**
- ✅ Acceptable in the worker app, in places like push notification copy, an empty-state cheer, or a streak achievement.
- ❌ Never in business dashboards, marketing pages, compliance/legal text, or buttons.
- Approved set: 👋 🎉 ⚡ ✅ ⭐ 💪 (used to celebrate, not to decorate)

---

## VISUAL FOUNDATIONS

### The big idea
The MyGig wordmark sets the whole system: a **hand-painted "my"** sitting next to a **bold geometric "Gig"**. That's the brand — human grit meets confident systems. Every visual decision should land somewhere on that spectrum.

### Colors — three commitments

The full token set lives in [`colors_and_type.css`](./colors_and_type.css). The TL;DR:

| Family | Token | Hex | Role |
|---|---|---|---|
| **INK** (off-black neutrals) | `--ink-900` | `#0E0D0B` | Primary surface, type, brand. The wordmark black. Never use pure `#000`. |
| | `--ink-500` | `#3D3A33` | Body text on paper |
| | `--ink-400` | `#6F6A60` | Secondary text |
| | `--ink-100` | `#E5E1D7` | Dividers, input borders |
| | `--ink-0`   | `#FAF8F4` | App background — warm "paper", not cool grey |
| **BRAND** (signature violet) | `--brand-500` | `#6C60FF` | MyGig's signature brand colour. Pulled from mygig.com.au. Primary CTAs, selection, key brand moments. White text reads cleanly on top. |
| | `--brand-100` | `#E8E6F9` | Info chips, badge backgrounds, the "Available in NSW, WA, TAS and NT" style pill (from mygig.com.au). |
| | `--brand-200` | `#DBD8FA` | Secondary fill, illustrations (from mygig.com.au). |
| | `--brand-700` | `#4B3FD9` | Pressed / active state. |
| **PAPER** (pure white surfaces) | `--surface-0` | `#FFFFFF` | Cards and modals on top of the warm app bg |

**Semantic colors** (`--success-500`, `--warn-500`, `--danger-500`, `--info-500`) are deliberately less saturated than the brand violet so they don't fight for attention. The brand colour carries weight; semantics are utility.

**Industry tag tints** (`--tag-hospo`, `--tag-events`, etc.) are pastel washes used _only_ for shift category chips. Never as chrome or background.

### Type — three voices

| Voice | Family | Where |
|---|---|---|
| **Display** (the "Gig" voice) | **Sora** 700/800 | Headlines, big numbers, hero. Heavy, geometric, slightly humanist — a strong companion to the wordmark's "Gig". |
| **Body** (utility) | **Manrope** 400/500/600/700 | Paragraphs, UI, forms, data. Open and legible at small sizes. |
| **Script** (the "my" voice) | **Permanent Marker** | A hand-painted nod to the brushed "my". Pull-quotes, hero callouts, easter eggs only. Never UI. |
| **Mono** | **JetBrains Mono** | Timestamps, shift IDs, payslip line items |

> **Font stack is official.** All four families are free and open-source (Google Fonts / SIL OFL), so they ship without licensing friction across web, app, and print. Loaded from `fonts.googleapis.com` at the top of `colors_and_type.css` — no install required, no missing-font fallbacks in production.

### Spacing — 4pt grid
Everything snaps to a 4px scale. Tokens `--sp-1` through `--sp-24`. Standard card padding is `--sp-6` (24px); section spacing is `--sp-16` (64px).

### Radii
- `--r-md: 12px` is the default. Cards, inputs, buttons.
- `--r-pill: 999px` for status pills, category chips, segmented controls. We use pills _a lot_ — they're a signature.
- `--r-xl: 28px` for mobile bottom sheets and hero cards.
- Never zero radius. We are not a brutalist brand.

### Shadows + elevation
Inky and subtle (`--sh-1` → `--sh-4`). We don't tint shadows blue or purple.

**Brand exception — the "stamp" shadow.** A hard offset black drop (`--sh-stamp: 4px 4px 0 var(--ink-900)`) used deliberately on:
- The primary CTA button on marketing pages (paired with a 3px black border)
- "On the job" stamps in empty states and confirmations
- Hero badges
It's a deliberate motif — feels like a job site sign / parking permit. Use it as a brand moment, not everywhere.

### Borders
- `--bw-hair: 1px` for dividers and standard cards
- `--bw-rule: 1.5px` for inputs at rest
- `--bw-heavy: 2px` for selected states
- `--bw-stamp: 3px` for the stamp motif only

### Backgrounds
The base is **warm paper** (`#FAF8F4`), not cool grey. Cards sit on top of this in pure white. This warm/cool contrast is intentional — it gives every screen a tiny bit of the analog "timesheet" feeling.

We **do not** use:
- Gradient backgrounds (no purple-to-blue washes — gig platforms over-use these)
- Glass / blur effects in product UI (rare exceptions in the worker app camera screens)
- Full-bleed stock photos behind text (we use real worker photography — see Imagery)

We **do** use:
- Solid black hero sections on marketing pages with violet accents
- A subtle paper-texture overlay on hero blocks (optional, very low opacity)
- The brush-stroke graphic from the logo as a divider or section opener

### Imagery
**Real workers. Real worksites. Documentary-feeling.** Imagery is the most important non-typographic carrier of the brand — it tells the trust story that the copy keeps repeating. The full rulebook with crops, shapes, treatments, and do/don'ts lives in the **Imagery — The MyGig look** preview card. The summary:

- **Subject** — workers mid-task. Eyes on the work, not the camera. Aprons, hard hats, hi-vis, forklifts, espresso bars, retail floors, event gates.
- **Light** — natural, warm. Golden hour, daylight through windows, kitchen tungsten. Never cold blue tech lighting.
- **Mood** — documentary, not staged. Saturation 0.85–1.0. Subtle grain ok. No filters.
- **Aspect ratios** — `4:5` for marketing heroes and worker chips, `3:4` for portraits, `1:1` for avatars and social, `16:9` for video posters and banners.
- **Corners** — default `12px` (`--r-md`), `28px` (`--r-xl`) for hero cards and mobile sheets, full circle for avatars only.
- **Treatments** — natural by default (use this 90% of the time). Brand-violet `18% multiply` overlay reserved for section dividers/story breaks. Stamp border (`2px ink + 6px ink offset shadow`) for marketing hero stacks only.
- **The hero stack** — the signature marketing composition: three photo-cards rotated at `+3°`, `−2°`, and straight. Always include at least one ink-900 card in the mix; never three light cards in a row.
- **Diversity** — represent Australia's casual workforce honestly. Age, gender, ethnicity — all real, all on the floor.

> **We do not generate fake AI worker photography.** If real photography isn't available for a layout, use a solid ink-900 block at the intended dimensions with a brand-300 corner label naming the planned shot (e.g. "Sarah, espresso pull, Single O Surry Hills"). This is the only sanctioned placeholder — see the Imagery preview card for the exact treatment.

### Avatars
Worker avatars follow a single rule: **use the worker's profile photo when we have it; otherwise initials on a coloured background.** Both variants share the circular crop and a `1.5px` ink border. The coloured background for initials is randomly assigned from the **industry tag tints** so it stays on-system. See the Worker chip preview card for the exact pattern.

### Hover, press, focus, disabled

| State | Treatment |
|---|---|
| **Hover** (mouse) | Background shifts one step darker on its scale (e.g. `--ink-50` → `--ink-100`). Buttons darken by ~6%. Lift by `1px` translate on stamp-style CTAs. |
| **Press / active** | Translate `2px, 2px` on stamp CTAs (shadow effectively disappears — feels like pressing a real button down). Other elements: background `--brand-700` for brand fills, `--ink-700` for ink. |
| **Focus (keyboard)** | 2px brand-violet outline at `2px` offset, never default blue. `outline: 2px solid var(--brand-500); outline-offset: 2px;` |
| **Disabled** | `opacity: 0.45`. No grey fill. We don't pretend it's clickable. |
| **Loading** | Pulsing shimmer on a 1.2s loop, ink-50 → ink-100. No spinners except on the worker mobile pull-to-refresh. |

### Animation
- Default duration: `200ms`, easing `cubic-bezier(0.22, 1, 0.36, 1)` (ease-out-quint).
- Slow: `400ms` for full-screen sheet transitions.
- Fast: `120ms` for hover/press feedback.
- **No bouncy/spring animations** in business UI. The worker app can use a subtle spring on accept/earnings reveal — only once a session per moment.
- Page transitions: slide up + fade for mobile bottom sheets; fade only for desktop modals.

### Layout
- **Marketing** max width `1320px`, gutters `48px`.
- **Business app** is a fixed-sidebar layout, content max `1140px` inside a fluid main, gutters `24px`.
- **Worker app** is mobile-first, 16px gutters, 24px on the home feed.

### Transparency + blur
Rarely used. The only sanctioned use is:
- Modal scrim: `rgba(14, 13, 11, 0.55)` (ink-900 at 55%)
- Worker app bottom-sheet handle drag area: 8px blur at 60% opacity
No frosted-glass nav bars.

### Iconography preview
See the **ICONOGRAPHY** section below — short answer: **Lucide**, stroke-only, 1.75–2px weight, mostly `--ink-700` on light.

---

## ICONOGRAPHY

### Library
We use **[Lucide](https://lucide.dev)** as the icon library — open source, stroke-based, comprehensive coverage of workforce/calendar/payment concepts we need (`Calendar`, `Clock`, `MapPin`, `Wallet`, `ShieldCheck`, `Briefcase`, `Star`).

Loaded from CDN: `https://unpkg.com/lucide-static@latest/font/lucide.css` or via React's `lucide-react` package. See `ui_kits/*/index.html` for the standard loader.

### Rules

- **Stroke weight**: `1.75–2px` — Lucide's default. Never solid/filled icons in product chrome (the only exceptions are filled status icons like the success checkmark in a paid-shift toast).
- **Sizing**: `16px`, `20px`, `24px`. Inline-text icons are `1em`.
- **Color**: `--ink-700` for primary, `--ink-400` for secondary/decoration, `--brand-700` when emphasising the active item in nav.
- **Alignment**: icons in buttons go on the **left**, with `8px` gap. Right-side icons are reserved for "leads onward" (`ChevronRight`, `ExternalLink`).
- **Never** rotate or skew icons for effect.

### Emoji
See CONTENT FUNDAMENTALS — emoji is **off** in business UI, used sparingly in worker app and never as core navigation. Use the icon library instead.

### Logo files
In `assets/`:

| File | Use |
|---|---|
| `logo-wordmark-black.png` | Light backgrounds. The horizontal lockup with "my Gig™". |
| `logo-wordmark-white.png` | Dark backgrounds. |
| `logo-mark-black.png` | Square avatar / app icon — full lockup on rounded black tile. |
| `logo-mark-white.svg` (TBD) | _Pending — please supply SVG masters when available._ |

**Clear space.** The wordmark needs clear space equal to the cap-height of "G" on all sides. Don't crowd it.

**Don't** stretch, recolour outside the approved palette, drop-shadow, or place on busy photographic backgrounds without a solid block behind it.

---

## AMY — the AI assistant

**Amy is MyGig's AI assistant.** She sits inside the Business platform and handles workforce work end-to-end: posting shifts, finding workers, checking awards, surfacing problems before they happen.

### Where Amy lives
| Surface | Treatment |
|---|---|
| **Topbar** | An "Ask Amy ⌘K" pill chip — always visible, keyboard-shortcutable. |
| **Proactive banner** | Above the dashboard KPIs. Amy raises flags ("Thu shift unfilled, want me to invite 3 top workers?") with one-click accept. |
| **Right drawer** | A dedicated 360px column docked to the right of the dashboard. Conversation flow, draft artifacts (shift cards, worker lists), composer. |
| **Inside flows** | "Post or ask Amy" replaces standalone "+ Post a shift" — natural-language input feeds the shift composer. |

### Amy's visual identity
- **The Amy mark** — a small purple radial-gradient orb with "Aa" inside. Three sizes (`sm 18`, `md 24`, `lg 32`). Use this anywhere Amy "speaks" — never a stock robot icon, never a human-style avatar.
- **The spark glyph (`✦`)** — Amy's signature glyph. Use it as a bullet in front of Amy-generated suggestions, draft artifacts, and proactive labels.
- **Brand-300 type on dark** for Amy-labelled headings (e.g. "AMY · NOTICED SOMETHING") so she reads as "AI, helpful" rather than competing with semantic colours.

### Amy's voice
She's the same brand voice — plain-spoken Aussie, evidence-led, sentence case — but a touch warmer because she's conversational.

- **Open with action.** _"Done. I drafted this."_ not _"I have processed your request."_
- **Show, don't tell.** When she proposes something, she generates an artifact (mini shift card, ranked worker list) inside her bubble — never a wall of text.
- **One-click out.** Every Amy response that can lead to action has a primary CTA (e.g. _"Post & invite all 3"_) and a ghost _"Edit"_.
- **Always cite the basis.** _"Follows the Hospitality Award L2."_ Compliance is the product; show your work.
- **Never apologise.** _"I couldn't find a barista within 5km — want me to widen to 10km?"_ — solutions, not regrets.

### When NOT to use Amy
- Compliance attestations (always human-confirmed).
- Cancellations / no-show resolutions (always human-approved).
- Anything the user explicitly asks to do manually.

Amy proposes, the user disposes. The system never auto-acts without an explicit confirm.

| Path | Purpose |
|---|---|
| `README.md` | This file. The strategy + foundations document. |
| `SKILL.md` | Cross-compatible skill manifest so this works as a Claude Code skill. |
| `colors_and_type.css` | The single source of truth for design tokens. Import this in every file. |
| `assets/` | Logos, brand marks. (Photography pending.) |
| `preview/` | Small HTML cards rendered in the Design System tab — color swatches, type specimens, components in isolation. |
| `ui_kits/marketing/` | Marketing site recreation — hero, value props, CTA. |
| `ui_kits/business/` | Business platform — dashboard, post-a-shift, workforce, Amy AI. |
| `ui_kits/business-mobile/` | Business **mobile** app — manager on the go: dashboard, post a shift, on-their-way tracking, Amy chat. |
| `ui_kits/worker/` | Worker mobile app — feed, shift detail, wallet, profile. |
| `ui_kits/jobboard/` | **Casual Job Board** — a fully-interactive UI kit (landing, browse + filters, job detail, list-a-job, mobile, apply flow). Built as a Design Component on these tokens. Open `JobBoard.dc.html`. |

---

## A note on this v1

This system was assembled from the public website, the wordmark, and a strong reading of MyGig's positioning. Real source materials (Figma, brand book, existing component library) will refine every layer of it — most likely the **font family**, the **exact hi-vis hex**, and the **icon set**. Treat this document as a confident first principle, not a final spec.
