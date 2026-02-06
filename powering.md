# Powering the ESP32-S3

The ESP32-S3 requires 3.3V power supply, however you can power as follows:

**USB cable***
- You can connect with a USB cable (just plug into the jack) and the Feather will regulate the 5V USB down to 3.3V. 

- For permanent installations, a 5V 1A USB wall adapter will let you plug in a USB cable for reliable power

- When USB is plugged in it will charge the Lipoly battery.

**Power Bank**

- For mobile projects, you can use a 5V 1-2.2A USB battery bank!

**Lithium Batteries**

- You can also connect a 4.2/3.7V Lithium Polymer (LiPo/LiPoly) or Lithium Ion (LiIon) battery to the JST jack. 

- Battery current: 250mAh or larger.

CHG LED:

  - LED yellow: The battery is charging
    
  - LED off: Charging is complete, the LED will turn off.
  
  - LED blink: If there's no battery plugged in, the CHD LED may blink rapidly - this is expected!

You can add a battery monitor (MAX17048 module), read more [here](https://learn.adafruit.com/adafruit-esp32-s3-feather/pinouts)

**DONT use alkaline!**

Do not use alkaline or NiMH batteries and connect to the battery port - this will destroy the LiPoly charger


### POWER PINS

BAT - This is the positive voltage to/from the 2-pin JST jack for the optional Lipoly battery.

EN - This is the 3.3V regulator's enable pin. It's pulled up, so connect to ground to disable the 3.3V regulator. 

3.3V - These pins are the output from the 3.3V regulator, they can supply 500mA peak. It is not recommended to power the board via this 3.3V pin, instead, use it to power sensors. 

USB - When you plug in USB-C, there is 5 V available on the USB pin. You can draw up to 100mA from it, more than that will overheat the regulator. It is not recommended to power the board using this USB pin. 

GPIO pins can draw up to 20mA


