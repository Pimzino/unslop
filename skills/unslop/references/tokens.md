# Tokens

Starting values for each pass. When the project already has a good system, keep its values and only fix how they are used. These are starting points, not a house style, so let the direction move them.

## Spacing scale

4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96, 128

- Inside a control: 4 to 12
- Between related items, like rows in a list: 2 to 8
- Between groups, like a label and its list or two cards: 12 to 24
- Between sections: 32 to 64, landing sections 80 to 128
- Row heights: 32 compact, 36 default, 40 to 44 touch
- Hero: 96 to 128 from the navigation to the headline on desktop, 48 to 64 on mobile

## App layout

- Sidebar 240 to 280 wide, content fluid with page padding 24 to 32, capped around 1440 to 1600.
- Top bar or page header 56 to 64 tall.
- Navigation rows 32 to 36, gap 2 to 4, section labels 24 above and 8 below.
- Stat cards in a row share one height, usually 3 or 4 compact cards per row on desktop, numbers only.
- The main chart spans at least two thirds of the content width and is 280 to 360 tall. A second data block next to it is a list or table, narrower, not another chart.

## Neutral ramps

For apps and dashboards use graphite, or a ramp just as grey, for every surface. For landing pages pick the ramp whose tint matches the world in the direction. Warm suits paper, wood, food, craft and anything human. Ink suits night, sky, water and anything technical. You can tint your own ramp the same way, keeping saturation very low, so a surface never reads as a color on its own.

### Dark

| Role | Graphite | Warm | Ink |
| --- | --- | --- | --- |
| Deepest surface, like a sidebar | #0f0f10 | #12110f | #07080d |
| Page background | #141415 | #161513 | #0b0d14 |
| Card | #19191b | #1c1a18 | #11141c |
| Raised, like an active row or input | #232325 | #262421 | #1a1e28 |
| Hairline | primary text at 8% | primary text at 8% | primary text at 8% |
| Primary text | #ededed | #efe9de | #eef0f5 |
| Secondary text | #a1a1a6 | #aaa398 | #a3a9b8 |
| Muted text and icons | #85858b | #8a847a | #7a8296 |

### Light

| Role | Graphite | Warm | Ink |
| --- | --- | --- | --- |
| Page background | #fafafa | #f7f4ee | #f5f7fa |
| Card | #ffffff | #fdfbf7 | #ffffff |
| Raised, like an active row or input | #f4f4f5 | #efe9df | #eceff4 |
| Hairline | primary text at 8% | primary text at 8% | primary text at 8% |
| Primary text | #171717 | #1f1b16 | #111827 |
| Secondary text | #525252 | #5e554a | #4b5565 |
| Muted text and icons | #737373 | #7b7266 | #6b7487 |

Muted text is for meta and captions only and stays near 4.5 to 1 on its surface. Body text uses primary or secondary.

### Text as one ink

Instead of three fixed colors, the text roles can be the primary text color at three opacities, so they stay in tune on every surface and over images. A warm dark page that works this way:

| Role | Value |
| --- | --- |
| Page | #151413 |
| Panel | #1c1b19 |
| Raised | #252321 |
| Hairline | #ece4d4 at 8% |
| Primary text | #efe9de |
| Secondary text | primary at 64%, or 85% for list items that need to read |
| Muted text | primary at 40% |

Check muted text against its surface, it must still reach about 4.5 to 1 for anything people need to read.

### Moment colors

Colors that only live inside the moment are named after their material and kept in their own group, apart from the ramp. A fire: `glow #e2b383`, `flame #ffb470`, `ember #ff7d38`, `core #fff4e4`. A reef: `sea #3aa3b8`, `deep #03131a`, `kelp #5d6e22`, `sand #ddb565`. These are examples of the idea, derive your own from the world.

Semantic colors, toned to sit inside any ramp: positive #4cc38a on dark and #16a34a on light, negative #e5484d on dark and #dc2626 on light.

## Accent

