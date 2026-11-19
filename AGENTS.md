# Agent guidance — Waveshare ESP32-S3 Explorer

These instructions describe the **public project**, regardless of which AI assistant or development environment is used. Human contributors can follow them too.

## Purpose and scope

Help people with varied experience experiment with the **Waveshare ESP32-S3-Touch-LCD-1.54 (touchscreen variant)**. Prefer one understandable, observable change to a large generated application. The repository must remain usable without AI tooling.

## Before proposing code

1. Read `README.md` and the relevant page under `docs/`.
2. Check the manufacturer's [board documentation](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54), [Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino), or [ESP-IDF guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/ESP-IDF) for the **exact** board variant.
3. Inspect any current project source and configuration before changing it. Do not assume example code or libraries from a similarly named device are compatible.
4. Identify whether instructions or claims are documented, proposed, compiled, or actually verified on hardware. Do not label a build or flash as successful without evidence.

## Development conventions

- Prefer the manufacturer's smallest relevant example as a starting point. For the initial display exercise, that is `04_gfx_helloworld` in Waveshare's Arduino example bundle.
- State and, when possible, pin toolchain and dependency versions. Avoid indiscriminate upgrades that break vendor examples.
- Keep changes small enough to inspect; explain unfamiliar APIs, pin assignments, memory settings, and peripheral initialization when relevant.
- Support macOS, Linux, and Windows documentation. Treat WSL2 and USB forwarding as optional, not mandatory.
- Include instructions for verifying a change and recovering/returning to a known firmware state when modifying flash.
- Do not assume a microSD card or other additional hardware is present.
- Do not add AI-harness-specific config files or make an AI assistant a build dependency.
- Respect upstream licenses; prefer links over unreviewed copying of vendor code or firmware.

## Public/private boundary

This is a public repository. Do not commit secrets, private network addresses, internal trackers, personal machine paths, workplace source material, or service-specific credentials. Before proposing a public commit, review files, logs, generated output, and commit messages for inadvertent disclosure.

An optional `AGENTS.local.md` may provide **local-only** context. If present and accessible, read it after this file when it is relevant; if it is absent or cannot be loaded by the current harness, proceed with this public guidance. `AGENTS.local.md` is intentionally ignored by Git. Its existence does not permit copying its contents into public files, issues, tool output, or commits. Never treat a Git ignore rule as a security boundary, and avoid placing actual secrets in agent-readable notes.

## Collaboration

When a decision depends on hardware, report the exact observed behavior and unresolved assumptions. Suggest a bounded test before adding abstraction or complexity. Ask before destructive operations, changing machine-wide configuration, erasing flash, or publishing material. Preserve contributors' ability to understand and modify their own programs.
