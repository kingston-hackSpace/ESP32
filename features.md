# Adafruit ESP32-S3 (8 MB Flash, no PSRAM)

### Native USB 

Its USB-C port can act like a keyboard, mouse, or disk drive, with no external USB-to-Serial converter required. Just plug it in!

### WIFI and BLE

- BLE it’s a version of Bluetooth designed to use very little power.

- ADC1 pins are safer for reliable analog readings when Wi-Fi or BLE is active.
  
  - D5, D6, D9 and D10 are on ADC1.

  - A5 is on ADC1.
  
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
     
### ANALOG READINGS/WRITINGS - ADC

ADC = Analog-to-Digital Converter
DAC = Digital-to-Analog Converter

READING via ADC
- A0-A5. Analog inputs via ADC.

- D5-D6, D9-D13. 
      
  - D5, D6, D9 and D10 are on ADC1.

  - D11-D13 are on ADC2.

DIGITAL WRITING ONLY

Adafruit's ESP32-S3 does not have a DAC, so you cannot do true analog out.

All digital pins can perform PWM, and any digital pin can be used for inputs or outputs.

## COMMUNICATION PROTOCOLS

The ESP32-S3 offer several communication protocols, which can be used in parallel, allowing you to connect a variety of devices and expand your project possibilities.

### SPI (high-speed) pins:

Ideal for high-speed data transfer, such as for LED matrix displays, SD card modules, audio devices

- SCK : This is the SPI clock pin.

- MOSI : data Out

- MISO : data In

### I2C pins (also STEMMA CONNECTOR):

Use I2C pins when you want to connect multiple devices (sensors, displays, RTCs, etc.) using only two wires: SDA (data) and SCL (clock).
(It is slower than SPI). 

- SCL : This is the I2C clock pin.

- SDA : This is the I2C data pin.
  

### UART pins:

Useful for talking to another microcontroller, GPS module, Bluetooth module, or serial device.

RX : receive (connect to TX on sensor/device)

TX : transmit (connect to RX on sensor/device)




