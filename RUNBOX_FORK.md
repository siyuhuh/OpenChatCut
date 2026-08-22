# Runbox OpenChatCut Fork

This fork keeps OpenChatCut's editor, timeline, export, Remotion runtime, and MCP bridge close to upstream. Runbox-specific behavior lives in a small personalization layer so upstream releases remain practical to merge.

## Personalization layer

- `src/skins.ts`: Runbox editor skin.
- `src/editor/design-presets.ts`: Runbox video Design Style.
- `src/components/settings/designStyleLocalization.ts`: Chinese labels for the Design Style.
- `src/agent/skills/runbox-series-video/`: repo-grounded series workflow and visual grammar.

Avoid changing timeline, export, persistence, or MCP internals unless a real series-video requirement cannot be implemented through these extension points.

## Upstream sync

```bash
git fetch upstream
git rebase upstream/main
npm run verify:skills
npx tsx src/skins.verify.ts
npx tsx src/components/settings/design-style-localization.verify.ts
```

Resolve upstream conflicts inside the personalization layer first. Keep product-specific media and episode projects outside this repository.

## License boundary

OpenChatCut is AGPL-3.0-or-later. Keep this fork and distributed modifications under that license and preserve notices. Exchange project files or MCP calls with the MIT-licensed `reel-forge` repository instead of copying OpenChatCut runtime code into it.
