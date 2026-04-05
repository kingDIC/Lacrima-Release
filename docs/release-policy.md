# Release Policy

This repository is the public Windows release endpoint for **Lacrima Tears of Life**.

It is intentionally narrow in scope: this repo exists to ship official Lacrima Windows builds, not to mirror development.

## User-Facing Rule

For every public release, the only file a normal Lacrima user should be told to download is:

-   `LacrimaTearsOfLife-Setup.exe`

The other release assets exist because of the current Windows packaging format and should not be presented as normal-user downloads.

## Required Release Assets

Every public Lacrima Windows release should include:

-   `LacrimaTearsOfLife-Setup.exe`
-   `RELEASES`
-   `LacrimaTearsOfLife-X.Y.Z-full.nupkg`

Optional:

-   `LacrimaTearsOfLife-X.Y.Z-delta.nupkg` if generated

## Why These Assets Exist

Lacrima currently uses a Squirrel-based Windows release layout.

That means:

-   `Setup.exe` is the real installer for players
-   `RELEASES` and `.nupkg` are support assets for the installer/update system
-   users should not be told to manually download `RELEASES` or `.nupkg`

## Tag Format

All shipped releases should use this tag format:

-   `vX.Y.Z`

Examples:

-   `v0.10.3`
-   `v0.10.4`

## Stable Channel Only

This repository is for Lacrima's **stable Windows channel** only.

No source snapshots, internal builds, multiplayer test builds, or private experiments should be treated as official releases here.

## Update Safety Rules

Even though the current user messaging is manual-download-first, the release asset set still needs to stay intact.

Because of that:

-   do not delete required assets from published releases
-   do not casually replace published assets in place
-   do not rename the repository owner or repository name casually

## Operational Boundary

This repository should stay:

-   a Lacrima Windows download repo
-   a release-history repo
-   a place for release-facing documentation only

This repository should not become:

-   a source mirror
-   a feature-planning repo
-   a gameplay discussion board
-   a source-level bug backlog