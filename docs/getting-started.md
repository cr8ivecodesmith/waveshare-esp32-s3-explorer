# Getting started

Start by flashing a working display example, then change something you can see.

These steps follow [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino); platform-specific details are still being tested.

## 1. Check your board

Use the **ESP32-S3-Touch-LCD-1.54** touchscreen model. The similarly named LCD-only board uses different examples.

- [Board overview](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54)
- [Assembly and usage instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use)
- [Firmware downloads](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Resources-And-Documents)

If installing the included battery, use the insulating sheet as directed by Waveshare. Have a **data-capable USB-C cable** ready. You don't need a microSD card for the display example.

Explore the factory application before uploading a sketch: flashing replaces the currently installed application. Save the factory firmware download and recovery instructions for later.

## 2. Set up your computer

Choose your operating system:

- [macOS](development/macos.md)
- [Linux / Ubuntu](development/linux.md)
- [Windows](development/windows.md)

Arduino is the starting route here; you can also develop with [ESP-IDF](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/ESP-IDF).

## 3. Build and flash Hello World

Follow the [manufacturer's Arduino setup](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino):

1. Install Arduino IDE and ESP32 board support. Start with the vendor-documented **ESP32 by Espressif Systems 3.2.0** package.
2. Download the board's Arduino example package and required libraries, using the documented versions.
3. Select **ESP32S3 Dev Module**, **16 MB flash**, the correct partition scheme for the example, and your board's USB port.
4. Open `Arduino/examples/04_gfx_helloworld`, compile, and upload.
5. Confirm the result on the screen.

If the port doesn't appear, follow Waveshare's BOOT/download-mode instructions. A fresh USB connection or power cycle may be needed after uploading.

## 4. Change one thing

Edit the displayed text, color, or position. Rebuild and upload, then check whether the result matches your expectation.

Want to understand how it works? Trace the initialization and drawing calls, or ask a coding assistant to explain them.

## What's next?

Try a [project idea](project-ideas.md), or build on another official example.

For firmware recovery, use [Waveshare's instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use) and the firmware image and flash address for your exact model. If you run into trouble, note your OS, board model, tool versions, example name, and error message.
