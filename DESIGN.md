---
name: Guane docs
description: Documentation and tutorials for Guane, a local R/Shiny app for phylogenetic comparative methods.
colors:
  app-teal: "#0d5368"
  forest-green: "#2f7d4f"
  forest-deep: "#1f5135"
  link-green: "#1c6a44"
  bark: "#6b4f2a"
  ink: "#1d2b2f"
  lichen-muted: "#4a5a5e"
  paper: "#ffffff"
  moss-surface: "#f6f8f5"
  sand: "#f4f1ea"
  sand-line: "#cbb994"
  hairline: "#d5ddd8"
  frame-grey: "#7a8a85"
  code-bg: "#f1f4f0"
  code-inline: "#6b3a1f"
  table-head-bg: "#e4eee7"
  chip-bg: "#e3eef1"
  chip-ink: "#0d3f4f"
  chip-line: "#5f8a97"
  mist: "#cfe6ec"
  focus-ember: "#b35c00"
  focus-gold: "#ffd166"
  caution-amber: "#9a5b00"
  important-red: "#a42828"
typography:
  display:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "clamp(2.1rem, 1.5rem + 2vw, 2.75rem)"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "1.85rem"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.01em"
  title:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "1.35rem"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.01em"
  title-sm:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 600
    lineHeight: 1.35
  body:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
  lead:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "1.1rem"
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 700
    letterSpacing: "0.06em"
  ui-chip:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif"
    fontSize: "0.92em"
    fontWeight: 600
  mono:
    fontFamily: "ui-monospace, SFMono-Regular, Menlo, Consolas, Liberation Mono, monospace"
rounded:
  chip: "0.3rem"
  frame: "0.5rem"
  card: "0.6rem"
  hero: "0.75rem"
  marker: "50%"
spacing:
  row: "0.6rem"
  gap: "1rem"
  inset: "1.25rem"
  block: "1.75rem"
  section: "2rem"
  heading: "3rem"
  measure: "55ch"
components:
  button-hero-primary:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.forest-deep}"
  button-hero-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.paper}"
  ui-chip:
    backgroundColor: "{colors.chip-bg}"
    textColor: "{colors.chip-ink}"
    typography: "{typography.ui-chip}"
    rounded: "{rounded.chip}"
    padding: "0.05em 0.45em"
  module-card:
    backgroundColor: "{colors.moss-surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "1.1rem 1.1rem 0.9rem"
  control-card:
    backgroundColor: "{colors.moss-surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "1rem 1.25rem 1.1rem"
  control-card-title:
    backgroundColor: "{colors.chip-bg}"
    textColor: "{colors.chip-ink}"
    rounded: "{rounded.chip}"
    padding: "0.15em 0.55em"
  meta-box:
    backgroundColor: "{colors.sand}"
    textColor: "{colors.ink}"
    rounded: "{rounded.frame}"
    padding: "0.85rem 1.25rem"
  recipe:
    backgroundColor: "transparent"
    rounded: "{rounded.card}"
    padding: "1.1rem 1.25rem 0.4rem"
  step-marker:
    backgroundColor: "{colors.forest-green}"
    textColor: "{colors.paper}"
    rounded: "{rounded.marker}"
    size: "1.9rem"
  navbar:
    backgroundColor: "{colors.app-teal}"
    textColor: "{colors.paper}"
  table-head:
    backgroundColor: "{colors.table-head-bg}"
    textColor: "{colors.forest-deep}"
  hero:
    textColor: "{colors.paper}"
    rounded: "{rounded.hero}"
    padding: "2rem 1.5rem"
---

# Design System: Guane docs

## Overview

**Creative North Star: "The Field Station Manual"**

The docs site is the Guane app's field manual: it wears the app's own teal navbar and forest greens so a researcher moving between app and page never changes worlds, then sets everything else on quiet paper so screenshots and real interface labels carry the teaching. It descends from the Shiny app's identity (teal `#0d5368` navbar, forest greens, a bark accent) but is its own surface, a Quarto theme layered on Bootstrap flatly (light) and darkly (dark). The app's own stylesheet is not part of this system.

