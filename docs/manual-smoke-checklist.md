# Manual Smoke Checklist

Use this checklist for each shipped Windows version before or immediately after publishing the stable release.

## Installation

- Confirm the installer `.exe` downloads from the GitHub Release page.
- Run the installer and verify installation completes without an unexpected hard failure.

## First Launch

- Launch the installed app.
- Confirm the splash or loading screen appears.
- Confirm the main window opens successfully.

## Update Path

- In the installed app, use `Help -> Check for Updates`.
- Confirm the update check completes against this repository's release feed.
- Test updating from an older installed version to the newly published release.
- Confirm the app launches successfully after the update.

## Release Asset Sanity

- Confirm the GitHub Release contains the installer `.exe`.
- Confirm the GitHub Release contains `RELEASES`.
- Confirm the GitHub Release contains the matching `*-full.nupkg`.
- If a delta package was generated, confirm it is attached and named consistently.

## Public Download Sanity

- Confirm the release is tagged with `vX.Y.Z`.
- Confirm the release notes and asset list are visible on the public Releases page.
- Confirm any unsigned-build warning note is still accurate for the current distribution state.
