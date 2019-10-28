# Space_Technology_Development_Team
The Challenge | Set Your Sights High! NASA builds and operates numerous satellite and airborne missions that deliver critical measurements and data to the world’s science community. Your challenge is to develop a tool that enables people to identify NASA satellites and satellite instruments as they fly over their locations on Earth. Help people explore the data and applications coming from the instruments overhead!


Link to NASA website:

https://2019.spaceappschallenge.org/challenges/living-our-world/set-your-sights-high/teams/space-technology-development-team/project

Link to official document submitted(Read-Only):
https://docs.google.com/document/d/1HU5X-25PlSWVo7L3nya_WIhBX7-DanZiKC2k5Emcmds/edit?usp=sharing


Minicube

    Raspberry Pi 4 controller Programmer for (decryption + satellite routing control + communication management between the satellite and the ground station via transmitter and receiver circuits).
    battery ,backup for the power supply.
    photosensors.
    solar cells ,power supply.
    Camera
    transmitter and receiver circuits .
    operations signals.
    Filters.
    RCL circles.
    Mercury tubes .
    Nano hydraulic arm.
    A mixture of metals (aluminum and galvanized iron) for the outer structure of the satellite .
    Stepper motors.
    Conductive wires.
    Thermal control louvers connected via bimetallic springs.
    Printed antenna.
    Monopropellant[Compressed Gas]
    Magnetic electrodes + Electromagnet
    List of items used above. 






The main idea of this project is to develop CubeSat satellites through the development of new mechanisms and methods to improve the functioning of the satellite.

The mission of the satellite will be to take pictures of the Earth's surface from space and send information to an earth station (for air navigation and climate change study).


CubeSats are a class of research spacecraft called nanosatellites. CubeSats are built to standard dimensions (Units or “U”) of 10 cm x 10 cm x 10 cm. They can be 1U, 2U, 3U, 6U or 12U in size, and typically weigh less than 1.33 kg. These satellites can be used for communications, studying the earth's upper atmosphere and taking pictures of the earth from space.The communication between the satellite and the earth station is carried out by frequencies VHF/UHF according to the licenses granted by the state in the spectrum distribution.They can be placed on orbits outside the atmosphere or placed in balloons at high altitudes.The chassis of the CubeSat would be made of small-sized flaps controlled by bimetallic springs to maintain thermal stability inside the satellite. As soon as the temperature inside the satellite increases due to the difference in the thermal expansion it leads to the expansion of spring and therefore opening the flaps vice-versa for the closing of the flaps when the system cools.









EXISTING ISSUES:

In general, the computational ability of spacecraft and satellites has lagged behind terrestrial computers by several generations. Moore's Law turns the supercomputers of yesterday into the laptops of today, but space computing remains relatively underpowered due to the harsh radiation environment and low risk-tolerance of most space missions,possible application that could be hosted onboard the next generation of high performance satellites, performing object classification on satellite imagery. Automation of satellite imagery processing is currently performed by servers or workstations on Earth. First traditional computer vision techniques such as edge detection and sliding windows are used to detect possible objects on the open ocean.

Existing cubesat satellite architectures use a “bent pipe” approach ; ground stations issue commands for such nano-satellites to dowlink unprocessed data.Bent pipes do not scale as the volume grows with the amount of data collected.Additionally the is a requirement of onboard computation so that the satellite can make “smart” decisions incase of loss or interruption of signal with the ground station.

Nano-satellites are equipped with high data-rate camera and other sensor feeds,Bandwidth from the sensor to the ground station is limited thus limiting this kind of centralized data processing approach, which is indeed unreliable.

All these factors make the capabilities of nano-satellites restricted by centralized terrestrial processing.



Cubesats are composed of 10cm×10cm×10cm (“1U”) volumes. Each 1U volume is restricted to 1.33kg. Small solar panels provide tens of watts of power or less. Existing onboard computers are simple, low-performance parts used mainly for pointing sensors, buffering data, and managing radios.

