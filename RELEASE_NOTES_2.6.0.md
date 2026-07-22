## AutoTrim Exporter 2.6.0

This update focuses on trimming quality and delivery safety. It also covers the changes from the unpublished 2.5.0 development cycle.

### Adaptive Silence Map (new in 2.6.0)

Trim detection is no longer a single fixed threshold. The new deterministic detector combines:

- a hard peak floor that always respects the user's start-threshold decision,
- a learned local noise floor, so stationary room tone or electronic hiss around an event is not exported as part of the asset,
- 10 ms onset energy with hysteresis, so quiet intentional material is not mistaken for silence,
- a decay-aware tail window that preserves low reverb and delay tails above the learned floor.

Constant intentional audio (drones, beds selected on purpose) is preserved even when no floor contrast exists, and per-item skip diagnostics now report the measured noise floor.

### Render safety hardening (2.5.0)

- Every export renders to a unique temporary file first; the existing delivery is replaced only after the new render is verified, and the previous version is restored automatically if the replacement fails.
- Incomplete or truncated renders are detected and never replace a delivery file.
- Trim boundaries must converge within a bounded number of analysis passes before a final render is committed; tails that keep growing stop the export at a 30-second guard instead of shipping a cut-off asset.
- Media source files currently used by the project are never overwritten — deliveries version away from them automatically.
- Cancellation and error paths restore mutes, selections, render settings, and the time selection, and each restore step is protected independently.
- The production Lua source is now exercised by an automated regression suite covering detection, selection, versioning, rollback, and cancellation behavior.

### Availability

This public preview contains product information and release notes only. No Lua source or distribution package is attached because the application source is maintained in a private repository. Licensed distribution packages will be announced separately.

### Requirements

- REAPER 7
- Windows, macOS, or Linux
- SWS Extension is optional
