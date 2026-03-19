# esp32-space-drop
Space Drop Game (by Chad Kapper) ported to ESP32

![breadboard](images/esp32_space_drop_breadboard-sm.png)

## Hardware Setup

- ESP32S3 or similar XIAO board
- SH1106 type OLED connected to SDA,SCL
- buttonPin1 D7 (button should connect to GND when pressed, add a 10k pullup)
- 10k pot A0 (connect wiper of pot to A0, other two pins to GND and VCC)
- buzzer/speaker D8 (connect with a series resistor around 100-220ohm)

## Software Setup

Add the sketch to your Arduino IDE.

You may need to add the following libraries:

- Adafruit_GFX_Library
- Adafruit_SH110x

Also, you may need to add the board profile for your particular board.
The ESP32S3 board needs this library:
- esp32 (by Espressif Systems, I installed v3.3.6)
