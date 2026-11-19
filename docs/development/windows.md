# Windows development environment

> **Status:** Preliminary guidance based on vendor documentation; not yet validated on project hardware.

For a first experiment, **use native Windows Arduino tooling and direct USB flashing**. WSL2 is optional and can be introduced later if you prefer its terminal environment.

1. Install the [Arduino IDE for Windows](https://www.arduino.cc/en/software) and the Espressif ESP32 board support described in [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino).
2. Install the libraries required by the **ESP32-S3-Touch-LCD-1.54** vendor example; keep its documented versions initially.
3. Connect the board with a **data-capable USB-C cable** and look for the corresponding **COM port** in Device Manager and the Arduino IDE.
4. Select **ESP32S3 Dev Module**, **16 MB flash**, and the appropriate COM port. Build and upload `04_gfx_helloworld` and verify what appears on the display.
5. If the port cannot be detected, follow the [manufacturer's BOOT-mode procedure](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).

**WSL2 note:** Working with source files under WSL does not automatically make the board's USB device available inside WSL. USB forwarding requires additional Windows/WSL configuration. For the initial project, avoid that complexity unless you specifically want to learn it.

See the shared [getting-started guide](../getting-started.md). Any AI coding assistant is optional.
