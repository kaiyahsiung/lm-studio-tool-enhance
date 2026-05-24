# LM Studio-Tool Enhance

A local-first, hardened fork of "LM Studio for Copilot Chat" for VS Code.

## What This Fork Is

`LM Studio-Tool Enhance` is a customized fork focused on stability when using local models and tool calling.

This project is intended for local workflows where users want:
- safer tool defaults
- fewer tool-calling failures
- better behavior with smaller or less reliable local models

## Current Release

- Extension ID: `evolution-local.lm-studio-tool-enhance`
- Version: `0.1.17-enhance.2`
- VSIX file:
  - `lm-studio-tool-enhance-0.1.17-enhance.2.vsix`

## Key Changes In This Fork

- Rebranded extension identity:
  - `name`: `lm-studio-tool-enhance`
  - `displayName`: `LM Studio-Tool Enhance`
  - `publisher`: `evolution-local`
- New custom icon asset for this fork.
- Safer default chat/tool settings:
  - `lmstudio-copilot.maxTools = 8`
  - `lmstudio-copilot.maxInputTokens = 8192`
  - `lmstudio-copilot.maxOutputTokens = 4096`
  - `lmstudio-copilot.enableThinking = false`
  - `lmstudio-copilot.reasoningEffort = medium`
  - `lmstudio-copilot.terminalToolTimeout = 120000`

## Install

### Install from VSIX

1. Open VS Code.
2. Open Extensions view.
3. Click `...` (top-right in Extensions panel).
4. Click `Install from VSIX...`.
5. Select:
   - `lm-studio-tool-enhance-0.1.17-enhance.2.vsix`
6. Reload window.

### Recommended

- Disable the original marketplace extension if both are installed, to avoid confusion.
- Verify LM Studio server URL in VS Code settings:
  - `lmstudio-copilot.serverUrl` (default: `http://localhost:1234`)

## Local MCP Setup (Optional, Recommended)

If you use LM Studio MCP tools, configure them in:
- `C:\Users\Evolution\.lmstudio\mcp.json`

Typical useful local tools:
- `fetch`
- `filesystem`
- `git`
- `chrome-devtools`
- `playwright`
- `sequential-thinking`
- `memory`

## Known Notes

- This repo was prepared from an installed extension package (prebuilt `dist/`), not a full upstream source checkout.
- Packaging in this workspace uses prebuilt assets and skips prepublish compile steps.

## License

This fork keeps the upstream MIT license.
See `LICENSE.txt`.

## Attribution

This project is based on:
- `danlambiase.lmstudio-copilot-provider`
- Upstream repo: `https://github.com/yoy123/lmstudio-copilot-provider`

See `NOTICE.md` for details.
