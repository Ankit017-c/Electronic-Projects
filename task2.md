__Ideation project 1(Line follower robot):__
The link for project:
__Problem Statement__
To make a robot to follow the predefined line drawn on floor.
__Ideation phase__
This robot can be divided into several parts:
• Infrared Sensors
• ADC (Analog to Digital Converter) and sensor circuit =>LM234 //two lm234 can support 8 sensors used in the project
• Processor => AVR microcontroller
• Driver=>IC L298 //L298 works happily up to 16 volts without any heat sink.//Environment need to be clean without dust,high humidity.
• Actuators (Motors and wheels)=>two motor drivers, L298
• Chassis and body structure

|Component|Feasibility|Advantages|Disadvantages|
|---------|-----------|----------|-------------|
|ADC LM234|Good managing of processing time|Two LM234 can support 8sensors used in project|ADC is that after every conversion, the counter gets RESET and count starts from 0 onwards. So, the conversion time depends on the magnitude of the input signal|
|AVR Microcontroller|Tough to Program|High performance, high speed and low power consumption.|Only available source is Atmel,fairly low power.|