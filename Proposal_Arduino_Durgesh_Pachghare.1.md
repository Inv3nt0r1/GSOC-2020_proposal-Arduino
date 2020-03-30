
# Writing examples, projects and enhancements for official libraries - A practical Approach

#### 26 March 2020, Durgesh Pachghare

  

## Abstract

 Examples listed in Arduino libraries are the biggest source of learning for beginners to professionals. Examples are the first face of any library that everyone looks for. Most people use implementation of function as stated in examples. Having a rich set of examples that are easy to understand and that shows its capabilities is really important. Some libraries lack such examples. Thus, I have taken this project to make my contribution in writing examples for official libraries under GSOC 2020. This project aims at following things:

1.  Writing more useful and practical examples wherever needed for Arduino libraries demonstrating the use of all the functions/features of the library.
2. Most of the projects contain the integration of multiple components like sensors and actuators. Thus, this project aims at writing examples that contain simple applications based on the integration of libraries, making hardware prototypes and documenting them in [Project Hub](https://create.arduino.cc/projecthub) that can really inspire developers to create and innovate.
3. Add some enhancements / solve bugs in the libraries.


## Technical Details


*  After reviewing all the Libraries listed under Arduino-Libraries, I have listed down libraries that need examples or potential projects that can be done and documented on Project Hub and also enhancements in libraries like adding new features or solving a few bugs.
* **Note:** However, the examples and projects that I have listed below are just my understanding of the need of examples in the libraries. I will be happy to discuss with mentors to list down a different set of examples or edit this existing list even on different libraries if needed.

These details are given as follows:


**Note:** Examples having [ Project ] tag are projects that will get implemented on hardware and documented on Project Hub.


#### [Keyboard](https://github.com/arduino-libraries/Keyboard)

This library allows an Arduino board with USB capabilities to act as a Keyboard.
 
- Examples Already Present:
  - Serial.ino - Reads a byte from the serial port, sends a keystroke back
- Examples Can be added:
  - KeyPattern.ino - Send keystrokes from a pattern of keys specified in the program
  - ProgramKeys.ino - Read a pattern of keys (Printable) from Serial monitor and program Arduino to send that pattern
  - Shutdown.ino - Program containing keystrokes to shut down a computer
  - MacroDeck.ino - Create a macro deck containing small array of switches programmed to send specific combination of keystrokes as a macro (like StreamDeck)
  - [ Project ] GamePad - Simple PS2 remote like gamepad containing 2 Joysticks (1 controlling aim and another controlling movement) and other programmable buttons
  

#### [Mouse](https://github.com/arduino-libraries/Mouse)

This library allows an Arduino board with USB capabilities to act as a Mouse.

- Already present: NA
- Can be added:
  - JoystickControl.ino - Move the mouse with the help of joystick connected to Arduino
  - DrawShapes.ino - Open paint and draw primitive shapes like reactangle, circle and square. 
  - [ Project ] GamePad - Simple PS2 remote like gamepad containing 2 Joysticks (one controlling aim and another controlling movement) and other programmable buttons like for fire and reload

#### [Arduino_JSON](https://github.com/arduino-libraries/Arduino_JSON)

Process JSON in your Arduino sketches.

- Examples Already present:
  - JSONArray.ino - This sketch demonstrates how to use JSON arrays.
  - JSONKitchenSink.ino - This sketch demonstrates use of functions in JSON library.
  - JSONObject.ino - This sketch demonstrates how to use JSON objects.

- Examples can be added:
  - IterateJSONObject.ino - Iterate through keys and values of JSON Object and function of finding value of specified key (To get clear understanding of how incoming JSON object is handled)
  - [ Project ] DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries (To get clear understanding of how JSON are used in application)

  
#### [Servo](https://github.com/arduino-libraries/Servo)

This library allows an Arduino board to control RC (hobby) servo motors.

- Already present:
  - Knob.ino - Move the servo on the input of Analog Potentiometer
  - Sweep.ino - Move servo from 0 to 180 and 180 to 0
- Can be added:
  - Wiper.ino - Using a servo as a car Wiper, activated by a switch
  - AutoDoor.ino - Open door (by moving servo) when someone comes in front of it (ultrasonic sensor) (SmartDustbin)
  - [ Project ] PanTiltIMU - Pan tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU (LSM9DS1/LSM6DS3)

#### [SD](https://github.com/arduino-libraries/SD)

The SD library allows for reading from and writing to SD cards.

- Can be added:
  - LogDataInCSV.ino - Log data from sensors into csv file
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature, and clock onto a display and log the data onto an SD card

<br>
<br>
<br>

#### [RTCZero](https://github.com/arduino-libraries/RTCZero)

The RTC library enables an Arduino Zero or MKR1000 board to take control of the internal RTC.

- Library Enhancements:
  - Function to set the RTC clock to the time of compilation
  - Accurate wrapping of time for functions setHours() and setMinutes()  
- Examples that can be added:
  - SleepWakeRTC.ino - Example in which arduino performs periodic task and goes in sleep mode after completing the task with setting an wake up alarm
  - [ Project ] CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. 
 


#### [AudioZero](https://github.com/arduino-libraries/AudioZero)
The AudioZero library enables an Arduino SAMD Board to play back .wav files from a storage device.

- Examples already present:
  - SimpleAudioPlayerZero.ino -  Demonstrates the use of the Audio library for the Arduino Zero
- Examples can be added:
  - Playlist.ino - Play all songs present in SD card sequencially or shuffled.  
  - [ Project ] CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. 


#### [Arduino_HTS221](https://github.com/arduino-libraries/Arduino_HTS221)

Allows you to read the temperature and humidity sensors of your Nano 33 BLE Sense.

- Examples already present:
  - ReadSensors.ino - Read the humidity and temperature sensor
  - ReadSensorsImperial.ino - Read the sensor values with imperial unit
- Examples can be added:
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature and clock onto a display and log the data on an SD card periodically



  

#### [Arduino_LSM6DS3](https://github.com/arduino-libraries/Arduino_LSM6DS3)

Allows you to read the accelerometer and gyroscope values from the LSM6DS3 IMU on your Arduino Nano 33 IoT or Arduino Uno WiFi Rev2 boards.

- Enhancement in Library:
  - Use of built-in FIFO Buffer
  - adding use of various modes which uses built-in FIFO buffer
  - Use of on-chip temperature sensor
- Examples Already Present:
  - SimpleGyroscope.ino - reads the gyroscope values from the sensor and prints on Serial monitor
  - SimpleAccelerometer.ino - reads the accelerometer values from the sensor and prints on Serial monitor
- Can be added:
  - SimpleTemperatureSensor.ino - Example to read temperature from the sensor
  - ReadWithFIFO.ino - Example to demonstrate use of FIFO Buffer while reading from the sensor
  - [ Project ] PanTiltIMU - Pan tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU (LSM9DS1/LSM6DS3)


#### [Arduino_LSM9DS1](https://github.com/arduino-libraries/Arduino_LSM9DS1)

Allows you to read the accelerometer, magnetometer and gyroscope values from the LSM9DS1 IMU on your Arduino Nano 33 BLE Sense.

- Enhancement in Library:
  - use of built-in FIFO Buffer
  - adding use of various modes which uses built-in FIFO buffer
- Already Present:
  - SimpleAccelerometer.ino - read the accelerometer values from the sensor and prints on the serial monitor
  - SimpleGyroscope.ino - reads the gyroscope values from the sensor and prints on Serial monitor
  - SimpleMagnetometer.ino - reads the magnetic field values from the sensor and prints on the serial monitor
-  Can be added:
   - ReadWithFIFO.ino - Example to demonstrate the use of FIFO Buffer while reading from the sensor
   - [ Project ] PanTiltIMU - Pan tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU (LSM9DS1/LSM6DS3)



#### [NTPClient](https://github.com/arduino-libraries/NTPClient)

- Library Enhancements:
  - write function getFormattedDate() and getFormattedDateTime()
  - add error handling routines to resolve bugs like crashing when DNS does not resolve
- Examples that can be added:
  - Example demonstrating the use of individual function of fetching hour, minutes, second, etc
  - Example demonstrating the use of setTimeOffset(), getFormattedDate() and getFormattedDateTime()

  

#### [ArduinoCloudThing](https://github.com/arduino-libraries/ArduinoCloudThing)

- Examples already present: NA
- Examples that can be added:
  - [ Project ] IoTSensorHub - Example project demonstrating the use of IoT Cloud by sending sensor data and visualizing them on cloud

  

#### [ArduinoModbus](https://github.com/arduino-libraries/ArduinoModbus)
Use Modbus with your Arduino.

- Examples can be added:
  - TCP:
    - EthernetModbusClientToggle.ino - Example to create a Modbus (Ethernet) TCP Server with a simulated coil. The value of the simulated coil is set on the LED
    - EthernetModbusServerLED.ino - Example to toggle the coil of a Modbus (Ethernet) TCP server connected on and off every second.

#### [ArduinoGraphics](https://github.com/arduino-libraries/ArduinoGraphics)

Core graphics library for Arduino. Based on the Processing API.

- Library Enhancement:
  - Add primitives shapes like circle using Bresenham's circle drawing algorithm and ellipse using Midpoint ellipse drawing algorithm
  - Add rotate() and translate() API for different types of coordinates, really helpful when we need to port the code for different screen s
- Examples already present: NA
- Can be added:
  - SimpleDrawing.ino - Simple Drawing containing shapes like circle, square filled with colors
  - DrawWithText.ino - Example demonstrating combined use of Text, strokes and shapes
  - AllFunctions.ino - Example demonstrating use and output of all usable functions of the library (Like Display "rect()" text first and use of rect() function by drawing rectangle)
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature, and clock onto a display and log the data onto an SD card




#### [Arduino_APDS9960](https://github.com/arduino-libraries/Arduino_APDS9960)

A library for the APDS9960 sensor, allows you to read gestures, color, and proximity on your Arduino Nano 33 BLE Sense board and other boards with sensor attached via I2C.

- Examples can be added:
  - Simple example demonstrating simple application using sensors present in APDS9960 
  - [ Project ] SimpleSnakeGame - Simple snake game on MKR RGB Shield with input of Joystick or gestures on Nano 33 BLE.

  

#### [ArduinoDMX](https://github.com/arduino-libraries/ArduinoDMX)

Control DMX lights with your Arduino. Using RS485 shields, like the MKR 485 Shield.

- Examples already present:
  - DMXBlink.ino - This sketch toggles the value of DMX channel 1 between 255 and 0
  - DMXFade.ino - This sketch fades the value of DMX channel 1 between 0 and 255 in steps to create a fade effect
- Examples can be added:
  - MultipleChannels.ino - Example containing control of multiple DMX channels

  

#### [Arduino_MKRRGB](https://github.com/arduino-libraries/Arduino_MKRRGB)

Allows you to draw on your MKR RGB shield. Depends on the ArduinoGraphics library.

- Examples already present:
  - ScrollText.ino - This example demonstrates how to display and scroll text on the MKR RGB shield.
  - SimpleDraw.ino - This example demonstrates how to draw on the MKR RGB shield.
- Example can be added:
  - Visualization.ino - Random Color Visualizations
  - Clock.ino - Simple Clock on MKR RGB Shield
  - [ Project ] SimpleSnakeGame - Simple snake game on MKR RGB Shield and TFT LCD with input of Joystick or gestures on Nano 33 BLE.


#### [TFT](https://github.com/arduino-libraries/TFT)

This library enables an Arduino board to communicate with the Arduino TFT LCD screen.

- Examples can be done:
  - [ Project ] SimpleSnakeGame - Simple snake game on TFT LCD Display with input of Joystick or gestures on Nano 33 BLE / IOT
  - [ Project ] DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries (To get clear understanding of how JSON are used in application)

#### [Scheduler](https://github.com/arduino-libraries/Scheduler)

The Scheduler library enables the Arduino Due, Zero, and MKR1000 to run multiple functions at the same time. This allows tasks to happen without interrupting each other.

- Examples already present:
  - MultipleBlinks.ino - Demonstrates the use of the Scheduler library for the Arduino Due
- Examples can be added:
  -  Adding few more simple examples to demonstrate working and better utilization of Scheduling using Scheduler Library.


<br>
<br>
<br>
<br>
<br>
  
### List of Projects:
| List of Projects | Libraries Used | Hardware Used |
|--|--|--|
| GamePad - Simple PS2 remote like gamepad containing 2 Joysticks (one controlling aim and another controlling movement) and other programmable buttons like for fire and reload | Keyboard, Mouse | Arduino Nano 33 IOT |
| CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. | ArduinoSound, RTCZero, AudioZero | MKR1000, I2S mic, speaker |
| DisplayHumidityTemp - Display Current Humidity, temperature, and clock onto a display and log the data in an SD card | ArduinoGraphics, HTS221, TFT, SD | Nano 33 BLE Sense, Display |
| PanTilt - Pan-tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU | LSM9DS1 / LSM6DS3, Servo | Nano 33 IOT, Servos, 3D printed frame |
| IoTSensorHub - Example project demonstrating the use of IoT Cloud by sending sensor data and visualizing them on cloud | ArduinoIOTCloud |  Nano 33 BLE Sense |
| SnakeGame - Simple snake game on MKR RGB Shield with input of Joystick or gestures | MKRRGB, TFT, Arduino_APDS9960| MKR RGB Shield / TFT LCD, Nano 33 BLE Sense |
| DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries | TFT, Arduino_JSON, WiFi | MKR 1000, TFT LCD |

 
 <br>
 <br> 
 
## Schedule of Deliverables

### **Before Community Bonding Period**

1.  Gather detailed insights of all 90 libraries and list down better examples that can be added to the libraries. Make changes in the list alongside.
2. Read contribution guidelines and get familiar with the standards and style-guide. Fix issues and create necessary pull requests to the best of my abilities to better understand and get familiar with contribution standards. 
3. Understand the electronics characteristics of newer Arduino Boards. It's much easier to work with any board and components once you have enough knowledge about its electronics.

### **Community Bonding Period**

1.  Purchase all the required hardware required from the Arduino store.
2. Communicate with mentors, get familiar with the expectations, work culture and standards. Plan platform and schedule for communication and submission.
3. Keeping my primary plan in mind, I will communicate with my mentors to create a more refined plan, finalize the examples list.
4. Create a testing and documentation plan, templates for testing details and documentation for submission.
5. Read datasheets of sensors and boards, learn and understand more about the libraries. Get everything ready to start coding.
6. Most importantly, Get involved in the community, communicate often, become familiar with everyone and become a part of this great family.

### **Phase 1**

List of libraries:
1. Keyboard
2. Mouse
3. Arduino_JSON
4. Servo
5. SD
6. RTCZero
7. ArduinoZero
8. Arduino_HTS221

Projects that will be done in this phase:

 1. GamePad - Simple PS2 remote like gamepad containing 2 Joysticks (one controlling aim and another controlling movement) and other programmable buttons like for fire and reload
 2. CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button.
 3. DisplayHumidityTemp - Display Current Humidity, temperature, and clock onto a display and log the data in an SD card

#### **Timeline**
This week-by-week timeline provides a rough guideline of how the project will be done.
Week 1: Libraries Keyboard, Mouse, Arduino_JSON and Servo
Week 2 and 3: Libraries SD, RTCZero, ArduinoZero, Arduino_HTS221
Week 3: Projects GamePad, CoronVirusWashHandAlert
Week 4: Project DisplayHumidityTemp, doing pending tasks and documentation. 

### **Phase 2**
List of libraries:
 1. Arduino_LSM6DS3
 2. Arduino_LSM9DS1
 3. NTPClient
 4. ArduinoCloudThing
 5. ArduinoModbus

Projects that will be done in this phase:

 1. PanTilt - Pan-tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU
 2. IoTSensorHub - Example project demonstrating the use of IoT Cloud by sending sensor data and visualizing them on cloud

#### **Timeline**
Week 5 and Week 6: Libraries Arduino_LSM6DS3, Arduino_LSM9DS1
Week 6: NTP Client, ArduinoCloudThing and ArduinoModbus
Week 7 and 8: PanTilt
Week 8: IoTSensorHub and doing pending tasks and documentation. 


### **Final Week**
List of libraries:

 1. ArduinoGraphics
 2. Arduino_APDS9960
 3. ArduinoDMX
 4. Arduino_MKRRGB
 5. TFT
 6. Scheduler

Projects that will be done in this phase:

 1. SnakeGame - Simple snake game on MKR RGB Shield with input of Joystick or gestures
 2. DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries

#### **Timeline**
Week 9: ArduinoGraphics, Arduino_APD9960, ArduinoDMX, Arduino_MKRRGB
Week 10: TFT, Scheduler, and project DisplayWeather
Week 11: Project SnakeGame
Week 12: Finalizing, Completing Pending tasks and Documentation.
  

## Development Experience

### **Arduino:**
I have around six years of experience working with Arduino. I started learning and trying example sketches from my school time. From then on, I have developed a lot of Arduino projects of robotics, drones containing various components. 
* **Professional Experience:**
	* I have experience of working with a startup as an under Govt. of India that designed and manufactured smart pill dispenser device under the scheme of eradicating Tuberculosis from India. 
	* My task was to design and program the embedded device in Arduino, which records when the user takes the medicine, triggers an alarm when the medicine needs to be taken and sends data to the server periodically through SMS. 
	* Since the actual code is under NDA, I have my [practise codes](https://github.com/Inv3nt0r1/Smart-pill-dispenser-device) which I used to test individual components and practise.


* **Development Experience:**
	* I have been a part of the Robotics club in my institute and also been Lead of the technical team 'Team Vector' which represents our institute in various robotics competitions like ABU Robocon. 
	* Repository containing basic codes for all the components that we used in the robotics club [is here.](https://github.com/Inv3nt0r1/Team_Vector_comp)
	* Project - 'Pre and post Accident detection and alerting system' which won the first prize in National Level Expo: [Description and code](https://github.com/Inv3nt0r1/Pre_post_accident_detection_and_alerting_system)
	* Project - Autonomous Quadruped Robot which uses servos as actuators. [ [Code] ](https://github.com/Inv3nt0r1/Team_Vector_comp/tree/master/Robocon_2019_Archive)
	* I have worked on Following Arduino Boards:
		1. Arduino Uno
		2. Arduino Mega
		3. Arduino Mini
		4. Arduino Nano
		5. Arduino Lilypad
		6. Other Arduino Supported Boards like: Teensy 3.2 and 3.6	
	* Single Board Computers:
		8. Raspberry Pi 3B+ and 4
		9. Intel Edison
	* I have experience with a lot of sensors from simple to industry level including but not limited to Distance sensors, Line Followers, Temperature sensors, IMUs over various buses like I2C and SPI.
	* I also have worked with some IoT Projects, various communication protocols, etc. 
	* I also have experience with a lot of Arduino shields like USB Shield, Ethernet Shield and various Motor Drivers.
	* I have done simple to complex projects using Arduino which includes all of these components with the proper design of algorithm and code.

### **Github**
My Github Profile: [Inv3nt0r1](https://github.com/Inv3nt0r1)

I am using Git from the last 2 years to manage my projects locally and have more than one year of experience in using Github. 

### **Other than Arduino:**
* I am passionate about robotics as well as drones. I have made many drone prototypes using some open-source firmwares like Ardupilot, BetaFlight as well as developing a simple code from scratch.
* I have an Instagram Channel where I upload pictures of some projects and things that I do: [TechOverclock](https://www.instagram.com/techoverclock/?hl=en)
* I have worked with These single board computers:
	1. Raspberry Pi 3B, 3B+ and 4
	2. Intel Edison
* Project - [Drowsiness Detection on Raspberry Pi](https://github.com/Inv3nt0r1/Drowsiness_detection_RaspberryPi) (A part of pre-post accident detection and alerting system project)
* I have done various testing projects as well. I am well experienced in writing test cases and test scenarios to test any software product. 


## Other Experiences


-   I also do competitive programming. I stood in the top 50 nationally in the Computer Society of India’s Discover Thinking programming contest. [[Certificate]](https://drive.google.com/open?id=1sdcS67UwYru_9lLJhZdGxs1RpKCd0VE1)
-   Technical Team Lead - Team Vector.
	-   Team Vector is a team of students in our institute who participates in Robotics Competitions like ABU Robocon.
	-   Being a lead my task was to teach Arduino and basics of Robotics to newcomers, decide strategies about participating in the competition.
	-   Designed High-Level Architecture of Robot and different software modules according to the application and testing them after development
	-   Developed algorithms from scratch like autonomous path planning and navigation using Machine Vision.

-   DELEGATE - Embedded Systems Conference [[Certificate]](https://drive.google.com/open?id=1H4HLAFzItwmvsjwpGLO4oUnX0OsHuMUP)
  
  

## Why this project?

  
Arduino is a member of my daily experiments. I learned Arduino completely from the examples of Libraries present in the IDE and using that I used to write my programs and try it. After practicing, I was able to write advance level code with Arduino integrating multiple sensors, actuators, and various devices. The majority of newcomers who start learning Arduino come from a non-programming background. When I used to teach Arduino to my juniors, I came to know how important examples are in the process of learning and trying new things. I want to make a contribution that will be helpful for the entire community of makers. I always wanted my knowledge and my skills to be used for everyone, for a good cause. This is the biggest opportunity for me to do contributions as give as much as I can to such a great open-source organization that will be helpful for every maker in the world. 


## Do you have any other commitments during the GSoC period?

  
Now because of coronavirus pandemic, everything is postponed. We had our Final year project evaluation in may which will get extended to June. So for a few days, I will need to go to college for demonstrating, submitting and evaluating our project. That will not hamper much to this work. 
I will be completely free in July and Starting of August. 
Its my passion and I am ready to work even 12-14 hours a day. I can easily push to at least 50 hours a week in July and August. 

## About me
My name is Durgesh Pachghare, a Computer Engineering student, from K. K. Wagh Institute of Engineering Education and Research which is affiliated to Savitribai Phule Pune University. Arduino was the thing from which I started my learning and experiments in Robotics. I am a well-experienced candidate with six years of experience working with various Arduino boards, Embedded systems, IoT and a large variety of sensors and actuators. Hardware systems, IoT, Arduino has been my passion from school time. I spend my weekend time doing various projects based on Arduino, Robotics, Drones, etc. I am the best candidate for this project because I have much experience working with Arduino and related components. I have my basics clear and thus I can understand quickly and can contribute more planned. I believe in clearing the basics before doing anything and doing everything with perfection. It is my dream to work with such great organization and contribute for open source that will be useful for entire world. This is what motivates me the most. Looking forward to work in Arduino.

My Email: durgeshpachghare01@gmail.com
Contact Number: +91 7057676280
My Github: https://github.com/Inv3nt0r1
My linkedin: https://www.linkedin.com/in/durgeshpachghare/
My CV: https://drive.google.com/open?id=1P5Eh9fU-S0oWWur3-2mpUqhmANDzkpwM
Communication thread in GSOC's repo: https://github.com/arduino/summer-of-code/issues/98




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwMDUxNzQwMjksMTI1NjM5MDQ2Myw4NT
AyNjU3LDE0MTc2NjMwMjMsLTEyODQ3MTgyODcsNTAxNjUxNzgs
LTEyODQ3MTgyODcsMTgxMDQ4MDE5NCwxOTE4OTUxNjY3LDM4Mz
czNjQ5OCw4OTA2NzUxNSwtNDU2NjQ3NjczLDEwMTY0NTE0Njks
LTMyMzA1MzI0MCwtMTM2NzgzNjcyNiwtMjAyMTAzNjU4MCwxMT
c0NzA3Nzg2LC02NjQ3MTE2MTYsLTIxMjMyMjIwNjIsNjU1Mjcw
NzY0XX0=
-->