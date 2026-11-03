---
version: alpha
name: Nightdesk
description: A graphite operations dashboard system for teams that live inside their numbers. Dense tables, gantt timelines, and KPI panels sit on a near-black shell, with color held back for gain, loss, and progress.
colors:
  canvas: "#303030"
  shell: "#121212"
  surface: "#1B1B1B"
  surface-raised: "#262626"
  surface-raised-hover: "#2F2F2F"
  border: "#2C2C2C"
  border-strong: "#3A3A3A"
  on-surface: "#EDEDED"
  on-surface-muted: "#8A8A8A"
  on-surface-faint: "#5E5E5E"
  on-primary: "#121212"
  primary: "#EDEDED"
  secondary: "#262626"
  neutral: "#1B1B1B"
  gain: "#3CC45A"
  error: "#E5484D"
  progress: "#2F7FF0"
  caution: "#E0B43A"
  focus: "#EDEDED"
typography:
  headline-lg:
    fontFamily: Fira Sans
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.005em
  headline-md:
    fontFamily: Fira Sans
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.3
  body-lg:
    fontFamily: Fira Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.45
  body-md:
    fontFamily: Fira Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.45
  body-sm:
    fontFamily: Fira Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Fira Sans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1
  display-figure:
    fontFamily: Sometype Mono
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  mono-value:
    fontFamily: Sometype Mono
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1
  mono-md:
    fontFamily: Sometype Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.3
  mono-axis:
    fontFamily: Sometype Mono
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1
rounded:
  none: 0px
  xs: 4px
  sm: 6px
  md: 7px
  lg: 10px
  xl: 20px
  full: 999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 20px
  2xl: 24px
  3xl: 32px
  stage: 40px
  gutter: 20px
  sidebar-width: 256px
  control-height: 34px
  row-height: 48px
components:
  app-shell:
    backgroundColor: "{colors.shell}"
    rounded: "{rounded.xl}"
  sidebar:
    backgroundColor: "{colors.surface}"
    width: "{spacing.sidebar-width}"
    padding: "{spacing.xl}"
  panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    height: "{spacing.control-height}"
    padding: 0 16px
  button-primary-hover:
    backgroundColor: "#FFFFFF"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    height: "{spacing.control-height}"
    padding: 0 16px
  button-secondary-hover:
    backgroundColor: "{colors.surface-raised-hover}"
    textColor: "{colors.on-surface}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-surface-muted}"
    rounded: "{rounded.md}"
  button-disabled:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface-faint}"
  input-field:
    backgroundColor: "{colors.shell}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    height: "{spacing.control-height}"
    padding: 0 12px
  input-field-focus:
    backgroundColor: "{colors.shell}"
    textColor: "{colors.on-surface}"
  input-field-error:
    textColor: "{colors.error}"
  checkbox:
    backgroundColor: "{colors.surface-raised-hover}"
    rounded: "{rounded.xs}"
    size: 16px
  checkbox-checked:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.xs}"
    size: 16px
  tabs-active:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    height: 26px
  tabs-inactive:
    backgroundColor: "transparent"
    textColor: "{colors.on-surface-muted}"
  nav-item-active:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    height: 36px
  kpi-figure:
    textColor: "{colors.on-surface}"
    typography: "{typography.display-figure}"
  delta-gain:
    textColor: "{colors.gain}"
    typography: "{typography.mono-md}"
  delta-loss:
    textColor: "{colors.error}"
    typography: "{typography.mono-md}"
  tooltip:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.mono-value}"
    rounded: "{rounded.md}"
    padding: 8px 12px
  gantt-bar:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    height: 40px
  table-header:
    backgroundColor: "{colors.shell}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    height: 44px
  table-row:
    textColor: "{colors.on-surface-muted}"
    height: "{spacing.row-height}"
  progress-meter:
    backgroundColor: "{colors.progress}"
    rounded: "{rounded.full}"
    height: 5px
    width: 84px
  icon-tile:
    backgroundColor: "{colors.surface-raised}"
    rounded: "{rounded.sm}"
    size: 26px
---

## Overview

Nightdesk is the late-shift operations desk. A matte charcoal canvas (`#303030`) holds exactly one inset near-black app shell (`#121212`), and inside that shell every panel is a flat graphite slab (`#1B1B1B`) cut apart by 1px hairlines. Nothing glows, nothing floats, nothing is glass. The product should feel like a well-kept ledger that happens to be on a screen: quiet, dense, legible at 2am, and completely honest about its numbers.

