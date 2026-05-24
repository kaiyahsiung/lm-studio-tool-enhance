# Changelog

## 0.1.17-enhance.2 - 2026-05-24

- Renamed extension identity to `LM Studio-Tool Enhance`.
- Updated extension package metadata:
  - `name`: `lm-studio-tool-enhance`
  - `publisher`: `evolution-local`
  - `displayName`: `LM Studio-Tool Enhance`
- Replaced icon with custom fork icon asset.
- Kept hardened local-default behavior:
  - `maxTools = 8`
  - `maxInputTokens = 8192`
  - `maxOutputTokens = 4096`
  - `enableThinking = false`
  - `reasoningEffort = medium`
  - `terminalToolTimeout = 120000`
- Packaged VSIX:
  - `lm-studio-tool-enhance-0.1.17-enhance.2.vsix`

## 0.1.17-hardened.1 - 2026-05-24

- Initial hardened fork from installed upstream extension.
- Introduced safer defaults for local model stability.
- Created first hardened VSIX package.
