__Problem Statement__: /
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
3) Ultrasonic Sensors HC-SR04 (explained in Hexapod)
Cheaper alternative: IR sensors but less reliable and can cause problem due to light intensity.
4) Power bank as range allows

