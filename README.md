# Adafruit BME280 Library [![Build Status](https://travis-ci.com/adafruit/Adafruit_BME280_Library.svg?branch=master)](https://travis-ci.com/adafruit/Adafruit_BME280_Library)

## Fork for ESP32 by TvE

- `begin` no longer calls `Wire.begin` so the application can call that itself and thereby specify
  which pins it wants to use.
- `_wire->endTransmission` uses `false` to allow the transction to continue, which is a requirement
  for the ESP32's I2C library to work correctly.

## Original README

<a href="http://www.adafruit.com/products/2652"><img src="./assets/board.jpg" width="500"/></a>

This is a library for the Adafruit BME280 Humidity, Barometric Pressure + Temp sensor

Designed specifically to work with the Adafruit BME280 Breakout 
 * http://www.adafruit.com/products/2652

These sensors use I2C or SPI to communicate, up to 4 pins are required to interface

Use of this library also requires [Adafruit_Sensor](https://github.com/adafruit/Adafruit_Sensor)
to be installed on your local system.

Adafruit invests time and resources providing this open source code, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!

Check out the links above for our tutorials and wiring diagrams 

Written by Limor Fried/Ladyada for Adafruit Industries.  
BSD license, all text above must be included in any redistribution

To download. click the DOWNLOAD ZIP button, rename the uncompressed folder Adafruit_BME280. 
Check that the Adafruit_BME280 folder contains Adafruit_BME280.cpp and Adafruit_BME280.h

Place the Adafruit_BME280 library folder your arduinosketchfolder/libraries/ folder. 
You may need to create the libraries subfolder if its your first library. Restart the IDE.

We also have a great tutorial on Arduino library installation at:
http://learn.adafruit.com/adafruit-all-about-arduino-libraries-install-use