The emotional target is calm control. A project lead opens Nightdesk, reads cashflow against burn, scans which projects slip across the week, and closes it in under a minute. The interface earns that speed by withholding: chrome is neutral grey, and **color only appears when it means something**. Green is gain. Red is loss. Cobalt is progress. Amber is mid-risk and nothing else. If an element is colored and it is not carrying a data signal, it is wrong.

What Nightdesk must never feel like: a neon crypto terminal, a purple SaaS landing page, a glassmorphism concept shot, or a "dark mode" that is just a light theme inverted. The essential traits are the charcoal frame around a near-black shell, the tonal stepping between surfaces, the tabular monospace figures, and the signature off-hours hatch.

The signature element is the **off-hours hatch**: a 45° repeating line of 1px `#2C2C2C` every 6px over the panel color. It marks weekends and non-working columns in timelines, empty chart regions, disabled controls, and idle states. It is the only texture in the system. Idle time is drawn, never labeled.

## Colors

The palette is a tonal ladder plus four signals. Build every screen from the ladder first; add signals only where data demands them.

**Tonal ladder (darkest inside, lighter outside):**

- **Canvas `#303030`**: the page behind the shell. It frames the product like a desk mat. Never use it inside the shell.
- **Shell `#121212`**: the app frame and main work area. Also used for inputs, table header strips, and the workspace switcher, so interactive wells read as "cut into" the panel.
- **Panel `#1B1B1B`**: panels, sidebar, chart cards, tables.
- **Raised `#262626`** / **Raised-hover `#2F2F2F`**: buttons, gantt bars, the active nav row, icon tiles, tooltips, the unchecked checkbox fill.
- **Hairline `#2C2C2C`** / **Hairline-strong `#3A3A3A`**: all borders and dividers, and the hatch stroke. Strong hairlines go on raised elements and hover states only.

**Ink:**

- **Ink `#EDEDED`**: primary text, KPI figures, active labels, and the primary button fill.
- **Ink-muted `#8A8A8A`**: secondary text, table cell values, inactive nav, axis labels on hover.
- **Ink-faint `#5E5E5E`**: placeholders, axis ticks, weekday letters, disabled text.

**Signals (data only):**

- **Gain `#3CC45A`**: positive deltas, cashflow series, healthy project meters.
- **Loss `#E5484D`**: negative deltas, burn series, at-risk meters, invalid inputs.
- **Progress `#2F7FF0`**: completion meters and in-flight status. This is not a brand color and never tints buttons or links.
- **Caution `#E0B43A`**: mid-risk status bars only.

Area charts may fade their series color from 18% alpha to 0 under the line. That is the only gradient permitted anywhere. There is no brand accent hue; the brand is the grey.

Contrast: Ink on Shell is 15.9:1, Ink-muted on Panel is 5.3:1. Ink-faint fails body contrast by design, so never use it for text a user must read to complete a task.

## Typography

Two families, strictly divided by content type.

- **Fira Sans (400/500/600)** sets every word: navigation, headings, table text, buttons, tooltips' date labels. Base size is 13px, navigation and table cells 14px, panel titles 15px/500, the page heading 22px/500. Headings never exceed weight 500; the brand wordmark alone uses 600.
- **Sometype Mono (400/500)** sets every number: KPI figures at 40px/500 with -0.02em tracking, currency and dates in tables at 13px, deltas at 13px/500, tooltip values at 18px/500, axis labels at 11px, gantt counts and ratios at 12px.

Rules:

- `font-variant-numeric: tabular-nums` is on at the body level. Do not turn it off.
- If a string is mostly digits (a date, a currency, `16/20`, `56%`), it is mono. If it is mostly words, it is sans. `Last 30 days` is sans; `12.5%` beside it is mono.
- Sentence case everywhere. No all-caps labels, no letter-spaced small caps, no kicker lines above headings.
- One size step of contrast per group. A panel head has a title and nothing else; do not stack a subtitle and a caption under it.

## Layout

**Stage and shell.** The page is Canvas with 40px of padding around a single shell capped at 1440px wide, radius 20px. The shell is a two-column grid: a 256px sidebar and a fluid main column. The main column has 20px padding and a 20px vertical gap between rows of panels.

**Sidebar anatomy, top to bottom:** brand row (22px logo + wordmark, hairline below), workspace switcher (Shell well with name and chevron), `Menu` group label with hairline, nav items (36px rows, 14px text, 16px Lucide icons), `Ongoing projects` group label, project rows (26px icon tile, name, 3-bar health meter, chevron), then the upgrade card pinned to the bottom with `margin-top: auto`.

