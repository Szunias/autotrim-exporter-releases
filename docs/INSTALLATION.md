# Installation

These steps install the licensed AutoTrim Exporter package published through
this repository's GitHub Releases page.

## Requirements

- REAPER 7.37 or newer (64-bit)
- ReaImGui 0.10.0.5 or newer in the 0.10 API series
- ReaPack, recommended for installing ReaImGui
- SWS Extension, optional
- On macOS and Linux, an output folder whose filesystem supports hard links,
  and `/bin/ln`. Where the hard link fails (for example on FAT/exFAT or some
  network mounts) AutoTrim stops rather than risk overwriting another
  program's file; export to a supported folder and copy the assets afterwards.
  Windows has no such requirement.

## Install ReaImGui

In REAPER, open **Extensions → ReaPack → Browse packages**, search for
`ReaImGui: ReaScript binding for Dear ImGui`, install it and restart REAPER.

## Install AutoTrim Exporter

1. Download the release ZIP and matching `.sha256` checksum from GitHub
   Releases.
2. Verify the downloaded ZIP against the published checksum.
3. Extract the package.
4. Copy the complete `AutoTrim Exporter` folder into the `Scripts` directory
   inside the REAPER resource path. On Windows you can instead double-click
   `Install-Windows.cmd` in the extracted package; `INSTALL.md` in the package
   describes its options.
5. In REAPER, open **Actions → Show action list**.
6. Choose **New action → Load ReaScript** and select
   `AutoTrim Exporter/AutoTrim_Exporter.lua`.

Open the resource path from **Options → Show REAPER resource path in
Explorer/Finder**.

Do not copy the launcher by itself. The UI, rendering engine and fonts must
remain in their supplied folder structure.
