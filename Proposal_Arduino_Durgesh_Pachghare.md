# Title

  

## Abstract

  

Examples listed in Arduino libraries are the biggest source of learning for begineers to professionals. Some libraries lack examples that can make users understand the capabilities of the library.
This project aims at three things:

 1. Writing more useful and practical examples wherever needed for Arduino libraries demonstrating use of of all the functions/features of the library.
 2. Most of the projects contain the integration of multiple components like sensors and actuators. Thus, this project aims at writing examples that contain simple applications based on the integration of libraries, making hardware prototypes and documenting them in [Project Hub](https://create.arduino.cc/projecthub).
 3. Add some enhancements in the libraries. 


## Technical Details

After reviewing all the Libraries listed under Arduino-Libraries, I have listed down libraries which needs examples or potential projects that can be done and documented on Project Hub. Also some libraries need some enhancements, like adding new features or solving few bugs. These details are given as follows:

Examples having tag [ Project ] are projects that will get implemented and documented on Project Hub.

#### [Keyboard](https://github.com/arduino-libraries/Keyboard)

This library allows an Arduino board with USB capabilities to act as a Keyboard.
 
- Examples Already Present:
  - Serial.ino - Reads a byte from the serial port, sends a keystroke back
- Examples Can be added:
  - KeyPattern.ino - Send keystrokes from a pattern of keys specified in the program
  - ProgramKeys.ino - Read a pattern of keys (Printable) from Serial monitor and program Arduino to send that pattern
  - Shutdown.ino - Program containing keystrokes to shut down a computer
  - ShapesInPaint.ino - Open Paint and draw a small simple shapes like circle, rectangle
  - [ Project ] BluetoothControl - Control the mouse and keyboard with a basic Bluetooth Module and android app

  

#### [Mouse](https://github.com/arduino-libraries/Mouse)

This library allows an Arduino board with USB capabilities to act as a Mouse.

- Already present: NA
- Can be added:
  - MakeCircle.ino - Move the mouse on the screen to make a circle for 5 seconds
  - JoyStickControl.ino - Move the mouse with the help of joystick connected to Arduino
  - ShapesInPaint.ino - Open Paint and draw a small simple shapes like circle, rectangle
  - [ Project ] BluetoothControl - Control the mouse and keyboard with a basic Bluetooth Module and android app

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



#### [SD](https://github.com/arduino-libraries/SD)

The SD library allows for reading from and writing to SD cards.

- Can be added:
  - LogDataInCSV.ino - Log data from sensors into csv file
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature, and clock onto a display and log the data onto an SD card

  

#### [ArduinoGraphics](https://github.com/arduino-libraries/ArduinoGraphics)

Core graphics library for Arduino. Based on the Processing API.

- Library Enhancement:
  - Add primitives shapes like circle using Bresenham's circle drawing algorithm and ellipse using Midpoint ellipse drawing algorithm
  - Add rotate() and translate() API for different types of coordinates
- Examples already present: NA
- Can be added:
  - SimpleDrawing.ino - Simple Drawing containing shapes like circle, square filled with colors
  - DrawWithText.ino - Example demonstrating combined use of Text, strokes and shapes
  - AllFunctions.ino - Example demonstrating use and output of all usable functions of the library (Like Display "rect()" text first and use of rect() function by drawing rectangle)
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature, and clock onto a display and log the data onto an SD card

  

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

  

#### [RTCZero](https://github.com/arduino-libraries/RTCZero)

The RTC library enables an Arduino Zero or MKR1000 board to take control of the internal RTC.

- Library Enhancements:
  - Function to set the RTC clock to the time of compilation
  - (Solve bug of setting 24 as an hour and then counting till 31)
- Examples that can be added:
  - SleepWakeRTC.ino - Example in which arduino performs periodic task and goes in sleep mode after completing the task with setting an wake up alarm
  - [ Project ] CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. 

#### [AudioZero](https://github.com/arduino-libraries/AudioZero)
The AudioZero library enables an Arduino SAMD Board to play back .wav files from a storage device.

- Examples already present:
  - SimpleAudioPlayerZero.ino -  Demonstrates the use of the Audio library for the Arduino Zero
- Examples can be added:
  - [ Project ] CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. 

#### [ArduinoModbus](https://github.com/arduino-libraries/ArduinoModbus)
Use Modbus with your Arduino.

- Examples can be added:
  - TCP:
    - EthernetModbusClientToggle.ino - Example to create a Modbus (Ethernet) TCP Server with a simulated coil. The value of the simulated coil is set on the LED
    - EthernetModbusServerLED.ino - Example to toggle the coil of a Modbus (Ethernet) TCP server connected on and off every second.


#### [Arduino_HTS221](https://github.com/arduino-libraries/Arduino_HTS221)

Allows you to read the temperature and humidity sensors of your Nano 33 BLE Sense.

- Examples already present:
  - ReadSensors.ino - Read the humidity and temperature sensor
  - ReadSensorsImperial.ino - Read the sensor values with imperial unit
- Examples can be added:
  - [ Project ] DisplayHumidityTemp - Example project to display Current Humidity, temperature and clock onto a display and log the data on an SD card periodically

  

#### [Arduino_APDS9960](https://github.com/arduino-libraries/Arduino_APDS9960)

A library for the APDS9960 sensor, allows you to read gestures, color, and proximity on your Arduino Nano 33 BLE Sense board and other boards with sensor attached via I2C.

- Examples already present:
  - ColorSensor.ino - simple example demonstrating reading from the color sensor
  - GestureSensor.ino - simple example demonstrating reading from gesture sensor
  - ProximitySensor.ino - simple example demonstrating reading from the proximity sensor
  - FullExample.ino - simple example containing reading all sensors and printing values on the serial monitor
- Examples can be added:
  - Simple example demonstrating simple application using sensors present in APDS9960 
  - [ Project ] SnakeGame - Simple snake game on MKR RGB Shield with input of Joystick or gestures on Nano 33 BLE.

  

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
  - Clock.ino - Simple Clock on MKR RGB Shield using RTCZero
  - [ Project ] SimpleSnakeGame - Simple snake game on MKR RGB Shield and TFT LCD with input of Joystick or gestures on Nano 33 BLE.


#### [TFT](https://github.com/arduino-libraries/TFT)

This library enables an Arduino board to communicate with the Arduino TFT LCD screen.

- Examples can be done:
  - [ Project ] DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries.
  - [ Project ] SimpleSnakeGame - Simple snake game on TFT LCD Display with input of Joystick or gestures on Nano 33 BLE / IOT
  - [ Project ] DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries (To get clear understanding of how JSON are used in application)


#### [Scheduler](https://github.com/arduino-libraries/Scheduler)

The Scheduler library enables the Arduino Due, Zero, and MKR1000 to run multiple functions at the same time. This allows tasks to happen without interrupting each other.

- Examples already present:
  - MultipleBlinks.ino - Demonstrates the use of the Scheduler library for the Arduino Due
- Examples can be added:
  -  Adding few more simple examples to demonstrate working and better utilization of Scheduling using Scheduler Library.

  

### List of Projects:
| List of Projects | Libraries Used | Hardware Used |
|--|--|--|
| BluetoothControl - Control the mouse and keyboard with a basic Bluetooth Module and android app | Keyboard, Mouse, ArduinoBLE | Arduino Nano 33 IOT |
| PanTilt - Pan-tilt mechanism (For ex. pan-tilt for fpv cam) on the input of Joystick or IMU | LSM9DS1 / LSM6DS3, <br> Servo | Nano 33 IOT, Servos, 3D printed frame |
| DisplayHumidityTemp - Display Current Humidity, temperature, and clock onto a display and log the data in an SD card | SD, ArduinoGraphics, Arduino_HTS221, TFT | Nano 33 BLE Sense, Display
| IoTSensorHub - Example project demonstrating the use of IoT Cloud by sending sensor data and visualizing them on cloud | ArduinoIOTCloud |  Nano 33 BLE Sense |
| SnakeGame - Simple snake game on MKR RGB Shield with input of Joystick or gestures | MKRRGB, TFT, Arduino_APDS9960| MKR RGB Shield / TFT LCD, Nano 33 BLE Sense |
| DisplayWeather - Display weather info on TFT LCD Display using TFT, JSON and WiFi libraries | TFT, Arduino_JSON, WiFi | MKR 1000, TFT LCD |
| CoronavirusWashHandAlert - A periodic alert which plays an audio asking users to wash hands to avoid getting infected by corona virus. Alert is disabled by a clap or a button. | ArduinoSound, RTCZero, AudioZero | MKR1000, I2S mic, speaker 




  
 
## Schedule of Deliverables

  


  

### **Community Bonding Period**

  

_What will you do during the community bonding period?_

  

### **Phase 1**

  

* Deliverable 1

* Deliverable 2

* ...

  

### **Phase 2**

  

* Deliverable 1

* Deliverable 2

* ...

  

### **Final Week**

  

_At this stage you should finish up your project. At this stage you should make

sure that you have code submitted to your organization. Our criteria to mark

your project as a success is to submit code before the end of GSoC._

  

## Development Experience

  

_Do you have code on GitHub? Can you show previous contributions to other projects?

Did you do other code related projects or university courses?_

  

_Do you have experience with Arduino?_

  

## Other Experiences

  

...

  
  

## Why this project?

  

_Why you want to do this project?_

  

## Do you have any other commitments during the GSoC period?

  

_Provide dates, such as holidays, when you will not be available._
