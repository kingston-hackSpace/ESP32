# Set-Up your ESP32-S3

**WINDOWS WARNINIG:** The ESP32-S2/S3 bootloader does not have USB serial support for Windows 7 or 8. Please update to version 10 which is supported by espressif. Read more [here](https://learn.adafruit.com/adafruit-esp32-s3-feather/overview-2)

**ARDUINO IDE:** Arduino IDE version 1.8 or higher.

----
## Set-Up instructions

(For visual instructions see [here](https://learn.adafruit.com/adafruit-esp32-s3-feather/overview-2))

Step1

Open your Arduino IDE, open Settings and add the following URL to the Additional Boards Manager URLs

      https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json 

Step 2

Go to the Tools → Board → Board Manager submenu. Choose **esp32 by Espressif Systems**

Step 3

In the Tools → Board submenu you should see ESP32 Arduino. Select:

      Adafruit Feather ESP32-S3 No PSRAM


Select the port:

ESP32-S3 support in Arduino uses native USB which can crash. If you ever DON'T see a serial/COM port, you can always manually enter bootloading mode. This bootloader is in ROM, it is 'un-brickable' so you can always use this technique to get into the bootloader. However, after uploading your Arduino code you MUST press reset to start the sketch.
