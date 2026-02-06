# Adafruit ESP32-S3 (8 MB Flash, no PSRAM)

### Native USB 

Its USB-C port can act like a keyboard, mouse, or disk drive, with no external USB-to-Serial converter required. Just plug it in!

### WIFI and BLE

- BLE it’s a version of Bluetooth designed to use very little power.

### Flash (8 MB)

- Flash memory is long-term storage memory. 

- It keeps its contents when power is off and is used to store:

    - Program code

    - Files (audio, images, configuration data)

### NO-PSRAM MEANING

- This board does not include external PSRAM (Pseudo-Static RAM). It only uses the ESP32-S3’s internal SRAM.
  
- Advantages:

    - Internal SRAM is much faster than PSRAM. Good for time-critical tasks such as timers, interrupts, motor control, and short audio playback.
    
    - Lower latency and more predictable behaviour.

- Disadvantages: 

    - Less total RAM available for large buffers, which affects:

        - Graphics resolution is limited.
        
        - Audio clips cannot be fully loaded into RAM (but can be streamed).
        
        - Camera projects are not suitable for this board.

### PIN OUT NOTES

- SCK - This is the SPI clock pin.

- MOSI - This is the SPI Microcontroller Out / Sensor In pin.

- MISO - This is the SPI Microcontroller In / Sensor Out pin.

- SCL - This is the I2C clock pin. There is a 5k pullup on this pin.