**Topbar.** A 44px Panel strip with back/forward ghost icon buttons, a breadcrumb (`Dashboard ▸ Overview`, current crumb in Ink), and a right-aligned command search (420px) ending in a `⌘K` kbd hint. There is no page hero. The dashboard begins with data.

**Dashboard rhythm.** Stack rows in this order and keep it:

1. **KPI row**: two (or three) KPI chart cards in an equal-column grid. Each card: title row (icon + title + kebab), then a two-column body with the big figure and delta on the left, the area chart plus month axis on the right, both bottom-aligned.
2. **Timeline panel**: head row with the period as the title (e.g. `May 2025`) and actions on the right (`Add project`, `Filter`, kebab), a ruled header of day columns (mono date + faint weekday letter), gantt bars, and the segmented range control (`1 Day / 1 Week / 1 Month / Full`) bottom-left.
3. **Table panel**: toolbar (240px search, Filter, Sort, then `Add project` pushed right), a Shell-colored header strip with rounded ends, 48px rows separated by hairlines.

**Density.** Nightdesk is compact but never cramped: 16px panel padding, 34px controls, 48px table rows, 8px gaps inside toolbars. Whitespace is spent between panels (20px), not inside them.

**Alignment.** Everything is left-aligned. Numbers in tables are left-aligned too, because tabular mono figures already align by column; right-aligning currency in this system creates ragged left edges against sans headers. The only right-aligned things are panel actions and toolbar end groups.

**Other section patterns.**

- *Forms / settings:* one Panel, labels stacked above 34px Shell inputs, 16px between fields, a single row of buttons at the bottom-left with the inverted primary first.
- *Detail page:* KPI row of three compact cards on top, then a two-column split (2fr table, 1fr activity panel).
- *Empty state:* a hatched `nd-empty` block inside the panel with one sentence and one action button. No illustration, no oversized icon.

**Responsive.** Below 1100px, KPI and card grids collapse to one column. Below 860px, the shell loses its radius and stage padding, the sidebar stacks above the main column, the topbar search hides, and gantt and table panels scroll horizontally inside `.nd-gantt-scroll` / `.nd-table-scroll` wrappers rather than reflowing.

## Elevation & Depth

Nightdesk is flat. Depth comes from tonal steps and hairlines, not shadows.

- **Shell** is the only element with a shadow: `inset 0 1px 0 #3A3A3A` (a lit top edge) plus `0 30px 60px -20px rgba(0,0,0,.6)` to seat it on the Canvas.
- **Tooltips** get Raised fill, a Hairline-strong border, and a two-layer subtle shadow. They are the only floating surfaces.
- **Everything else** separates via 1px hairlines and the Canvas > Shell > Panel > Raised ladder. A raised element is lighter, not higher.

Motion is limited to 140ms background/border transitions on hover. No entrance animations, no count-up figures, no parallax.

## Shapes

- Shell: 20px.
- Panels, cards, upgrade card, empty states: 10px.
- Buttons, inputs, gantt bars, nav rows, tooltips, table header strip ends: 7px.
- Segmented options and icon tiles: 6px.
- Checkboxes, kbd hints, health meters, count chips: 4px.
- Progress track: fully rounded, 5px tall.
- Avatars: circles with a 2px Raised ring, overlapped by 8px.

Everything else is square. Hairlines are always 1px. Never use a 2px border to signal state; use a lighter fill or the strong hairline.

## Components

All classes are prefixed `nd-` and live in `css/system.css`. Icons are **Lucide**, 16px, 1.5 stroke, inheriting `currentColor`.

**Buttons.** `.nd-btn` is Raised with a hairline border, 34px tall, 500 weight. `.nd-btn--primary` is inverted: Ink fill, Shell text; there is at most one per view (usually `Upgrade` or a form submit). `.nd-btn--ghost` is transparent muted text for icon actions and kebabs. `.nd-btn--icon` makes it square. Disabled buttons drop to Panel with the hatch texture and faint text.

**Inputs.** `.nd-input` and `.nd-search` are Shell wells with hairline borders. Focus lightens the border to Ink-muted; errors set it to Loss. `.nd-search` wraps a Lucide `search` icon, a bare input, and an optional `.nd-kbd` hint.

**Checkbox.** `.nd-check` on a native checkbox: 16px, 4px radius, Raised-hover fill. Checked inverts to Ink with a Shell tick. Indeterminate shows a Shell bar.

