__Problem Statement__: \
To make a micro mouse which can navigates itself through a maze.

__Design__ \
There are few constraints which we have to keep in mind.
(1)The device should be self-contained, with no remote controls or pre-loaded maze configurations 
(2)The device should not use an energy source requires combustion. 
(3)The device should not leave any part of its body behind while navigating the maze
(4)The device should not modify or damage the maze, and should not jump or fly over the maze walls
(5) Width<16cm Height<100cms

__Components__
1) ATmega32 8-bit RISC Microcontroller
2) Faulhaber 1524E 6V motor(absence of fatigue, maximum precision and speed, optimum ergonomics.).Much cheaper alternative but less
precison: N20-6V-600RPM dc motor with encoder.
3) Ultrasonic Sensors HC-SR04 (explained in Hexapod) ![datasheet](https://cdn.sparkfun.com/datasheets/Sensors/Proximity/HCSR04.pdf)
Cheaper alternative: IR sensors but less reliable and can cause problem due to light intensity.
4) Power bank as range allows


![](https://github.com/Ankit017-c/Electronic-Projects/blob/master/images/Screenshot%20(84).png)

The ATmega32 device is used as a central controller for the micromouse system, and can be programmed in standard C (recommended), or in Assembly. A set of libraries are available from Procyon AVRlib that will make some features on this device much easier to use. In addition it is recommended to program this device in AVRStudio 4 or higher and utilize the included avr-libc libraries.(AVR Libc is a Free Software project whose goal is to provide a high quality C library for use with GCC on Atmel AVR microcontrollers)

Utrasonic vs IR sensors: \
Ultrasonic sensors are, for the most part, completely insensitive to hindering factors like:Light,Dust,Smoke, Mist, Vapor etc
Ultrasonics aren’t as good as Infrared at defining edges of an area.
Infrared sensor values normally fluctuate in variant light conditions.  
When objects pass within the range, the light waves detect those objects and reflect the presence back to the sensor. Their wavelengths are less than that of microwaves.  While they’re able to detect motion, they can also measure the emission of heat by an object.
There are a lot of limitations in infrared sensors, like the inability to use them in sunlight due to interference. It can make outdoor applications or dark indoor applications difficult. Ultrasonic sensors work using sound waves, detecting obstacles is not affected by as many factors. Thus we will use ultrasonic sensors.

Faulhaber motors has very high precision and its very useful in this constrained enviroment but the major problem is cost. So much cheaper alternative is N20-6V motors with encoders for providing feedback signals to control the speed and overall stability.

We can use power bank in the range allowed and in accord with our voltage requirement. 
