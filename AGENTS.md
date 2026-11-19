# Project guidance

Waveshare ESP32-S3 Explorer is a collection of approachable experiments for the **Waveshare ESP32-S3-Touch-LCD-1.54** touchscreen board.

## Before working

- Read `README.md` and the relevant guide under `docs/`.
- Use the [Waveshare board documentation](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54) and its [Arduino](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino) or [ESP-IDF](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/ESP-IDF) examples. Confirm the board variant, pin assignments, and peripheral setup.
- Inspect existing code and configuration before changing them.

## Developing examples

- Start with a small working example. The initial display exercise uses Waveshare's `04_gfx_helloworld`.
- Prefer readable, incremental changes that people can understand and build upon.
- Record toolchain and library versions needed to reproduce a build.
- Distinguish what was compiled from what was tested on a physical board. Include steps to verify behavior.
- Document how to restore or recover firmware when applicable. Confirm the board and flash settings before uploading.
- Keep setup guides usable on macOS, Linux, and Windows.
- Keep the project independent of any particular AI coding assistant.

## Local context

If `AGENTS.local.md` exists, consult it for relevant machine-specific instructions. It is optional, ignored by Git, and may need to be opened explicitly in some tools.

This repository is public. Keep private URLs, credentials, local infrastructure details, and workplace material out of committed files and shared outputs. Never store secrets in agent instructions.

## Working style

Explain unfamiliar hardware decisions and test assumptions against documentation or observed behavior. When something fails, report what was tried and what happened. Ask before destructive operations, erasing flash, or changing system-wide configuration.
