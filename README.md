# Waveshare ESP32-S3 Explorer

A small, open-ended playground for the [Waveshare ESP32-S3-Touch-LCD-1.54](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54). Start with a working example, change something you can see or hear, and explore what this pocket-sized device can do.

The project began as an invitation for people with different programming backgrounds to try hardware projects. Anyone can use the materials, with or without an AI coding assistant. There is no prescribed challenge or requirement to complete anything.

## Hardware

The **touchscreen variant** combines a 240 × 240 LCD, capacitive touch, Wi-Fi, Bluetooth LE, microphones, speaker, motion sensor, and buttons. A microSD card is optional for basic experimentation. Confirm details against [Waveshare's board documentation](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54); examples for similarly named *non-touch* boards are not interchangeable.

## Start here

1. Read the [getting-started guide](docs/getting-started.md) and the [official user guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).
2. Choose your [development environment](docs/development/) (macOS, Linux, or Windows).
3. Reproduce Waveshare's `04_gfx_helloworld` example, then modify one visible detail.
4. Browse the [project ideas](docs/project-ideas.md) or invent your own.

Waveshare supports both [Arduino](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino) and [ESP-IDF](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/ESP-IDF). Arduino examples are the suggested first route, not a required framework.

## What is here today?

**Early documentation scaffold only.** No original firmware example, reproducible automated build, or tested cross-platform flash workflow has been added to this repository yet. The first hardware-validation task is to reproduce a vendor example, record its dependencies, then publish a minimal working example.

- [Getting started](docs/getting-started.md)
- [Development environments](docs/development/)
- [Project inspiration](docs/project-ideas.md)
- [Example status](examples/README.md)

## AI assistance is optional

Use any coding assistant, or none. The repository includes portable [agent guidance](AGENTS.md), but does **not** require OpenCode, Codex, or another harness. If you use an agent, have it read the board's official documentation, explain the example you chose, and verify every board-specific assumption before flashing.

Private local work context belongs in the optional, ignored `AGENTS.local.md` file. See [the example](AGENTS.local.example.md). Never publish personal or internal infrastructure URLs, secrets, or workplace-specific data here.

## Contributing

Small, reproducible experiments and corrections to platform guidance are welcome. Describe the board variant, operating system, framework/library versions, actual hardware test performed, and recovery procedure where relevant. Clearly label untested suggestions.

Upstream examples and dependencies belong to their respective authors; link to them instead of copying their source or binaries without reviewing licenses.

## License

Original code and documentation in this repository are licensed under the [Apache License, Version 2.0](LICENSE), unless otherwise noted. Third-party libraries, examples, firmware, and other materials retain their respective licenses; this project's Apache-2.0 license does not relicense them.

