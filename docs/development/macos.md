# macOS setup

1. Install [Arduino IDE](https://www.arduino.cc/en/software) and the ESP32 board package following [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino).
2. Install the libraries required by the example, using Waveshare's documented versions.
3. Connect the board using a data-capable USB-C cable. Select its port in Arduino IDE. If needed, compare `ls /dev/cu.*` before and after connecting it.
4. Select **ESP32S3 Dev Module**, **16 MB flash**, and the example's partition settings.
5. Build and upload `04_gfx_helloworld`. Confirm the display output.

If the port is missing, check the cable and use [Waveshare's BOOT-mode instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).

Continue with [Getting started](../getting-started.md).
