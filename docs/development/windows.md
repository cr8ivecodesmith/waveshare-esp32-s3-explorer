# Windows setup

For your first upload, Arduino IDE on Windows provides a direct path to the USB-connected board.

1. Install [Arduino IDE](https://www.arduino.cc/en/software) and ESP32 board support following [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino).
2. Install the libraries required by the example, using Waveshare's documented versions.
3. Connect the board using a data-capable USB-C cable. Find its **COM port** in Device Manager or Arduino IDE.
4. Select **ESP32S3 Dev Module**, **16 MB flash**, the example's partition settings, and the correct COM port.
5. Build and upload `04_gfx_helloworld`. Confirm the display output.

If the port is missing, follow [Waveshare's BOOT-mode instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).

**Using WSL2?** USB devices are not automatically passed through to WSL. If you prefer building and flashing from WSL, you'll need to configure USB forwarding separately.

Continue with [Getting started](../getting-started.md).
