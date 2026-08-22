---
name: runbox-series-video
description: |
  Build a repeatable product-video series for Runbox or another developer tool from a real product repository, existing talking-head footage, and a shared visual system. Use when the user wants repo-grounded scripts, curiosity-first product demos, reusable Runbox Motion Graphics, or a sustainable series workflow instead of a one-off edit.
user-invocable: true
---

# Runbox Series Video

Use this workflow to turn a real software project into a repeatable family of videos. The goal is not to list every feature. Each episode should create one useful question, prove one concrete idea, and leave the editor with reusable visual building blocks.

Read [references/runbox-design-system.md](references/runbox-design-system.md) before creating Motion Graphics or setting a project-wide Design Style.

## Ground every claim

Treat the product repository as the source of truth.

1. Read the README, package manifest, release/version metadata, and the implementation behind every screen or capability named in the script.
2. Record each proposed claim with its evidence path and the visible shot that can prove it.
3. Remove or soften claims that cannot be demonstrated in the current build.

An external coding agent may inspect a local repository directly. The editor's internal agent cannot assume local filesystem access; when repository evidence is unavailable, use project attachments or ask for the relevant README, screenshots, or product URL.

## Establish the episode before editing

Write a compact episode brief with:

- viewer problem;
- curiosity-first hook;
- one-sentence promise;
- proof moment;
- call to action;
- target duration and platform;
- reusable visual motif.

For a first-contact product video, lead with the user's messy workflow or surprising result. Explain implementation details only after the viewer understands why the product exists. Do not open with a feature inventory.

## Work in dependency order

1. Finalize the spoken structure and A-roll timing.
2. Confirm the representative visual direction.
3. Apply the `Runbox Control Plane` Design Style or an approved derivative.
4. Create exactly one representative Motion Graphic and inspect composed timeline frames.
5. Wait for user approval before producing the rest of the visual batch.
6. Add B-roll, captions, and music only when requested and only after timing is stable.
7. Verify the editable timeline before export.

Use `talking-head-guide` for speech cleanup and placement judgment. Use `create-motion-graphics` for direct-authored Motion Graphics and follow its property, font, canvas, and verification contracts.

## Choose moments that deserve Motion Graphics

Use Motion Graphics when code can explain an invisible relationship faster than a screen recording:

- several tools or projects converging into one workspace;
- local folders becoming a browsable project map;
- a command moving from task to terminal to result;
- Git state changing through clear checkpoints;
- a repeated workflow becoming a reusable preset.

Do not cover strong product footage with decorative animation. If the real interface already proves the point, use a crop, highlight, pointer, or short label instead.

## Build reusable components, not repeated scenes

Reuse a Motion Graphic asset only when the viewer task, information shape, and spatial form repeat. Expose titles, labels, colors, numbers, and fonts as editable properties. Create a separate asset when the explanation changes, while preserving the same palette, typography, line weight, and motion rhythm.

Useful recurring families:

- `Convergence Map` for chaos becoming organized;
- `Command Route` for step-by-step execution;
- `Git Checkpoint` for change, review, and restore;
- `Feature Focus` for one interface detail plus one claim;
- `Series End Card` for repository link and next episode.

## Preserve the series system

After approval, save the Design Style and keep a short series bible containing the approved palette, fonts, motion rules, safe zones, caption treatment, recurring components, and examples of what to avoid. New episodes should reuse the system while introducing at most one new visual motif.

The live OpenChatCut project remains the review surface. Do not export merely to prove an edit. Export only when the user requests delivery or the edit is approved as final.