- Keep a real brand color. A violet to blue or any other hue to hue glow gradient is slop, not a brand color, unless the user says otherwise.
- Without a brand color, take it from the world. Warm worlds suit amber, coral or ember orange. Cool worlds suit cobalt, teal or a clear sky blue. Natural worlds suit moss or sage. Avoid the purple to blue family unless the brand really is purple.
- Text on the accent reaches 4.5 to 1 contrast. Darken the accent or use dark text when it does not.
- The accent covers a few percent of the screen, like the primary action, the selection and one key figure.

## Buttons

- Hero buttons 44 to 48 tall, navigation buttons 32 to 36, padding 16 to 20 on the sides.
- Primary on dark: an off white from the ramp with dark text, or the accent. Primary on light: the primary text color as a fill with white text, or the accent.
- Secondary: the raised surface with a hairline, primary text.
- A soft top highlight like `inset 0 1px 0 rgba(255,255,255,0.12)` on dark buttons gives depth without a glow.
- Button labels are 14 to 15px at 600. Buttons and chips may be pills.
- A button can carry its shortcut as a small keycap after the label, like `Start typing ↵`.
- A button that belongs to the hero object can take its material, like a graphite metal fill next to a black typewriter. It is still one tone shifting, never two hues.

## Type families

Pick by the character in the direction. All of these are free, and a partner can come from any row.

| Character | Interface family | Optional partner |
| --- | --- | --- |
| Precise, technical, calm | Geist, Inter, Inter Tight, IBM Plex Sans | Geist Mono, IBM Plex Mono, JetBrains Mono for figures and meta |
| Warm, friendly, human | Instrument Sans, DM Sans, Figtree | Instrument Serif or Newsreader for the hero headline only |
| Editorial, literary, crafted | Inter or Instrument Sans for the interface | Newsreader, Instrument Serif or Fraunces for headlines |
| Playful, bold | Space Grotesk, Bricolage Grotesque | a mono for small labels |
| The world has its own type | the interface family from another row | the world's face for the headline only, like Courier Prime for a typewriter, a pixel face like Silkscreen or Pixelify Sans for a game, a book serif like EB Garamond for reading |

A display serif or a world face belongs to large headlines only, never to labels or buttons. A pixel face is the exception when the whole page is the game.

Prefer a variable version of the family, so weights between the steps are available.

## Type scale

| Use | Size | Line height | Weight |
| --- | --- | --- | --- |
| Small labels, meta, counts | 12 | 16 | 400, mono welcome |
| Secondary text, captions | 13 to 14 | 20 | 400 |
| Body, nav items | 14 to 16 | 20 to 24 | 400 to 450 with a variable font, 500 for the selected item |
| Buttons, small titles | 14 to 16 | 20 to 24 | 600 |
| Logo wordmark | 16 to 18 | 1 | 500 to 600 |
| Hero subhead | 18 to 20 | 28 to 30 | 400, secondary color, at most 36rem wide |
| Card figures | 28 to 32 | 1 | 500, tabular |
| Page title | 28 to 36 | 1.15 | 400 to 500 |
| Hero headline | 56 to 72 desktop, 36 to 44 mobile | 1.02 to 1.08 | 400 to 500 |

Letter spacing is 0 to 0.02em for anything under 16px, slightly positive reads well on dark pages. Display text from 40px can go to -0.02em, and from 56px to -0.03em, for a family with normal spacing like Inter or Geist. A family that is already tight, like Inter Tight, needs only -0.01em or none at display sizes. A monospace headline needs more, around -0.03em, because its letters are spaced for typing, not reading.

## Radius

| Element | Radius |
| --- | --- |
| Keycap, tag, small button | 4 to 6 |
| Row, input, button | 8 to 10 |
| Card | 12 to 16 |
| Panel or window | 14 to 20 |
| Dialog, large frame or bezel on a landing page | 24 to 28 |
| Button or chip | 8 to 10, or a pill |

Nested radius: inner = outer − padding, never below 4. A 16px card with 8px padding holds items with an 8px radius. A 28px bezel with 8px padding holds a screenshot or video with a 20px radius.

## Icons

lucide, 16 or 18px, stroke 1.5, color of the muted or secondary text role, 8 to 10px gap to the label.

