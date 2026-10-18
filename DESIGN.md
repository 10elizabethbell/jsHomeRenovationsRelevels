---
name: J's Home Renovations & Relevels LLC
description: Mobile home sets and relevels. Rain or shine, we work all the time.
colors:
  ground: "#1b2a39"
  ground-2: "#213446"
  ground-3: "#2a4055"
  paper: "#eceae4"
  paper-ink: "#1b2a39"
  paper-muted: "#4a5866"
  ink: "#f3f1ea"
  muted: "#b7c3cf"
  level: "#f2c230"
  level-bright: "#ffd651"
  level-on-paper: "#7d5f00"
  vial: "#c9e25a"
  rain: "#8fcbff"
  line: "rgba(243,241,234,.16)"
  line-on-paper: "rgba(27,42,57,.14)"
  field-stroke: "rgba(243,241,234,.18)"
  error: "#ffb3a1"
  error-stroke: "#ff9c85"
typography:
  display:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(3.3rem, 17vw, 6rem)"
    fontWeight: 900
    lineHeight: 0.86
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2.1rem, 9vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1.6rem, 7vw, 2.3rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title-sm:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "0"
  lede:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    lineHeight: 1.15
  numeral:
    fontFamily: "system-ui, -apple-system, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "44px"
    fontWeight: 900
    lineHeight: 1
    fontFeature: "\"tnum\""
rounded:
  control: "12px"
  focus: "6px"
  round: "50%"
spacing:
  gutter: "20px"
  tight: "10px"
  gap: "16px"
  block: "28px"
  section-top: "56px"
  section-bottom: "64px"
  section-top-wide: "84px"
  section-bottom-wide: "92px"
  container: "1120px"
components:
  button-primary:
    backgroundColor: "{colors.level}"
    textColor: "{colors.paper-ink}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 10px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.level-bright}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 10px"
    height: "56px"
  input:
    backgroundColor: "{colors.ground-3}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "14px"
    height: "54px"
  chip:
    backgroundColor: "{colors.ground-3}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper-ink}"
  row-arrow:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.round}"
    size: "44px"
  row-arrow-active:
    backgroundColor: "{colors.level}"
    textColor: "{colors.paper-ink}"
---

# Design System: J's Home Renovations & Relevels LLC

## Overview

**Creative North Star: "Back to Level in the Rain"**

A mobile home sits crooked under a storm-slate sky, and a crew comes out anyway and puts it back to level. Every surface of the system is drawn from that one scene: wet slate for ground, rain-washed siding for the light bands, and a single yellow spirit level whose bubble is the whole story. The yellow is the crew's tool, so it marks the one thing to do on any screen and the moment something reads true.

The voice is a working crew talking on the phone: heavy, uppercase, short headings in the device's own system face, then plain sentence-case body copy at a comfortable phone size. Density is low and single-column on phones, with big touch targets (44px minimum, 56px for primary actions). Bands of slate and paper are joined by puddle-surface seams that keep moving, so the page itself is weather.

The hero is a living canvas scene, not a photo: the visitor drags the home back to level themselves, and the level bubble confirms it.

**Key Characteristics:**
- Storm-slate ground with rain-washed paper bands; one yellow accent.
- Heavy uppercase system type for headings; sentence-case body.
- Flat UI chrome; depth comes from tonal bands and the painted scene.
- One 12px radius across every control.
- Moving puddle-wave seams between bands; motion is weather, not decoration.

## Colors

A cold, wet slate world with one warm tool-yellow in it, plus a rain-blue that only appears where water or text entry is involved.

### Primary
- **Level-Tool Yellow** (`level`): the spirit level. Primary buttons, the emphasized word in the display headline, the wordmark initial, the phone icon, the service-row arrow on hover and focus, text selection, and the global focus ring.
- **Struck-Bright Yellow** (`level-bright`): the hover state of the primary button only.
- **Paper-Safe Level** (`level-on-paper`): yellow pushed down to a dark ochre so it holds contrast on the paper band; used for the step numerals.

### Secondary
- **Rain Blue** (`rain`): text-field and chip hover/focus borders, and (at 35% alpha) the water line of the puddle seams on dark bands. It belongs to the form and the water.

### Tertiary
- **Vial Green** (`vial`): the spirit-level fluid. In the UI it appears only as confirmation, when the hero hint switches to "Level." state.

