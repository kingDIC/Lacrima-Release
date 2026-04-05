# Manual Smoke Checklist

Use this checklist for each new **Lacrima Tears of Life** Windows release.

## Release Page

- Confirm the new GitHub Release is tagged correctly, for example `v0.10.3`.
- Confirm the release notes clearly say normal users should download `LacrimaTearsOfLife-Setup.exe` only.
- Confirm `LacrimaTearsOfLife-Setup.exe` is attached.
- Confirm `RELEASES` is attached.
- Confirm the matching `*-full.nupkg` is attached.

## Install Flow

- Download `LacrimaTearsOfLife-Setup.exe` from the public Releases page.
- Run the installer.
- Confirm installation completes without an unexpected hard failure.

## First Launch

- Launch the installed Lacrima app.
- Confirm the loading screen appears.
- Confirm the main window opens.
- Confirm the app reaches the normal Lacrima shell instead of closing immediately.

## Basic Lacrima Checks

- Confirm card data loads.
- Confirm the main app shell is responsive.
- Confirm one or two core views open normally, such as rules or field.

## Current Rollout Note

Lacrima is currently manual-download-first.

That means this checklist should focus on:

- installer download
- installation success
- first launch success
- core app usability

Do not rely on in-app update checks as the primary release gate for this phase.
