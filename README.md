# unslop

Created by Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), who started the [Unslopping series](https://x.com/heydamir/status/2115063463063998736) on X.

> **This is a fork.** The original is [heydamir/unslop](https://github.com/heydamir/unslop). The `main` branch here mirrors it unchanged. The `improvements` branch adds the rules Damir's own sites follow that the original skill leaves out. See [What this branch adds](#what-this-branch-adds) and [CHANGES.md](CHANGES.md).

![A vibecoded dashboard unslopping itself, frame by frame](skills/unslop/references/refs/story-dashboard-frames.webp)

unslop is a skill for Claude that turns vibecoded, AI-looking UI into a designed interface with its own character. It finds the slop first, the purple gradients, glows, emoji labels, shouty copy and uneven spacing, then sets a direction from your product and fixes the screen pass by pass like a designer doing a redline review. It works in whatever your screen is built with, like Next.js, React, Vue, Svelte, Tailwind or plain HTML and CSS, on dashboards, apps and landing pages, and even on a live site when all you have is a link.

## Install

For Claude Code, clone the `improvements` branch and copy the skill into your skills folder. If you already have the original installed, remove it first, since both are called `unslop`.

```bash
rm -rf ~/.claude/skills/unslop
git clone -b improvements https://github.com/Pimzino/unslop
mkdir -p ~/.claude/skills && cp -r unslop/skills/unslop ~/.claude/skills/
```

For a single project, copy it into `.claude/skills/` inside that project instead.

To update later, pull and copy again.

```bash
cd unslop && git pull
rm -rf ~/.claude/skills/unslop && cp -r skills/unslop ~/.claude/skills/
```

For claude.ai, zip the skill folder and upload the file in the skills section of your claude.ai settings.

```bash
cd unslop/skills && zip -r unslop.skill unslop
```

## Use

In Claude Code, type `/unslop` with what you want, or just ask in your own words and Claude picks the skill up by itself.

```
/unslop this dashboard
/unslop the hero of https://example.com
/unslop my landing page and make the story video so I can post it
```

It audits the screen and proposes a direction before it edits anything, so you can steer it early. If the screen is already good, it tells you so and suggests a few small refinements instead of redesigning it.

## What it does

- **Audit.** Lists every sign of slop with where it lives.
- **Direction.** Character, world, the one or two moments that carry the color, and a signature detail, all taken from your product. Landing pages, empty states and 404s also get a concept, one object and one verb.
- **Passes.** Spacing, color, icons, copy, type, layout, details, visuals and motion, in that order.
- **Visuals.** Shows your product instead of a glossy blob. When a hero needs a scene or an object, it can generate one through an image service like fal, Replicate, OpenAI images or Higgsfield. If none is connected, it offers to connect one as an MCP server, and it shows the prompt and asks before every paid generation. Dashboards and apps rarely need one.
- **Story video.** A square video under 10 seconds of your screen unslopping itself, ready to post. It needs Playwright and ffmpeg.

Try it on the two vibecoded screens in [examples](examples).

## What this branch adds

The original rules ban some things Damir's own pages on [heydamir.design](https://heydamir.design) and [living-ui.dev](https://living-ui.dev) rely on, like one copper sheen on a headline word, a lit primary button, frosted chips over a scene and slow loops. This branch keeps those bans for the chrome and lets one effect through inside the moment, when something in the product's world explains it.

- **Moment effects.** A four part test for when an effect is allowed: physical, from the world, on the moment only, calm.
- **Living concepts.** A new [references/living.md](skills/unslop/references/living.md) on finding the one object and the one verb for a landing page, an empty state or a 404, and building it in code.
- **Materials.** Measured recipes in the tokens for a dialog shadow, a quiet lit button, a bezel, cursor light, a lit ring and frosted chips.
- **Type.** Inter Tight, the world's own typeface for headlines, variable weights and tracking by family.
- **Copy.** One turn of phrase, a plain line on how to play, human status lines.
- **Accessibility.** Reduced motion, sound off until asked for, keyboard hints.
- **Unslop slop check.** So the skill doesn't turn every product into warm graphite and copper.

The nine passes, the audit and polish modes, the story video, the scripts and the examples are unchanged. The full list is in [CHANGES.md](CHANGES.md).

## Keeping up with the original

`main` follows [heydamir/unslop](https://github.com/heydamir/unslop) and `improvements` sits on top of it. When the original changes, click **Sync fork** on `main` in GitHub, then merge it into this branch.

```bash
git checkout improvements
git pull
git fetch origin main
git merge origin/main
git push
```

Conflicts only happen where the original edits the same lines as this branch. Keep both changes where you can.

## Hire the unslopper

Would rather have a designer do it? Damir unslops one key screen in 3 days, built in your stack, at [heydamir.design/unslop](https://heydamir.design/unslop).

## License

[CC BY 4.0](LICENSE). Use it, change it and share it, including commercially, as long as you credit Damir Sokolovsky ([@heydamir](https://x.com/heydamir)) and link back to the [original repository](https://github.com/heydamir/unslop). This fork is an adaptation under the same license, with its changes listed in [CHANGES.md](CHANGES.md).
