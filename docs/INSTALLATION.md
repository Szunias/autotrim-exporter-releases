# Installation

AutoTrim Exporter is not publicly distributed yet. These steps describe the
installation flow that will accompany the first licensed release.

## Requirements

- REAPER 7 (64-bit)
- ReaImGui 0.10.0.5 or newer in the 0.10 API series
- ReaPack, recommended for installing ReaImGui
- SWS Extension, optional

## Install ReaImGui

In REAPER, open **Extensions → ReaPack → Browse packages**, search for
`ReaImGui: ReaScript binding for Dear ImGui`, install it and restart REAPER.

## Install AutoTrim Exporter

1. Download the release ZIP and matching `.sha256` checksum from GitHub
   Releases.
2. Verify the downloaded ZIP against the published checksum.
3. Extract the package.
4. Copy the complete `AutoTrim Exporter` folder into the `Scripts` directory
   inside the REAPER resource path. Windows packages also include an optional
   installer script.
5. In REAPER, open **Actions → Show action list**.
6. Choose **New action → Load ReaScript** and select
   `AutoTrim Exporter/AutoTrim_Exporter.lua`.

Open the resource path from **Options → Show REAPER resource path in
Explorer/Finder**.

Do not copy the launcher by itself. The UI, rendering engine and fonts must
remain in their supplied folder structure.