Density is reading density: a 17px system-ui body at 1.6 leading, prose held to a 55ch measure (about 72 real characters), and reference frames (cards, callouts, figures, tables) spanning the full content column. Colour means something: green is the modules and progress, teal is the app's own controls, bark marks tutorial metadata labels. Depth is almost absent; boxes are defined by 1px frames and tonal fills, never by side stripes.

Every state is legible without colour: body links are underlined, the current nav item is bold and underlined, focus is a 3px ring. The system meets WCAG 2.2 AA in both themes.

**Key Characteristics:**
- App lineage: teal navbar, forest-green hero gradient, bark labels.
- Paper page, 1px frames, tonal fills; flat at rest.
- Prose at the measure, frames at the column.
- Interface names always appear as teal label chips, exactly as the app writes them.
- Light and dark themes share every component rule; dark only overrides tokens.

## Colors

A forest-and-teal palette from the app, cut with one warm bark note, on white paper.

### Primary
- **App Teal** (app-teal): the navbar ground, link hover, note callout frame. The single strongest carry-over from the app.
- **Forest Green** (forest-green): step markers, tip callout frame, the 1px rule under every page title, the light end of the hero gradient, form `accent-color`.
- **Forest Deep** (forest-deep): the dark end of the hero gradient, table header text, the navbar's 1px bottom border, hero primary button text.
- **Link Green** (link-green): body links (always underlined), card title links, text caret.

### Secondary
- **Chip Teal** (chip-bg / chip-ink / chip-line): the `.ui` interface-label chip and the control card's frame and title chip. Reserved for names of things in the app.
- **Mist** (mist): navbar hover text and `::selection` background.

### Tertiary
- **Bark** (bark): small uppercase field labels in the meta box and the control card rows. The SCSS token is named `$guane-eyebrow` for historical reasons; its only live use is these field labels.
- **Sand** (sand, sand-line): the tutorial meta box fill and its 1px frame.
- **Code Inline Brown** (code-inline): inline `code` text.

### Neutral
- **Ink** (ink): body text and headings.
- **Lichen Muted** (lichen-muted): page descriptions, figure captions, the drawn breadcrumb chevron.
- **Paper** (paper): page background, hero text and buttons.
- **Moss Surface** (moss-surface): module and control card fill.
- **Hairline** (hairline): h2 underline, card frames, dl row dividers, step connector. Decorative only.
- **Frame Grey** (frame-grey): screenshot frame and recipe frame (meets 3:1 as a UI boundary); scrollbar thumb.
- **Code Bg** (code-bg), **Table Head Bg** (table-head-bg): code blocks and table header rows.

### Status and focus
- **Caution Amber** (caution-amber): the "Scientific caution" warning callout frame. **Important Red** (important-red): data-loss callouts.
- **Focus Ember** (focus-ember): 3px focus ring on paper. **Focus Gold** (focus-gold): focus ring on the teal navbar, green hero and lightbox overlay, and on every surface in dark mode.

### Dark theme
Dark overrides tokens only (`theme/guane-dark.scss`): page `#11191b`, ink `#e4ebe7`, muted `#a9b8b4`, link `#7fd4a4` (hover `#9fd9ea`), navbar `#0a3d4d`, hero `#153a27 -> #1f5135`, surface `#1a2427`, sand `#211d15` / line `#4a3f2c`, bark `#d9b27c`, hairline `#33433f`, frame grey `#5d6e6a`, code `#18252a` / inline `#f0c48a`, table head `#1c3327` / `#cde8d6`, chip `#17343d` / `#cfe6ec` / `#4f8797`, forest green and step marker `#5cc088` (marker text `#11191b`), callouts note `#4fb3cf`, tip `#5cc088`, warning `#e0a33a`, important `#ef7b7b`, selection `#245563`, focus `#ffd166`.

