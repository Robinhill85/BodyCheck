# BodyCheck — Brand Kit

Extracted from the live site source (`03-creatives/pitch-site/index.html` and its CSS), not from a visual guess. Every value below is traced to a declaration in the code.

> Not a medical device. Routing, not diagnosis.

## 1. Colours

| Hex | Name | Where it is used |
|---|---|---|
| `#0D1117` | Base background | Page background (`bg-[#0D1117]`), nav bar, dark section backgrounds, hero gradient target |
| `#13181F` | Surface / card | Stat cards, how-it-works cards, table header row, equity cards (`bg-[#13181F]`) |
| `#00E5C3` | Brand teal (accent) | Logo icon, ECG waveform, primary button fill, eyebrow labels, links, "YOU ARE HERE" tag, all positive checkmarks |
| `#FFFFFF` | White (text) | Primary text, headings; used at many opacities (see note) |
| `#F87171` | Action-needed red (Tailwind `red-400`) | The only state colour hard-coded in the live UI: Action Needed pill, dot, and selected row (`text-red-400`, `bg-red-400/10`, `border-red-400/40`) |

White is used through opacity tiers rather than separate hexes: `white/90` and `/80` (strong text), `/65`, `/60`, `/55`, `/50` (body), `/40`, `/35`, `/30`, `/25`, `/20` (muted/labels), `/8` and `/5` (borders, hairlines).

### Near-duplicates to collapse
- `#0D1117` (base) and `#13181F` (card) are both very dark blue-black and read as one "near-black" family. They are intentionally distinct (page vs. raised surface). Keep both, but do not introduce a third dark in between.
- The many `white/xx` opacities collapse to roughly three roles: text (`/90`–`/55`), muted (`/40`–`/20`), hairline (`/8`–`/5`).

### Flag: not BodyCheck colours
The saved page also contains the Manus editor chrome design tokens (e.g. `--text-brand: #0081f2`, `--logo-color: #34322d`, `#f8f8f7`). These belong to the Manus platform UI, **not** the BodyCheck brand. Ignore them when building creatives.

### Five states
Only **Action Needed** has a dedicated colour in the live UI (`red-400 / #F87171`). Stable, Watch, Elevated Risk, and Recovery render with neutral `white/20` dots in the state selector. The conceptual green to amber to orange to red to teal ramp exists only in the state-visual artwork and the Fotor prompts, not in the CSS. Lock any per-state palette on the canvas; do not claim it is in the product yet (TODO).

## 2. Fonts (in declaration order)

- **Headings, wordmark, and stat numbers:** `"Space Grotesk", sans-serif` (set inline on every `h1`/`h2`/`h3`, the wordmark, and the big stat figures).
- **Body and paragraphs:** the Tailwind default sans stack: `ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif`.
- **Labels / eyebrows / version tags:** a `mono` utility class (monospace) for the small uppercase tracked labels.

### Fotor substitution note
Space Grotesk may not be available in Fotor. Closest common substitutes, in order: **Sora**, then **Montserrat**, then **Poppins** (all geometric sans with a similar wide, modern feel). For the mono labels, use **Space Mono**, **Roboto Mono**, or **IBM Plex Mono**.

## 3. Wordmark

Built from two parts, no custom logotype:
- **Icon:** Lucide `heart-pulse` SVG (a heart with an ECG line through it), `stroke-width: 2`, stroke colour `#00E5C3`, 20x20 in the nav.
- **Text:** "BodyCheck" in `Space Grotesk`, `font-bold`, white.
- **Optional tag:** a mono caption "v0.1 · VibeHack 2026" in `#00E5C3` at 60% opacity beside the wordmark.

Local logo files already exported in `03-creatives/brand-logos/`: `bodycheck-icon.svg/png`, `bodycheck-logo-primary.png`, `bodycheck-logo-inverse.png`, `bodycheck-ecg-motif.svg/png`.

## 4. Motif

A recurring **ECG / heartbeat waveform** in brand teal:
- SVG `path`, `viewBox="0 0 200 100"`, `preserveAspectRatio="none"`, `stroke="#00E5C3"`.
- Drawn twice: a sharp line at `stroke-width: 1.5`, `opacity: 0.9`, over a soft duplicate at `stroke-width: 4`, `opacity: 0.15`, `filter: blur(3px)` to create the glow.
- Animated horizontally via a `waveform-track` element in the hero lower third.
- Supporting motion utilities: `teal-glow` (glow on the primary button) and `pulse-dot` (pulsing dot on state pills).

The motif doubles as the logo icon (heart-pulse) and the section divider, which is what ties the identity together: one teal line, read as a heartbeat.
