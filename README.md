# Temperature-controlled-fan
Temperature-controlled fans are essential components in modern electronic devices and systems, providing efficient thermal management to prevent overheating and ensure optimal performance and reliability. This paper presents a comprehensive study on the design, implementation, and performance evaluation of a temperature-controlled fan system. The system employs a microcontroller-based approach to monitor ambient temperature continuously and adjust fan speed accordingly. Key components include a temperature sensor for accurate measurement, a microcontroller for processing data and controlling fan speed, and a fan unit capable of variable speed operation.

The design methodology encompasses sensor selection, calibration techniques, and algorithm development for fan speed control based on temperature thresholds. Practical considerations such as power consumption, noise levels, and response time are addressed through careful component selection and tuning of control parameters. Experimental results demonstrate the effectiveness of the system in maintaining temperature within desired limits under varying load conditions
____________________________________________________________________________________________________________________________________________________________________________
**COMPONENTS**
1.Arduino UNO	
2. Temperature Sensor
3.2N2222 NPN Transistor
4.LCD(16x2)
5.DC Motor
6.Connecting Wires
7.Bread Board
8. Resistor
9. Capacitor
10.Buzzer
_____________________________________________________________________________________________________________________________________________________________________________________________________
**CIRCUIT DESIGN OF TEMPERATURE CONTROLLED FAN USING ARDUINO**
1.	LCD Display (LCD1 - LM016L)
RS (Pin 4): Connected to Arduino Pin D9 RW (Pin 5): Connected to Ground
EN (Pin 6): Connected to Arduino Pin D8 D4 (Pin 11): Connected to Arduino Pin D2 D5 (Pin 12): Connected to Arduino Pin D3 D6 (Pin 13): Connected to Arduino Pin D4 D7 (Pin 14): Connected to Arduino Pin D5

2.LM35 Temperature Sensor (U1)
VCC: Connected to +5V GND: Connected to Ground
VOUT: Connected to Arduino Analog Pin A0

3.BUZZER (BUZ1)
Positive Terminal: Connected to Arduino Pin D6 Negative Terminal: Connected to Ground

4.IRFZ44N MOSFET (Q1)
Gate: Connected to Arduino Pin D7 through R1 (10k ohm) Drain: Connected to one terminal of Fan Motor (M1) Source: Connected to Ground

5.Fan Motor (M1)
Positive Terminal: Connected to +12V through Diode (D1 - 1N4007) Negative Terminal: Connected to Drain of MOSFET (Q1)

6.Diode(D1 - 1N4007)
Anode: Connected to the negative terminal of the Fan Motor (M1)
Cathode: Connected to +12V

7.Resistors
R1 (10k ohm):Connected between Gate of MOSFET (Q1) and Arduino Pin D7
R2 (100 ohm):Connected between VDD (Pin 2)

