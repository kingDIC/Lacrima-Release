# Release Policy

This repository is the public Windows release endpoint for **Lacrima Tears of Life**.

It exists to host release artifacts for the stable channel and to provide the asset layout required by the Electron Forge + Squirrel.Windows update flow.

## Tag Format

All shipped releases should use Git tags in this format:

`vX.Y.Z`

Examples:

- `v1.0.0`
- `v1.2.3`

## Stable Channel Only

This repository is for the **stable** release channel only.

Pre-release, preview, experimental, multiplayer-related, or internal distribution channels are out of scope unless the repository policy is intentionally revised later.

## Required Asset Contract

Every shipped Windows release must include:

- installer `.exe`
- `RELEASES`
- `*-full.nupkg`

Optional:

- delta `.nupkg` if generated

If a version is published for end users, these required assets should be attached to the GitHub Release together.

## Update Safety Rules

The Electron app uses this repository's release assets for Windows auto-updates.

Because of that:

- do not delete required assets from an already-published release
- do not replace assets in place after clients may already reference them
- do not rename the repository owner or repository name casually once clients are installed

Changing or removing published update artifacts can break update detection or update delivery for existing installations.

## Operational Intent

This repository should remain a clean public distribution counterpart only.

It should not become:

- a source mirror
- a private development dump
- a backlog for source-level bug reports
- a general-purpose project management repository
