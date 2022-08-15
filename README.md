# Wasdom ESP32 Setup
ESP32 is a 2.4 GHz Wi-Fi/Bluetooth combo chip built on TSMC's ultra-low-power 40nm process technology. This device has been designed to provide the best power and RF performance, demonstrating robustness, versatility, and reliability in a wide variety of applications and power scenarios.

Make sure your computer has the latest version of the Arduino IDE from [here](https://www.arduino.cc/en/Main/Software) before starting the setup.

## Contents:
  - [Installing ESP32 Add-on in Arduino IDE](#installing-esp32-add-on-in-arduino-ide)
  - [Testing the Installation](#testing-the-installation)

## Installing ESP32 Add-on in Arduino IDE
To install the ESP32 board in your Arduino IDE, follow these steps:
* In your Arduino IDE, go to `File` > `Preferences`
* Enter the following into the "Additional Board Manager URLs" field:
``` 
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json 
```
Then, click the “OK” button
* Open the Boards Manager. Go to `Tools` > `Board` > `Boards Manager`
* Search for ESP32 and press install button for the "ESP32 by Espressif Systems"
And That’s it!

## Testing the Installation
Plug the ESP32 board to your computer. With your Arduino IDE open, follow these steps:
* Select your Board in `Tools` > `Board:"Arduino Uno"` > `ESP32 Arduino` > `WEMOS D1 MINI ESP32`
* Select the Port in `Tools` > `Port` > `COM3`
 
Note: if you don’t see the COM Port in your Arduino IDE, you need to install the [CP210x USB to UART Bridge VCP Drivers](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers)
* Open the following example under `File` > `Examples` > `Basics` > `Blink`
* A new sketch opens in your Arduino IDE, press the Upload button in the Arduino IDE
You should see a "Done uploading" message and the led of the ESP32 is now working 
