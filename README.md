# EMG-Sensor-with-Audiovisual-Output
You have been approached by a company who wants to build a simple device controlled by a muscle activity sensor. There is no specific requirement which muscle group you should use for your control signals. It could be either the biceps muscle (when you flex your arms), finger muscles (when you type), masseter (when you clench your teeth) or any other muscles which present an electromyogram (EMG) signal when being activated. You will work in groups and have up to one week to deliver the device. The output of your device should indicate, using either an audio, visual, and/or motion, the movement and strength of the muscle activities.

LED Bar-Graph Display
We can create an n-LED bar-graph display to act as a “muscle
strength” indicator. The n-LED will act as a thermometer display
– with no EMG activity, all LEDS will be off. Then as the EMG
activity increases in amplitude, more and more LEDs will light
up. To accomplish this, you will use the ADC on the Arduino
board to digitize the integrator’s output and convert the strictly
binary code from the ADC to a thermometer code before the
multiple-line digital output is used to drive LEDs.
Notes: 1. Always use current-limiting resistors before
connecting the Arduino’s digital output to an LED. The nominal
current through an LED should be approximately 20mA.
2. If the Arduino pin is not able to provide enough driving current
to LEDs, a buffer circuit powered by a powerful supply voltage
should be added in between the LEDs and the Arduino’s output
pins.

Dimmer LED display
We can use a single digital output line on the Arduino board to
drive a display pattern made by synchronized LEDs. With no
EMG activity, the pattern remains dark. Then as the EMG signal
increases in amplitude, the brightness of the pattern on display
increases.
Hint: use the pulse-width modulation (PWM) on the digital
output line of your Arduino board.
