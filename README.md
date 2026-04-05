# Lacrima Tears of Life Releases

This is the public Windows release repository for **Lacrima Tears of Life**.

If you want to install Lacrima on Windows, this is the right place.

This repository does **not** contain the private source code for the app. It exists only to publish official Windows release files.

## What To Download

Normal users should download **only**:

- `LacrimaTearsOfLife-Setup.exe`

That is the Windows installer.

Normal users should **ignore**:

- `RELEASES`
- `*.nupkg`
- `Source code (zip)`
- `Source code (tar.gz)`

## Why Are The Other Files There?

Lacrima currently uses a Windows release format based on Squirrel.

That means each GitHub Release includes a few support files in addition to the installer:

- `LacrimaTearsOfLife-Setup.exe`
  The file a normal user should run.
- `RELEASES`
  Metadata used by the installer/update system.
- `*.nupkg`
  The packaged Lacrima app data used by the installer/update system.

You do **not** manually download those support files. They just need to exist on the release.

## Current Distribution Model

Right now the public release flow for Lacrima is:

- download `LacrimaTearsOfLife-Setup.exe`
- install the app
- launch the installed app from Windows

For this phase, think of this repository as the official Lacrima Windows download page.

## What This Repository Is For

- official Windows releases for Lacrima
- the public download page for Lacrima on Windows
- installer support files required by the current packaging format

## What This Repository Is Not For

- private source code
- gameplay design discussion
- multiplayer/server coordination
- source-level issue triage
- feature development

## Release Format

Each release is tagged like this:

- `v0.10.3`
- `v0.10.4`

Platform scope right now:

- Windows only
- stable releases only

## Unsigned Windows Warning

Lacrima Windows builds are currently **unsigned**.

That means Windows or your browser may show warnings such as:

- Microsoft Defender SmartScreen
- browser download warnings
- Windows "unknown publisher" prompts

That is expected for now. Download only from this repository's official **Releases** page.

## Support

If you need help with Lacrima installation or release downloads, use the support path documented in [SUPPORT.md](SUPPORT.md).
