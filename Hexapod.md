__Hexapod__ \
__Problem Statement__:To create the orientation and visual representation of Hexapod. \
__Simulation__ \
For the design and simulation we can use the tools available in MATLAB software. In addition, we can design and implement a dynamic model (using the Simscape Multibody toolbox) as well as a three-dimensional model of the robot, using Virtual Reality Modeling Language (VRML), that help to visualize the robot’s walking sequence. The data received from the IMU sensors to the microcontrollers is sent to the software wirelessly using Raspberry PI.

__Elecctronic Part__ \
In order to control the robot there must be some control unit.we can use __MCU Atmega2560__ to drive the servomotors and sensors on this robot. All sensors like sonars, LCD display, memory card, GPS module or force-sensitive resistors wil connect to this. LCD display is connected by digital pins using integrated __Hitachi HD44780 driver__, which allows 4-bit or 8-bit mode. The 4-bit mode requires seven I/O pins from the Arduino, while the 8-bit mode requires 11 pins. There are also 18 servomotors connected to digital pins and driven by MCU’s timers. The MCU is integrated on open-source electronic platform __Arduino Mega 2560__. Arduino board is connected to the Raspberry Pi via USB cable.We should use raspberry Pi because it has extremely low power consumption (max. 3.5 W) and can run linux based operating system Raspbian. There are several models, which differ in RAM, the number of USB ports or GPIO pins. Raspberry Pi is equipped with a USB Wi-Fi dongle, which is connected to a wireless network, and runs Qt client program(a small client server), which is able to find the IP address of the server and gets connected to it. All Sesors and servomoter are connected and driven by Arduino board. Sensor data are sent to a computer after successful connection. We will use this data in our software for the simulation of Hexapod.\
Sensors used are:
1) Ultrasonic distance sensors HC-SR04 – sonars. These sensors can measure distance from 2 cm to 400 cm. Alternatively we can use TFmini mounted to servo to get clean scan using single triggers per servo postition. OR for cheaper alternative we can use TOF sensor for distance measure as it is much more cheaper and compact than TFmini.
2) GPS modules \

__Pipeline__
HC-SR04 Sonars => MCU Atmega2560 => Raspberry PI =>(through wifi) Computer \

__Design and 3D Model__ \
To obtain the three-dimensional (3D) model of the hexapod robot, we will employ the VRML language, developing a robot model using simple geometrical figures. This language allows to obtain a complex model, simply using a group of basic 3D bodies (cubes, spheres, cones, etc.) as shown in figure below. There are many alternatives to develop a 3D model using VRML language: one of them consists in programming it directly using its commands or employing a graphical editor that eases the design. 

![](https://www.intechopen.com/media/chapter/50860/media/fig5.png)
