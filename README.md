# AutoTrim Exporter

<p align="center">
  <strong>A focused sound-design export workflow for REAPER.</strong><br>
  Select the layers. Frame the sound. Deliver verified audio assets.
</p>

<p align="center">
  <img alt="Latest release 3.11.0" src="https://img.shields.io/badge/release-3.11.0-55c58a">
  <img alt="REAPER" src="https://img.shields.io/badge/DAW-REAPER-d9a441">
  <img alt="Proprietary license" src="https://img.shields.io/badge/license-proprietary-6b7280">
</p>

---

AutoTrim Exporter brings the repetitive parts of sound-asset delivery into one clear REAPER workflow. It collects layered material across tracks, detects useful audio, preserves tails, prepares levels, handles naming and versioning, and verifies every file before it becomes a delivery.

This repository is the public home for product information, release notes, and distribution updates. The application source is maintained privately.

## Built for sound-design sessions

Sound effects rarely live on one clean track. A finished asset may combine impacts, debris, sweeteners, sub layers, reverbs, and tails — with long ambience or temporary material sitting nearby. AutoTrim Exporter helps isolate the intended event without turning export preparation into another editing session.

## Highlights

- **Select overlapping layers** across tracks from a single timeline anchor (`V`).
- **Ignore unrelated long items and muted material** while keeping explicitly selected source material.
- **Automatically frame the result** horizontally and vertically in REAPER.
- **Detect useful audio** with Smart trim, which learns each recording's own gates, or with independent start and tail thresholds.
- **Preserve transients and tails** with adjustable padding and extra-tail controls.
- **Or skip trimming completely** and deliver the selection exactly as it sits.
- **Render one layered asset, one file per item, or a queue** of groups marked with `Q` and numbered `Name_01`, `Name_02`, `Name_03` in one export.
- **Inspect every queued group** on the Groups page, give it its own name or variant tag, and save the queue in the project for later revisions.
- **Preview the delivery before rendering**: a dry-run delivery sheet lists every filename with its predicted bounds, and A/B audition compares an item with its trimmed window.
- **Name files to UCS 8.2.1** and embed the metadata librarians read.
- **Deliver against a profile** for Wwise, Unreal, EBU R128, Netflix and more.
- **Get a per-batch delivery report** with a verdict for every file, plus a JSON manifest for middleware hand-off.
- **Deliver WAV, FLAC, OGG, or MP3** while keeping analysis lossless.
- **Normalize by LUFS-I, RMS, Peak, or True Peak** with a true-peak ceiling.
- **Work through naming lists** for variations and production batches.
- **Create safe incremental versions** or deliberately replace an existing delivery.
- **Verify temporary renders before committing files** to the destination folder.
- **Review export history** on the History page, and audition deliveries in REAPER's Media Explorer.

## The workflow

1. Select the item that anchors the sound event.
2. Press **Select overlapping** (`V`) to collect its layers across tracks.
3. Review the automatically fitted arrange view.
4. For a batch of variations, press `Q` to queue each sound as a group, and check them on the Groups page.
5. Choose trimming (Smart, manual or none), naming, level and format settings, then preview the delivery sheet.
6. Export verified WAV, FLAC, OGG, or MP3 assets and audition them in REAPER's Media Explorer.

## Requirements

- REAPER 7.37 or newer (64-bit)
- ReaImGui 0.10.0.5 or newer in the 0.10 API series
- ReaPack is recommended for installing ReaImGui
- Windows, macOS, or Linux
- On macOS and Linux, an export folder on a filesystem with hard-link support
  (FAT/exFAT volumes and some network mounts do not qualify)
- SWS Extension is optional

See the [installation guide](docs/INSTALLATION.md) for the complete package
layout and setup process.

## Availability

AutoTrim Exporter 3.11.0 is the current stable release. It is the first public
release since 3.4.4 and includes every change from the unpublished 3.4.5–3.10.0
builds.

- [Download AutoTrim Exporter 3.11.0](https://github.com/Szunias/autotrim-exporter-releases/releases/download/v3.11.0/AutoTrim-Exporter-3.11.0.zip)
- [Download the SHA-256 checksum](https://github.com/Szunias/autotrim-exporter-releases/releases/download/v3.11.0/AutoTrim-Exporter-3.11.0.zip.sha256)
- [Read the complete release notes](https://github.com/Szunias/autotrim-exporter-releases/releases/tag/v3.11.0)

Installation and upgrade instructions are included in the package. Historical
release notes are available under [releases](releases/).

## Source and licensing

AutoTrim Exporter is proprietary software. The source repository is private, and no source-code license is granted through this public release hub. See [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Copyright © 2026 Szunias. All rights reserved.</sub>
</p>