### Named Rules
**The Role Colour Rule.** Green belongs to modules and progress, teal to the app's own controls, bark to tutorial metadata labels. A new component picks one role; it does not mix them.

**The Token-Only Dark Rule.** Dark mode is a token override file. A component that needs a dark-only rule is a token that is missing.

## Typography

**Display Font:** system-ui (native stack)
**Body Font:** system-ui (native stack)
**Label/Mono Font:** ui-monospace (SFMono, Menlo, Consolas) for code

**Character:** One native sans at every level, weight and size doing the hierarchy. It renders the lambda, pi and subscripts of the tutorials on every researcher's machine with no download.

### Hierarchy
- **Display** (700, clamp 2.1 to 2.75rem, 1.3, -0.02em): the page title only.
- **Lead** (400, 1.1rem, muted): the one-sentence page description under the title.
- **Headline** (700, 1.85rem, 1.3, -0.01em): h2 sections, 3rem above, 1rem below, grey hairline under.
- **Title** (700, 1.35rem, 1.3): h3; 2.25rem above, 0.6rem below. Card titles drop to 1.15rem; the control card title becomes a 1.1rem/600 chip.
- **Title small** (600, 1.05rem, 1.35): h4.
- **Body** (400, 17px, 1.6): prose capped at 55ch; `text-wrap: pretty` on paragraphs, `balance` on headings; tabular lining numerals in tables.
- **Caption** (400, 0.875rem, 1.45, muted): figure captions, held to the measure, left-aligned.
- **Label** (700, 0.75 to 0.78rem, 0.06em, uppercase, bark): field labels in the meta box and control card rows only.
- **UI chip** (600, 0.92em): interface names inline in prose; 0.82rem inside module-card chip lists.

### Named Rules
**The Native Stack Rule.** No webfonts. The system stack is the face.

**The Prose-at-the-Measure Rule.** `p, ul, ol, dl, blockquote` cap at 55ch everywhere, including inside frames; figures, code, tables and grids take the full column.