### Neutral
- **Storm Slate** (`ground`): page background, the hero, the quote section; also the ink on paper (`paper-ink` is the same slate).
- **Wet Slate** (`ground-2`): the alternate dark band (services, close, footer).
- **Slate Puddle** (`ground-3`): recessed fill for inputs and unselected chips.
- **Rain-Washed Siding** (`paper`): the light band for explanatory content.
- **Paper Muted** (`paper-muted`): secondary text on paper.
- **Bone Ink** (`ink`): primary text on dark; also the fill of a selected chip.
- **Fog** (`muted`): secondary text on dark: ledes, row descriptions, footer.
- **Hairlines** (`line`, `line-on-paper`, `field-stroke`): 1px list rules and 2px control strokes, always translucent ink over the band they sit on.
- **Error Coral** (`error`, `error-stroke`): validation message text and the invalid input border on dark.

### Named Rules
**The One Bubble Rule.** Level yellow is the only accent in the UI chrome, and it means "this is the action" or "this is true". At most one yellow-filled control per viewport cluster; everything else is slate, paper, or ink.

**The Water Belongs to the Form Rule.** Rain blue is never a button fill or a headline color. It appears on input focus/hover and on the seams' water line, nowhere else.

**The Yellow-Off-Paper Rule.** Level yellow never sits as text on the paper band; use the paper-safe level there.

## Typography

**Display Font:** system UI stack (system-ui, -apple-system, "Segoe UI", "Helvetica Neue", Arial, sans-serif)
**Body Font:** the same stack
**Label/Mono Font:** the same stack; numerals use tabular figures

**Character:** One family, voice carried entirely by weight and case. Black-weight (900) uppercase headings with tight negative tracking and sub-1 line-heights shout like a hand-painted truck door; body is regular weight sentence case and reads like a text message. The system stack is a deliberate house choice: it renders instantly in Facebook's in-app browser and looks like the visitor's own phone.

### Hierarchy
- **Display** (900, clamp(3.3rem, 17vw, 6rem), 0.86, uppercase): the hero headline only. One word may take level yellow.
- **Headline** (900, clamp(2.1rem, 9vw, 3.6rem), 0.95, uppercase): section headings. The closing band scales it up to clamp(2.3rem, 11vw, 4.6rem).
- **Title** (900, clamp(1.6rem, 7vw, 2.3rem), uppercase): service row names.
- **Title Small** (900, 22px, uppercase, no tracking): step names.
- **Lede** (400, 18px, max 52ch): the line under a section heading, in fog or paper muted. Hero promise runs clamp(17px, 4.6vw, 20px) at 1.4 and 30ch.
- **Body** (400, 17px, 1.55): all running copy. Emphasis is bold weight in the full-strength ink color, never yellow.
- **Label** (800, 16px): buttons, form labels and legends, the phone number. Optional markers drop to 500 in muted.
- **Numeral** (900, 44px, tabular): step numbers.

### Named Rules
**The Shout-Then-Talk Rule.** Headings are 900-weight uppercase with tight tracking; everything below a heading is sentence case. Never set body or button text in uppercase.

**The House Stack Rule.** The system stack is the only typeface. Do not import a webfont; weight (400/600/700/800/900) and case carry all hierarchy.

## Layout

Phone-first single column inside a 1120px container with a 20px gutter. Sections pad 56px top and 64px bottom on phones, 84px and 92px from 1024px up. Lists start 26 to 30px under their heading; a second heading inside one band sits 64px below the previous content.

At 1024px and up, the hero becomes a two-column grid (copy 1fr, scene 1.3fr) with the scene bleeding to the right edge, and content sections with a heading-plus-list structure split into 1fr / 1.2fr columns with a 64px gap. Steps go to three columns at 900px. Below 380px, the wordmark, buttons and phone tighten and the phone icon drops.

**The Phone-First Column Rule.** Compose for one column at 375px first; wide layouts only split heading from content, they never add new content.

**The Thumb Rule.** Every interactive element is at least 44px tall; primary actions are 56px.

## Elevation & Depth