Earth-observing camera is included for use by the dual CSP units for sensing and processing. The full-resolution images are 2448x2050 pixels, but connection speeds to Earth are in the range of tens of kilobits, and thus these images take a great amount of time to downlink from space.



We develop support for processing high-rate data in cubesats. Tiled image processing can be tuned empirically to maximize accuracy. Intelligent early discard avoids processing uninteresting sensor data.



Using Unlike x86-based systems, most ARM systems (like those on CSP) do not have a supported pre-built TensorFlow package (i.e. installation isn’t as simple as pip install tensorflow). Furthermore, on embedded systems with limited memory and compute, the Python frontend adds substantial overhead to the system and makes inference slow.





The problems that we will address in this project are:

1- Making a high-efficiency satellite while maintaining the small size of the satellite.

2- Energy management for correspondence between the satellite and the Earth station.

3- Direct the satellite and maintain the presence of the satellite in orbit.

4- Lack of Onboard compute power for collection/sensing and processing of data.







    Solution:

Proposed Solutions To The Above Problems Numbered:

1- To increase the efficiency of the satellite we will use the Raspberry Pi 4 controller to act as the main controller of the satellite, and we will use the ports Raspberry Pi 4 as inputs (camera + light sensors) and outputs (to control parts such as solar cells and hydraulic arm).

This controller has been chosen because it is small in size and support for many functions and applications and also features a good data processing capability with the possibility of connecting the camera directly to it via the DSI port and connect the optical sensors through the general digital ports General Purpose Inputs / Outputs.

2-We have addressed the problem of orientation of the satellite and dispensed with the reaction wheel (to control the attitude of the satellite), through the creation of a new mechanism does not depend on the Pushing force or fans, but we have created a new method based on changing the centers of physical weight of the satellite in certain directions that will create a sequential circle movement, this movement changes the position of the satellite and modify the direction and we will explain The non-use of the energy stored in the battery inside the satellite will provide the energy used by the signal amplifiers inside the satellite for other purposes and will also provide the power to send signals to the earth station.

We will also increase the length of the solar panels but without affecting the size of the satellite, by making the solar panels fold down like a sail after the satellite stabilized in orbit, which will increase the number of photons falling on the panels and thus save more energy.

3-The exploitation of chemical compounds of capillary property and density deformities of some materials such as:Mercury, plutonium, antimony, bismuth, gallium, silicon, zinc cyanide and zirconium tungstate.

The direction of the satellite is adjusted by controlling the intensity of the heat projected on these materials inside small tubes distributed in the four directions inside the satellite, making it expand causing a change in the center of balance and the physical weight of the satellite. It is controlled through ports connected by Stepper motors that are closed and opened through directions from the Raspberry Pi controller according to the data entered by it from the optical sensors (photosensors).

The use of changing the position of the gravity of the satellite (physical weight) to control the direction through the expansion of some of the chemical elements inside it provides energy for correspondence between the satellite and the earth station and increases battery life.



4-The Raspberry Pi controller features easy programming by connecting it to a computer, allowing the use of processing software that includes An image processor, also known as an image processing engine, image processing unit (IPU), or image signal processor (ISP).








Conclusion:

We have developed a satilight which is capable of going to orbit and also detecting climate change using a camera connected to a low power raspberry PI 4. We have also developed the guidance and control mechanisms of the satellite .In our project we harnessed the changing satellite mass in controlling satellite orientation as we developed the solar cells of the satellite. 


********** Space Technology Development Team ***********


Leaders:


1- Rishabh Chakrabarty  
 @exynos - Computer Control and Communication Systems
 
2- Amon Saka Kaneko
 @amon4321 - Student in High School.
 
3-Albedeir Yaseen Jafer
 @albedeir - Communication and control engineering.

Members:
4- Stephen Wallen 
 @a-wallen  - Graphics. 
5- Fedaa Ahmed Alsoufi 
 @alsoufifedaa - Programmer systems.
6- Hatvi Thakkar  
 @hthakka1 - Aerospace Engineer.
 
 
 

