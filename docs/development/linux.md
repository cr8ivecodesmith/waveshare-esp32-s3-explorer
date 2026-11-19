# Linux / Ubuntu development environment

> **Status:** Preliminary guidance based on vendor documentation; not yet validated on project hardware.

1. Install [Arduino IDE](https://www.arduino.cc/en/software) and the Espressif board support described in [Waveshare's Arduino guide](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Arduino). Start with the vendor's documented dependencies.
2. Connect the board with a **data-capable USB-C cable** and compare attached serial devices before and after connecting. Depending on how the firmware exposes USB, a port may appear as `/dev/ttyACM*` or another serial device.
3. If the port is present but cannot be opened, inspect device ownership and permissions (`ls -l /dev/ttyACM*` if applicable). Some distributions use the `dialout` group; verify the actual group rather than applying an unexamined system-wide fix.
4. Select **ESP32S3 Dev Module**, the correct port, and **16 MB flash**, then build and upload `04_gfx_helloworld`.
5. If the port is not recognized, consult [Waveshare's BOOT-mode instructions](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54/Instructions-For-Use).

See [getting started](../getting-started.md). Native Linux flashing is the straightforward first route; do not assume a container or special AI environment is required.
