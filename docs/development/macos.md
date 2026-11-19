# macOS development environment

> **Status:** Preliminary guidance based on vendor documentation; not yet validated on project hardware.

1. Install the [Arduino IDE](https://www.arduino.cc/en/software) and set up **ESP32 by Espressif Systems** following [Waveshare's Arduino instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino).
2. Follow the vendor's documented library versions and use **ESP32S3 Dev Module** with **16 MB flash** for its examples.
3. Connect the board using a data-capable USB-C cable. Check the IDE's port selector; if necessary, compare `ls /dev/cu.*` before and after connecting the board.
4. Build and upload `04_gfx_helloworld`, then verify the display. See [getting started](../getting-started.md) for the full learning path.
5. If no device appears, check USB cable/permissions first, then use the board's documented BOOT procedure.

Use terminal tools or an AI coding assistant if you prefer, but neither is required. Record any version-specific differences when you verify this on macOS.