**The Caps-Are-Field-Labels Rule.** Uppercase tracking appears only on a field label naming the value beside or below it (You'll learn, Time, Where, Default, Change it when, Check after). Never above a heading.

## Layout

Quarto's docked-sidebar docs layout: fixed teal navbar, left sidebar per section, right "On this page" TOC, one content column. The home page drops the TOC and replaces the visible title with the hero (title stays for screen readers).

Two widths only: prose at the measure (55ch), frames at the column. Module grids use `auto-fit, minmax(min(100%, 20rem), 1fr)` with a 1rem gap (2x2 on desktop, one column on phones). Control grids hold at most two columns and fall to one below about 41rem of column. The meta box and control card use container queries: meta facts go three across (2fr / 0.8fr / 3fr) at 36rem; control rows go label-beside-value (9rem label column) at 34rem.

Vertical rhythm: more space above a heading than below; callouts and screenshots 1.75rem off neighbours; 2rem under the title rule. Breakpoints are Bootstrap's (the hero tightens below 576px; scroll padding grows below 992px). Nothing overflows horizontally at 320 to 375px: long URLs and inline code break, plain `pre` blocks wrap, wide tables scroll inside their own labelled region.

## Elevation & Depth

Flat, tonal and framed. Depth comes from 1px borders and three fills (moss surface, sand, code bg) against paper. Two shadows exist, both soft and neutral.

### Shadow Vocabulary
- **Screenshot lift** (`box-shadow: 0 2px 10px rgba(0,0,0,0.08)`): at rest under framed app screenshots, so a white app window separates from white paper.
- **Card hover** (`box-shadow: 0 4px 14px rgba(0,0,0,0.12)`, 150ms ease): module cards on hover only, confirming the whole card is a link.

### Named Rules
**The Frame-Not-Stripe Rule.** A rounded box carries its role colour through a full 1px frame, a chip or a tinted header row. No coloured side stripe on any box, callouts included.

## Shapes

Softly rounded rectangles on one ladder: chips 0.3rem, frames (callouts, code, screenshots, meta box) 0.5rem, cards and recipe 0.6rem, hero 0.75rem. Step markers are circles joined by a 2px hairline connector. Borders are always 1px, except the 2px hero buttons and the 3px focus ring. The breadcrumb chevron between chips is drawn from two borders, not a glyph.

## Components

### Buttons
Only in the home hero, two at most.
- **Primary:** paper fill, forest-deep text, 2px paper border, weight 600; hover fill `#e3f1e8`.
- **Secondary:** transparent, paper text and 2px paper border; hover `rgba(255,255,255,0.12)`.
- **Focus:** 3px focus-gold ring, 2px offset.

### Chips (`.ui` interface label)
- **Style:** chip-bg fill, chip-ink text, 1px chip-line frame, 0.3rem radius, weight 600. Wrapped chips clone their frame per line.
- **Use:** exact names of app buttons, tabs, cards, inputs and options. In a breadcrumb (`.guane-path`) chips are joined by a drawn chevron announced as "then".

### Cards / Containers
- **Module card:** moss surface, 1px hairline, 0.6rem radius; one link (the h3 title in link green) stretched over the whole card; hover lift; focus ring on the whole card. On the advanced overview a card also carries a wrap of 3 or 4 non-link flagship chips.
- **Control card (signature):** moss surface, 1px chip-line frame, 0.6rem radius. The h3 is styled as the app's label chip. Four definition rows in fixed order (Where, Default, Change it when, Check after), bark caps labels, hairline between rows; stacked below 34rem, two-column above.
- **Meta box:** sand fill, 1px sand-line frame, 0.5rem radius; three bark-labelled facts (You'll learn, Time, Prerequisites).
- **Worked recipe:** no fill, 1px frame-grey frame, 0.6rem radius, heading starting "Worked example:", wraps a step list so the green markers carry the colour.
- **Callouts:** Quarto built-ins with a 1px frame in the status colour, 0.5rem radius, full-opacity tinted header row, 0.55rem/1rem header and 0.75rem/1rem body inset. "Scientific caution" is always a warning callout.

### Step list
Numbered forest-green circles (1.9rem, bold 0.95rem numerals) at the left, a 2px hairline connector between steps, 2.75rem text inset. One action per step.

### Screenshots
App screenshots framed with 1px frame grey, 0.5rem radius and the screenshot lift, up to 960px wide and aligned to the text edge (deliberately wider than the prose); caption muted, left, at the measure. Open in a lightbox.

### Navigation
Teal navbar, white links, mist on hover, 1px forest-deep bottom border, logo capped at 34px. The current item is weight 600 with a 2px underline at 0.35em offset. Sidebar and breadcrumb links keep a 24px minimum target; sidebar and TOC entries wrap at 1.35 to 1.4 leading.

### Tables
Header row in table-head-bg with forest-deep text, hairline rules, tabular numerals; tables wider than about four columns scroll inside a focusable labelled region.

## Do's and Don'ts

### Do:
- **Do** write every interface name as a `.ui` chip, exactly as the app labels it.
- **Do** give every boxed component a full 1px frame and keep its prose at 55ch.
- **Do** keep focus visible: 3px ember ring on paper, gold on teal, green and dark grounds, 2px offset.
- **Do** underline body links (1px, 2px on hover).
- **Do** add dark values as token overrides in `guane-dark.scss`, never as component rules.
- **Do** frame screenshots with `.guane-shot` and give each a specific `fig-alt`.

### Don't:
- **Don't** put a coloured side stripe on any box.
- **Don't** set a kicker, eyebrow or uppercase label above a heading; uppercase caps are field labels only.
- **Don't** load a webfont or add a `css:` file; the theme SCSS is the only stylesheet.
- **Don't** use inline `style=` attributes or raw HTML for layout.
- **Don't** use emoji or text glyphs as icons; separators like the breadcrumb chevron are drawn in CSS.
- **Don't** add shadows beyond the screenshot lift and card hover.
- **Don't** signal state by colour alone.
