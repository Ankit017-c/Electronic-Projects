2)__Automated water motor with level indicator__
This project is based on reflection of echo. JSN-SR04 or a Water Proof ultra-sonic sensor is an electronic device that works on the 
principle of transmission and reflection. This sensor has two pins named as TRIG and ECHO pin. The echo pin emits the waves. 
These waves travel through the medium as a wave and reflects back whenever it hits an object or an obstacle ahead of its propagation.
The time taken for the emission and reflection is calculated and using this value they calculated the water level. Thus, Arduino is 
coded accordingly. An LCD screen is used to display the information.

3)	Cell Phone tracking system__
(Using schottky diodes)
__Schottky diodes__ are special diodes formed by combining N type semiconductor material with a metal and are typically low noise diodes,
operating at a high frequency. These diodes have a unique property of conducting at a very low forward voltage between 0.15 to 0.45V.
This enables the diode to provide high switching speed and better system efficiency.  The low noise is due to the very low reverse 
recovery time of about 100 per sec.
__Basic Idea__: The signal from mobile phone is a RF signal. When a mobile phone is present near the circuit, the RF signal from the
mobile induces a voltage in the inductor via mutual induction. This AC signal of high frequency of the order of GHz is rectified by 
the Schottky diode. The output signal is filtered by the capacitor. This low power signal can be amplified and used to power any 
indicator like an LED in this case. The signal is amplified using BJT in its common emitter mode.  i.e. the emitter base junction 
is forward biased and the collector base junction is reverse biased, a small base current results in a larger collector current.

4)FM bugger
