# Linux / Ubuntu setup

1. Install [Arduino IDE](https://www.arduino.cc/en/software) and ESP32 board support following [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino).
2. Install the libraries required by the example, using Waveshare's documented versions.
3. Connect the board using a data-capable USB-C cable. Check which serial device appears (often `/dev/ttyACM*`).
4. If the serial device is present but cannot be opened, inspect its permissions with `ls -l` and check whether your user belongs to the required group (often `dialout`).
5. Select **ESP32S3 Dev Module**, **16 MB flash**, the example's partition settings, and the serial port.
6. Build and upload `04_gfx_helloworld`. Confirm the display output.

For connection or download-mode problems, see [Waveshare's instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).

Continue with [Getting started](../getting-started.md).