The UI chrome is flat: no box-shadows anywhere. Depth comes from tonal banding (storm slate, wet slate, slate puddle for recessed fields) and from the alternation of dark and paper bands. The only shading on the page is painted inside the hero scene as part of the world (eave shade, the level's shadow, fog over the treeline).

**The Weather-Not-Shadow Rule.** Controls never lift off the page with shadows; they sit in it. Recess with a lighter slate fill, emphasize with yellow, separate with hairlines.

## Shapes

One radius for everything a thumb touches: gently rounded 12px corners on buttons, inputs, chips and the Facebook link. The service-row arrow is a full circle. Focus rings round at 6px. Lists are open, divided by 1px hairlines rather than boxed. The only curved silhouette at page scale is the puddle seam's water line; the in-scene spirit level and its vial are capsule-shaped.

**The One Radius Rule.** Controls use 12px; nothing else gets a corner value. No cards, no pills on buttons.

## Components

### Buttons
Tactile, square-shouldered, heavy-labelled.
- **Shape:** 12px radius, 2px level-yellow border on every variant, 56px tall.
- **Primary:** level yellow fill with slate label.
- **Hover / Focus:** primary brightens to struck-bright yellow; ghost takes a 12% yellow wash. Background and color transition in 0.2s; press nudges down 1px. Focus uses the global 3px yellow ring at 3px offset.
- **Ghost:** transparent with bone-ink label and the same yellow border; always the companion to a primary in a pair (grid 1fr / 1.25fr, 10px gap, max 440px).
- **Submit:** the primary button at full form width (max 620px).

### Chips
- **Style:** slate-puddle fill, 2px translucent ink stroke, 12px radius, 48px tall, 700 weight. Single-select radio groups.
- **State:** hover and keyboard focus turn the stroke rain blue; selected inverts to bone-ink fill with slate text.

### Inputs / Fields
- **Style:** slate-puddle fill, 2px translucent ink stroke, 12px radius, 54px min height (textarea 96px, vertical resize only), 500 weight 17px text, placeholder in a light slate.
- **Focus:** stroke turns rain blue (also on hover); no glow.
- **Error:** stroke goes error coral and a 15px/600 coral message appears under the field; validation runs only after the first submit attempt.

### Navigation
A header row, not a menu: the wordmark at left (yellow 900-weight initial at 30px beside a two-line 11.5px uppercase 800-weight business name in ink) and a tap-to-call phone number at right (800 weight, tabular figures, yellow handset icon, underline in yellow on hover). There are no nav links.

### Service Rows
An open list of oversized uppercase titles divided by hairlines, each row a link to the quote form that preselects the matching job. The row itself never highlights; only the 44px circular arrow reacts, filling level yellow on hover and focus.

### Signs List
On paper: an open list at 18px/600 with hairline separators, each item marked by a small slate bar (a level's body seen edge-on) rather than a bullet or checkmark.

### Level Scene (signature)
The hero canvas: a mobile home on cinder-block piers with a wood cap, steel beams, lap siding, and a yellow spirit level lying on the roof, under slanting rain in front of a treeline silhouette over wet dirt with puddles. Top and bottom (and left/right on desktop) fade out via a mask so it dissolves into the slate.
- **Behavior:** idle, the crew loops: the home settles to a random 1.8 to 3.0 degree tilt, a red bottle jack appears at the low end and lifts it to level, window lights warm up, then it settles the other way. Dragging either end tilts it (0.032 degrees per px, clamped at 4.2); releasing within 0.45 degrees snaps to level; the crew resumes after 4.5 s idle. The bubble follows with a damped spring. When level, the hint below turns vial green and reads "Level. That's how we leave it."
- **Rain:** 150 drops on phones, 320 on desktop; the pointer pushes rain aside like an umbrella; drops splash on the roof and ripple in puddles.
- **Height:** clamp(250px, 40svh, 360px) on phones, 540px on desktop.
- **Reduced motion:** renders level and static; drag still works, redrawing on input only.

### Puddle Seam (signature)
A 48px full-width SVG that joins two bands: the lower band's color fills below a water line built from three summed sine waves (swell 3px, ripple 1.5px, plus a 0.6px chop), so the seam drifts continuously. A 2px stroke traces the water line: rain blue at 35% on dark-to-dark or dark-to-paper seams, slate at 25% when leaving paper. Wavelength scales with element width so bumps keep the same physical size on phones. Animation pauses offscreen and is static under reduced motion.

**The Water Line Rule.** Bands that change color between story chapters meet at a puddle seam, not a straight edge or a diagonal.

**The One Loop Rule.** All continuous motion shares one requestAnimationFrame loop, each piece pauses when offscreen, and every motion has a reduced-motion state that still shows the finished picture.

## Do's and Don'ts

### Do:
- **Do** keep level yellow for the single primary action, the true/level moment, and focus.
- **Do** set headings in 900-weight uppercase system type with negative tracking, and everything else in sentence case.
- **Do** join color bands with a moving puddle seam (48px, swell 3, ripple 1.5).
- **Do** use the 12px radius and 2px strokes on every control, with 44px minimum and 56px primary touch targets.
- **Do** recess inputs and chips with slate puddle fill and turn their stroke rain blue on hover and focus.
- **Do** pause any animation offscreen and provide a static, complete reduced-motion state.

### Don't:
- **Don't** add a second accent to the UI chrome; red, green and blue in the hero scene are world objects (jack, vial, rain), not palette.
- **Don't** put drop shadows or gradients on UI controls or bands; shading belongs only inside the painted scene.
- **Don't** import a webfont or use a display face other than the system stack.
- **Don't** box content in cards; use open lists with hairline rules.
- **Don't** set level yellow as text on the paper band.
- **Don't** use stock imagery or icon-font glyphs; imagery is the drawn scene (or the crew's own work), icons are inline stroked SVG.
