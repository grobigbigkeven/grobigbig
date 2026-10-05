# Gro Big Big — Design System

The brand and component system for **Gro Big Big**, a holding company for business
services. The house sits behind two operating brands — **AccPro** (cloud accounting
& advisory) and **grof** (corporate services for founders) — and exists to hold one
standard across both.

> The name is deliberate. *Grow big big* is how a Singaporean tells you to aim higher
> without the corporate theatre — ambition and warmth in the same breath. The brand is
> that idea made calm: big intentions, run quietly.

## Sources
- `Gro Big Big Brand.dc.html` — the original brand-guide microsite this system was lifted from.
- `uploads/` — grof brand-guideline screenshots & colour references (Montserrat / Hind Vadodara, navy + orange).
- `assets/` — supplied AccPro and grof logo files (full-colour, white, reversed).

---

## Content fundamentals
**Voice: big ambition, said plainly.**
- **Lead with the work**, not the group's size or history. Credentials come last, if at all.
- **Warm, not loud.** The name has a wink; copy can too — but confidence is quiet. No hype, no superlatives.
- **Back it with numbers.** Every claim earns its place with something verifiable.
- **Person:** addresses the reader as *you* / *businesses*; the group is *the house* or *we*.
- **Casing:** sentence case everywhere except the amber **eyebrow**, which is UPPERCASE with wide tracking. Brand name is always "Gro Big Big"; "grof" is always lowercase; "AccPro" keeps its camel cap.
- **No emoji.** Punctuation is plain; em-dashes and mid-dots (·) carry rhythm.
- **We say:** grow · the house · operating brands · standard · trusted · clarity. *"Grow big big — run calm."*
- **We avoid:** synergy · best-in-class · world-class · empower · leverage · seamless · ecosystem.

---

## Visual foundations
- **Colour.** House primary is **Pine Green `#173E3D`** — deliberately halfway between AccPro's forest and grof's navy. The accent is **Amber `#E0913A`**, halfway between AccPro's gold and grof's orange. The house reads as the calm middle that holds both. Backgrounds are a warm paper **Canvas `#F5F4F0`** and **White**; text is a warm-cool near-black ink `#1C2128`. Chroma is kept very low on every neutral.
- **Typography.** One geometric sans for the house: **Plus Jakarta Sans** (400/500/600/700). Tight display tracking (down to −2.6px on the hero), generous body leading (1.65). Operating brands keep their own faces in their own contexts (grof: Montserrat + Hind Vadodara).
- **The eyebrow.** Signature device: a 32×2 amber tick + uppercase amber label above most headings. Only uppercase element in the system.
- **Backgrounds.** Pine and dark grounds carry a faint 64px white grid texture. No photographic hero, no gradients, no illustration in the house brand (sub-brands may differ).
- **Cards.** White on canvas, 1px `#D9DDD8` hairline border, 12px radius. Mostly flat; the focal card lifts with a **pine-tinted** shadow (never neutral grey). An operating brand is signalled with a 3px coloured top accent bar.
- **Spacing & layout.** 8px base rhythm; sections breathe at **104px**; content caps at a **1080px** container with 48px gutters.
- **Radius.** 8px (controls), 12px (cards), 14px (panels), pill for tags.
- **Motion.** Calm — 120–320ms, standard easing, no bounce. Hover shifts colour/border only; focus shows an amber ring (`0 0 0 3px rgba(224,145,58,0.28)`).
- **Shadows.** Always pine-tinted alpha, three steps (sm/md/lg).

---

## Iconography
Line-based, **rounded-geometric, 2px stroke**, legible at small sizes (per the supplied
icon-direction sheet: Accounting, Inventory, Payroll, CRM, POS, Banking…). The system
uses **[Lucide](https://lucide.dev)** via CDN as the closest match to that direction —
*flag:* substitute the brand's own icon set when it's delivered. Emoji are never used.
The logo **mark** (three rising bars — two brand roots climbing to one amber peak) is the
only bespoke vector; it ships as `assets/gbb-mark.svg` / `gbb-mark-reversed.svg`.

---

## Index / manifest
**Root**
- `styles.css` — global entry point (consumers link this; `@import`s everything below).
- `tokens/` — `colors.css`, `typography.css`, `spacing.css`, `effects.css`, `fonts.css`.
- `fonts/` — Plus Jakarta Sans (variable, roman + italic).
- `assets/` — logo marks (`gbb-mark*.svg`), AccPro & grof logos (colour / white / reversed), grof mark & icon.

**Components** (`components/core/`, namespace via `_ds_bundle.js`)
- `BrandMark`, `Eyebrow`, `Button`, `Tag`, `Card`, `Input`, `Stat`. Card: `core.card.html`.

**Foundations** (`guidelines/` — Design System tab cards)
- Colors: primary, neutrals, operating brands · Type: scale, weights, eyebrow ·
  Spacing: scale, radius & elevation · Brand: logo, architecture, iconography, voice.

**Slides** (`slides/`) — `title`, `section`, `content`, `statement` (1280×720).

**UI kits** (`ui_kits/`)
- `holding-site/` — the Gro Big Big marketing homepage, composed from core components.

**Templates** (`templates/` — starting points consuming projects can copy)
- `homepage/` — the holding-company marketing homepage (`Homepage.dc.html`), editable markup built from the core components.
- `deck/` — a 4-type slide deck (`Deck.dc.html`): title · section · content · statement, on the shared deck stage.

---

## Caveats
- **Icons** are Lucide (CDN) standing in for the brand's own line set — swap when delivered.
- The house system ships one typeface, **Plus Jakarta Sans**. The operating sub-brands
  (AccPro, grof) keep their own faces inside their own products — not part of this house system.
- Logos are the supplied raster PNGs; drop in official vectors when available.
