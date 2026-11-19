# Getting started

**Goal:** Make one visible change on the Waveshare ESP32-S3-Touch-LCD-1.54. This guide is a first path, not a required course.

> **Status:** Documentation-level starting point. The commands, dependencies, and flashing sequence have not yet been validated on the six physical devices associated with this project. Follow the official guidance if anything here differs.

## 1. Identify and inspect the board

Check that yours is the **ESP32-S3-Touch-LCD-1.54** (with touch), not the otherwise similarly named LCD-only variant.

- [Hardware overview](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54)
- [Official user guide and assembly precautions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use)
- [Firmware resources](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Resources-And-Documents)

If your kit includes a battery that needs installation, follow Waveshare's assembly instructions and use the provided insulating sheet. Use a **data-capable USB-C cable** for programming. A microSD card is not necessary for the first display example.

Before flashing anything, inspect the factory application and locate Waveshare's factory firmware and restoration instructions. Flashing a sketch will replace the application currently on the device.

## 2. Prepare a development environment

Select the notes for your operating system:

- [macOS](development/macos.md)
- [Linux / Ubuntu](development/linux.md)
- [Windows](development/windows.md)

Waveshare documents two programming routes: [Arduino](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino) and [ESP-IDF](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/ESP-IDF). The initial path below uses **Arduino** because it has a small display-oriented example. You can choose a different toolchain.

## 3. Reproduce a manufacturer's example

In [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino):

1. Install Arduino IDE and the Espressif ESP32 board support as directed. Waveshare currently documents the **ESP32 by Espressif Systems 3.2.0** package for these examples.
2. Obtain the **ESP32-S3-Touch-LCD-1.54** example package and its required libraries. Use the vendor-documented versions first rather than replacing all dependencies with the newest ones.
3. In Arduino IDE, select **ESP32S3 Dev Module**, the connected USB port, and **16 MB flash**. Choose the partition layout required by the example.
4. Open the vendor example named **`04_gfx_helloworld`** (under `Arduino/examples`), build it, and upload it using the manufacturer's instructions.
5. Confirm that the screen displays the expected output. Record your OS, tool versions, USB port, compile/upload results, and any workaround needed.

If the USB port is missing, Waveshare documents holding **BOOT** while connecting USB, then releasing it to enter download mode. After uploading, power-cycle the board. Do not erase flash just to troubleshoot a missing port.

## 4. Make a small modification

Change one clearly visible detail: text, positioning, foreground color, or background color. Rebuild and reflash; compare actual behavior with your expectation.

Before experimenting with more peripherals, try explaining the example's setup and draw calls in your own words (or ask a coding assistant to walk through them).

## 5. Explore further

Browse [project ideas](project-ideas.md) for motion-, touch-, audio-, and Wi-Fi-based directions. Some ideas are purely proposed; do not assume a completed example exists in this repository.

## Troubleshooting and recovery

Use [Waveshare's user guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use) for bootloader behavior and vendor firmware restoration. Confirm you have the correct firmware image **and flash address** for your exact model before restoring. Current project maintainers have not verified a cross-platform recovery workflow; document successful recoveries when available.

For help, report your board model, OS, toolchain/version, USB port (without private machine identifiers), sample name, error, and what you already tried.
