# Contributing

Thanks for helping improve `LM Studio-Tool Enhance`.

## Scope

This fork focuses on:
- local model stability
- safer tool-calling defaults
- practical local development workflows

## Basic Workflow

1. Create a feature branch.
2. Make focused changes.
3. Test extension behavior in VS Code.
4. Update `CHANGELOG.md` if behavior changes.
5. Open a pull request.

## Suggested PR Checklist

- [ ] Change is local-model friendly.
- [ ] Tool-calling behavior is still safe.
- [ ] No accidental branding/license regressions.
- [ ] README/NOTICE updated when needed.

## Packaging Note

This repo currently packages from prebuilt `dist/` assets.
If you move to full source-based builds, update scripts and documentation accordingly.

## Security

Do not add default behavior that executes destructive shell commands silently.
Prefer explicit confirmation for risky operations.