## Depth

- Dark: surface steps plus a hairline. An active row can carry `inset 0 1px 0 rgba(255,255,255,0.12)` as a top highlight.
- Light: `0 1px 2px rgba(0,0,0,0.05)` for small things, `0 8px 24px rgba(0,0,0,0.06)` for floating ones.

## Materials

Recipes for surfaces that should feel like real objects. Values are for a dark warm page, swap the ink for your ramp.

- **Dialog or floating panel.** A light ring inside, a dark ring outside and one long soft drop. `box-shadow: inset 0 0 0 1px rgb(239 233 222 / 0.07), 0 0 0 1px rgb(0 0 0 / 0.6), 0 40px 90px -30px rgb(0 0 0 / 0.95)`.
- **Quiet button, lit from above.** A tone shift in one neutral, a top highlight, a dark lower edge and a small drop. `background: linear-gradient(#2d2b28, #211f1d); box-shadow: inset 0 0 0 1px rgb(239 233 222 / 0.1), inset 0 1px 0 rgb(255 255 255 / 0.1), inset 0 -1px 0 rgb(0 0 0 / 0.35), 0 1px 2px rgb(0 0 0 / 0.5)`.
- **Bezel.** A frame around a screenshot, video or device. Outer radius 28, padding 8, inner radius 20, frame a step above the page, and an inner ring of white at 5% on the image so its edge does not bleed into the frame.
- **Cursor light.** A radial gradient on the surface that follows the pointer through two custom properties set from `pointermove`, faded in on hover over 500ms. On a quiet button it is the ink at about 9%, `radial-gradient(140px 70px at var(--gx) var(--gy), rgb(239 233 222 / 0.09), transparent 75%)`. On the one lit button it is the hot core of the moment color, `radial-gradient(120px 80px at var(--gx) var(--gy), var(--core), color-mix(in srgb, var(--core) 50%, transparent) 45%, transparent 80%)`. Primary action and hero object only.
- **Lit ring.** For the one primary action or the one card that matters. A conic gradient in the moment colors turning slowly behind the element, shown only on its border with `mask: linear-gradient(#000 0 0) content-box exclude, linear-gradient(#000 0 0)`, plus a small ember shadow under it, `0 8px 22px -10px color-mix(in srgb, var(--ember) 40%, transparent)`. Turn time 10 to 16 seconds.
- **Frosted chip over a scene.** Only when there is an image behind it to blur. `background: linear-gradient(rgb(255 255 255 / 0.46), rgb(255 255 255 / 0.2)); backdrop-filter: blur(9px) saturate(1.4); box-shadow: inset 0 0 0 1px rgb(255 255 255 / 0.55), inset 0 1px 0 rgb(255 255 255 / 0.85), 0 10px 28px -14px` with a shadow color taken from the scene's light, and text in a dark tone of the scene, not grey.

## Motion

One easing curve for everything, `cubic-bezier(0.22, 1, 0.36, 1)`.

| Use | Duration |
| --- | --- |
| Hover, press, toggles | 120 to 180ms |
| Menus, popovers, tooltips | 160 to 220ms |
| Entrances, sheets, layout changes | 300 to 500ms |
| Stagger between items | 40 to 60ms, at most six items |

| Hover lift of a gallery tile | 500ms, 2 to 4px |
| Sheen on one word of a moment | 4 to 6s, linear, looping |
| Turning light on a lit ring | 10 to 16s, linear, looping |
| One reward pop, like a check after success | 500 to 600ms, peak at 1.08 |

- Rise distance on enter: 6 to 14px, with an optional scale from 0.985. Press scale: 0.97 to 0.98.
- Transition color, background, border, opacity and transform only.
- A second curve, `cubic-bezier(0.65, 0, 0.35, 1)`, is fine for things that travel and come back, like a toggle sliding or bellows opening.
- Under `@media (prefers-reduced-motion: reduce)`, loops pause on a good frame, entrances become a 150ms fade, and physics jumps to its rest state.

---

Part of unslop by Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0. Keep this credit in copies and adaptations.
