# Living concepts

How to find the one object at the center of a landing page, an empty state or a 404, and how to make it answer when people touch it. Read this before writing the concept line of the direction. Skip it for dashboards and app screens.

These rules come from the concepts on [heydamir.design](https://heydamir.design) and the playgrounds on [living-ui.dev](https://living-ui.dev), all by Damir Sokolovsky. If you have a browser, open two or three of the playgrounds before you start and use them, then come back. Take how they think, never their objects.

## What a concept is

One sentence with three parts: an object, a verb, and why it belongs to this product.

- `A real accordion whose bellows open into the answers` for an FAQ
- `The digits of the 404 sinking into a small reef you can stir by shaking the window` for a page not found
- `A typewriter where every key lands on paper and typos stay` for a typing test
- `A snow globe with the cabin inside that you grab and shake` for a winter rental
- `A shredder on a desk that eats the file you drag into it` for a privacy tool

The examples only show the shape. Never reuse their objects.

## Finding the object

Try these in order and stop at the first one that gives a clear object.

1. **Take a word literally.** The product name, the section name or the component name often is an object already. Accordion, sank, clack, stillwood, margin, touch grass. Read the page and list its nouns and verbs, then ask which of them you could hold.
2. **Find the old thing the product replaces.** A typing test replaces a typewriter, a notes app replaces a notebook, an invoice tool replaces an envelope, monitoring replaces a lighthouse keeper. The old thing is rich, physical and known to everyone.
3. **Show the promise as a physical event.** `Invoices that chase themselves` becomes a paper plane made of figures. `One light, every color` becomes a glass slab splitting a beam. The headline and the object say the same thing.
4. **Use the product's own material.** Money for finance, notes for music, characters for code, letters for writing. Draw the object out of it, see the glyph treatment in [effects.md](effects.md).

If nothing gives a clear object in a few minutes, there is no concept. Use the scene hero or the product view instead. A forced object is worse than none.

## Picking the verb

The verb is what the visitor does, and it should be what the real object is for.

- **Press** keys, buttons, a stamp
- **Shake** a globe, a jar, the window itself
- **Drag** a file into a shredder, a digit out of the water
- **Type** on a typewriter, a terminal, a note
- **Hover** to move a light, a lens, a spectrum
- **Play** a record, a tape, a music box
- **Open** bellows, a door, a book, a drawer

One verb per page. The interface's own job should map onto it when it can: an accordion component opens like an accordion, a 404 page sinks, a download falls into a folder.

## Building it

- Build what people touch in code. HTML and CSS for parts with text and clear shapes, like keys, labels, paper and buttons. Canvas for many small moving things, like water, snow, sparks or glyphs. WebGL only when the object needs real light and depth.
- A generated image can be a material inside it, like the marbled vinyl of a record or the wood of a desk, never the whole interactive thing.
- Name the colors of the world after their materials and keep them in their own group of tokens, like `sea`, `kelp`, `sand`, `crab` for a reef or `ember`, `flame`, `core` for a fire. The chrome around the object keeps its quiet ramp.
- Movement copies the real thing. Weight, settling, a small delay before water calms, a key that springs back. Use one physics model and tune it, do not chain eases.
- The object works the moment the page loads, with a still state that already reads well, so a screenshot or a visitor who never touches it still sees a designed page.

## Making it discoverable

- The copy says how to play in plain words, right under the headline or next to the object: `Give the window a shake to stir the water, or fish a digit out and toss it back in`.
- Every action has a keyboard path, shown as small keycaps, like `Space to shake`, `Enter to drive`, `Tab to try again`.
- The cursor changes over the object, to grab or pointer, so people know it is live.
- Sound is off until the visitor turns it on with a visible control, `Hear the water`, which then reads `Mute the water`.
- Under `prefers-reduced-motion` the object shows its still state and the verb still works, with the change shown at once instead of animated.

## Copy around it

- The headline names the idea in two short lines with one turn, `Typos stay on paper`, `This page sank`, `A landing page you can shake`, `One light, every color`.
- The body says what the product does, plainly, and the instruction line says how to play. Neither repeats the other.
- One dry joke is allowed in small text, like `no real vinyl was harmed`. Only one.

## Performance

- Follow the rules in [effects.md](effects.md). Read pixels once, draw from atlases, animate at the rate the thing needs, pause off screen.
- Physics and particles run at most at 60 steps per second and drop to a few per second when nothing moves.
- Cap the device pixel ratio at 2 and keep the total size of the page under a few megabytes before any video.

## When not to

- Not on dashboards, settings or screens people work in every day.
- Not in polish mode, where it goes into the report as a suggestion.
- Not when the user asked only for cleanup.
- Not twice on one page. One object, one verb.

---

Adapted from unslop by Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0. Keep this credit in copies and adaptations.