**Tabs.** `.nd-segmented` is the range control: small 26px options, the selected one on Raised with a strong hairline. `.nd-tabs` is the page-level variant: underlined with a 1px Ink rule on the active tab.

**Panel.** `.nd-panel` with `.nd-panel__head` (title flexes, actions right). Add `.nd-panel__head--ruled` when a hairline should separate the head from dense content like a gantt.

**KPI chart card.** `.nd-kpi` grid: `.nd-kpi__figure` in 40px mono, `.nd-kpi__foot` holding `.nd-delta--gain` or `--loss` (Lucide `arrow-up-right` / `arrow-down-right`) plus the muted period text. The chart uses `.nd-chart--gain|--loss` with `.nd-chart__line`, an optional 18%-to-0 area fill, a dashed `.nd-chart__crosshair`, an Ink `.nd-chart__dot`, and a positioned `.nd-tooltip`. `.nd-axis` below marks the current period with `.is-current`.

**Gantt timeline.** `.nd-gantt` is a CSS grid with `--nd-gantt-cols` columns. Day headers use `.nd-gantt__head` (mono date, faint `<small>` weekday letter). `.nd-gantt__col` draws hairline column rules; `.nd-gantt__col--off` hatches weekends. `.nd-gantt__bar` spans columns with `grid-column`, holding a name with icon tile, `.nd-gantt__stat` items (Lucide `clipboard` count, `circle-check` ratio), and an `.nd-avatars` stack.

**Data table.** `.nd-toolbar` above `.nd-table`. Header cells sit on a Shell strip with rounded ends and hold `.nd-sort` buttons with Lucide `arrow-up-down`. Rows: `.nd-cell-check`, `.nd-cell-primary` for the name in Ink, `.nd-cell-num` for dates. Progress uses `.nd-meter` with `--nd-value` and a `.nd-meter__chip` showing the percentage.

**Sidebar parts.** `.nd-brand`, `.nd-switcher`, `.nd-nav-heading`, `.nd-nav-item` (active via `aria-current="page"`), `.nd-health` (three `<i>` bars tinted `--gain|--caution|--loss`), `.nd-tile`, `.nd-upgrade`.

**Status and counts.** `.nd-status` renders a signal dot plus a real state word (`Deployment`, `Testing`). `.nd-count` holds live numbers only.

**Accessibility.** Focus is a 2px Ink ring offset by 1px of Shell (`:focus-visible`). Sort headers expose `aria-sort`; segmented options use `aria-pressed`; nav uses `aria-current`. Signals never carry meaning by color alone: deltas pair color with an arrow icon, health meters sit next to named projects, meters print their percentage.

**Framework adaptation.** Keep the `--nd-*` custom properties as the single token source. In React or Vue, wrap classes one-to-one (`<Button variant="primary">` → `.nd-btn.nd-btn--primary`) and never re-declare colors inline. Charts from any library must map series strokes to `--nd-gain`, `--nd-loss`, or `--nd-progress`, gridlines to `--nd-hairline`, and axis text to Sometype Mono 11px in `--nd-ink-faint`.

## Do's and Don'ts

**Do**

- Frame the product: Canvas outside, one 20px-radius Shell inside. Always.
- Step surfaces tonally (Canvas > Shell > Panel > Raised) to show hierarchy.
- Set every figure, date, ratio, and percentage in Sometype Mono with tabular numerals.
- Use the hatch for weekends, empty chart regions, disabled controls, and idle states.
- Pair every signal color with a second cue: an arrow, a label, or a printed value.
- Lead every panel with its title alone, then data. Start the page with the breadcrumb and KPI row.
- Keep the inverted Ink button to one per view.

**Don't**

- Never use a color for decoration. No colored icons, no colored headings, no accent-tinted links, no brand hue.
- Never use Progress blue for buttons, focus, or selection. It means "done ratio" and nothing else.
- Never add shadows to panels, cards, or buttons. Only the shell and tooltips cast shadows.
- Never use gradients beyond the 18%-to-0 fill under an area chart line.
- Never use `backdrop-filter`, glow, neon, or glass.
- Never use all-caps labels, letter-spaced micro-labels, or a label line above a heading.
- Never put decorative pills or badges on screen. A chip must display a live status, count, or percentage.
- Never invent a second texture. The hatch is the only one.
- Never scale a Lucide icon past 32px or use it as an illustration.
- Never right-align a column of mono figures against left-aligned sans headers.
