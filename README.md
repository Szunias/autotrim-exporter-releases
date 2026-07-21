# AutoTrim Exporter

<p align="center">
  <strong>A focused sound-design export workflow for REAPER.</strong><br>
  Select the layers. Frame the sound. Deliver verified WAV assets.
</p>

<p align="center">
  <img alt="Version 2.4.0" src="https://img.shields.io/badge/version-2.4.0-5b6ee1">
  <img alt="REAPER" src="https://img.shields.io/badge/DAW-REAPER-d9a441">
  <img alt="Proprietary license" src="https://img.shields.io/badge/license-proprietary-6b7280">
</p>

---

AutoTrim Exporter brings the repetitive parts of sound-asset delivery into one clear REAPER workflow. It collects layered material across tracks, detects useful audio, preserves tails, prepares levels, handles naming and versioning, and verifies every WAV before it becomes a delivery file.

This repository is the public home for product information, release notes, and distribution updates. The application source is maintained privately.

## Built for sound-design sessions

Sound effects rarely live on one clean track. A finished asset may combine impacts, debris, sweeteners, sub layers, reverbs, and tails — with long ambience or temporary material sitting nearby. AutoTrim Exporter helps isolate the intended event without turning export preparation into another editing session.

## Highlights

- **Select across tracks** from a single timeline anchor.
- **Ignore unrelated long items** while keeping explicitly selected source material.
- **Automatically frame the result** horizontally and vertically in REAPER.
- **Detect useful audio** with independent start and tail thresholds.
- **Preserve transients and tails** with adjustable padding and extra-tail controls.
- **Render one layered asset or one file per item.**
- **Normalize by LUFS-I, RMS, Peak, or True Peak** with a true-peak ceiling.
- **Work through naming lists** for variations and production batches.
- **Create safe incremental versions** or deliberately replace an existing delivery.
- **Verify temporary renders before committing files** to the destination folder.
- **Review export history and diagnostics** from a dedicated Results tab.

## The workflow

1. Select the item that anchors the sound event.
2. Run **Select across tracks** to collect the matching layers.
3. Review the automatically fitted arrange view.
4. Choose delivery, trimming, naming, and level settings.
5. Export verified WAV assets.

## Requirements

- REAPER 7
- Windows, macOS, or Linux
- SWS Extension is optional

## Availability

AutoTrim Exporter is currently in private product development. Public release notes are available from the [Releases](../../releases) page. Licensed distribution packages will be announced here when available.

## Source and licensing

AutoTrim Exporter is proprietary software. The source repository is private, and no source-code license is granted through this public release hub. See [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Copyright © 2026 Szunias. All rights reserved.</sub>
</p>
