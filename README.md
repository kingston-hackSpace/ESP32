# ESP32
----

### WHAT IS THE ESP32?

The ESP32 is a powerful, low-cost microcontroller made by Espressif Systems. What characterizes it its that it comes with Wi-Fi, Bluetooth (Classic + BLE), a generous set of GPIO pins, and a rich set of peripherals. Think of it as a capable, connected microcontroller that sits in a sweet spot between simple boards like the Arduino and a Raspberry Pi.

----

### WHEN (AND WHY) TO USE AN ESP32 

Choosing the right board for your project matters. 

USE A ESP32 IF:

- You need Wi-Fi or Bluetooth (sending data to a server, phone, or cloud)

- Your project needs more processing power or memory

- You need a small but powerful microcontroller

- More specifics about the ESP32 will vary depending on the model

---
## ESP32 TYPES

At hackSpace we have the **ESP32-Feather-V2** and the **ESP32-S3 Feather**, which suit different kinds of projects:

— **ADAFRUIT ESP32 Feather V2 (8MB Flash, 2MB PSRAM):** Best for projects that need to store or move large amounts of data — like driving a screen, buffering sensor readings, or working with graphics. Its 2MB PSRAM gives it extra memory headroom that the S3 lacks. It also supports Bluetooth Classic (not just BLE), which matters if you're connecting to older Bluetooth devices like speakers or serial adapters. Best programmed using the Arduino IDE. One important note: analog sensor readings on ADC2 pins stop working once Wi-Fi is active. 

- [Adafruit ESP32 Feather V2 Tutorial](https://github.com/kingston-hackSpace/ESP32/edit/main/README.md)

---

— **Adafruit ESP32-S3 (8MB Flash, no PSRAM):** The newer chip. Best for interactive and sensor-heavy projects. Its standout feature is native USB — it can present itself to a computer as a keyboard, mouse, MIDI controller, or USB drive without any extra hardware, making it great for performance and installation work. Almost any pin can be assigned to PWM, I2C, SPI, or UART in code Adafruit, which makes wiring up motors, LEDs, and sensors more flexible. It has no DAC (so no true analog audio output), but handles NeoPixel LEDs, servos, and I2C sensors very well. It also works smoothly with CircuitPython — files can be edited directly from your file system like a USB stick Adafruit, which is a friendlier workflow for beginners.

- [Understanding FEATURES and PINOUT](https://github.com/kingston-hackSpace/ESP32/blob/main/features.md)

- [Powering the ESP32-S3](https://github.com/kingston-hackSpace/ESP32/blob/main/powering.md)

- [Set-Up your ESP32-S3](https://github.com/kingston-hackSpace/ESP32/blob/main/setup.md)

- Read more about Adafruit ESP32-S3 [here](https://learn.adafruit.com/adafruit-esp32-s3-feather)
----

⚠️ POWERING: IMPORTANT NOTE:

Both boards run at 3.3V logic — not 5V like an Arduino Uno. Most modern sensors and components are fine with this, but always check before wiring something up. GPIO pins are not 5V safe Espressif. Also, for power-hungry components like motors or large LED strips, use the USB or battery pins directly rather than drawing from the 3.3V regulator





