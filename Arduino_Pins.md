# Connection between Arduino pins and sensor/actuator pins

1. Analog Joystick Module:
   - VCC pin is connected to the 5V pin on Arduino.
   - GND pin is connected to the GND pin on Arduino.
   - VRx pin (X axis) is connected to the analog A0 pin on Arduino.
   - VRy pin (Y axis) is connected to the analog A1 pin on Arduino.
   - SW pin (switch) is connected to the digital 4 pin on Arduino.

2. SSD1306 OLED Display 1.3 Inch:
   - Vin pin is connected to the 5V pin on Arduino.
   - GND pin is connected to the GND pin on Arduino.
   - SDA pin is connected to the analog A2 pin on Arduino.
   - SCL pin is connected to the analog A3 pin on Arduino.

3. DRV8825:
   - DIR pin (Direction) is connected to the digital 2 pin on Arduino.
   - STEP pin is connected to the digital 3 pin on Arduino.
   - VMOT pin is connected to the Input pin 7805 VOLTAGE REGULATOR and Capacitor 100µF.
   - GND MOT pin is connected to the GND pin 7805 VOLTAGE REGULATOR and Capacitor 100µF.
   - GND Logic pin is connected to the GND pin on Arduino and Capacitor 10µF.
   - RST pin and SLP pin are connected together and connected to the Capacitor 10µF. 
   - A1, A2, B1, and B2 pins are connected to the stepper motor wires.

4. NEMA 17 Stepper Motor:
   - Motor wires are connected to the A1, A2, B1, and B2 pins on DRV8825.

5. 7805 VOLTAGE REGULATOR
   - Input pin is connected to the Sleeve pin Jack Connector and Positive pin Battery.
   - GND pin is connected to the Tip pin Jack Connector and Negative pin Battery.
   - Output pin is connected to the 5V pin on Arduino and RST, SLP pin DRV8825.
