- 👋 Hi, I’m @CharlesBirks   
- 👀 I’m interested in the application of process controls using Arduino and RPI4 ...
- 🌱 I’m currently learning Python and diving deeper into the Arduino IDE to get the most out of the micro-controllers...
- 💞️ My current focus is on learning the building blocks needed for Simultaneous Localization and Mapping as applied to small robotics
- 📫I have been working in industrial thermal processing ( I sell Kilns and Heat Treat Furnaces) since 1973. 
      Prior to that I was in the US Navy and trained in "Fire Control" which is a euphimism for the process of using 
      a compass, gyroscopes, radars and sonar as input to computers, both analog and digital, to calculate the real-time bearing, 
      course, and range to a target for the purpose of predicting where it will be in the future and then interception with any form of ordinance.
      
  My current interest in SLAM is primarily for the purpose of "keeping the saw sharp". I am working on a small mobile robot of my own design and construction
  equiped with an RPLidar, a BNO055 IMU, and a series of 12 VL53L0X Time-of-Flight Flight Distance Measurement Sensors arrayed around the chassis perimeter to detect 
  obstructions, terrain, and overhead clearances.
      
  Each sensor group utilizes an Arduino Mega-2650 as direct operator, with a fourth board handling motors for the drive. 
  Each Arduino is connected via USB to the central RPI-4 which is tasked with overall command and control.
      
  Allowing the Arduino boards to interrogate and collate data from the sensors provides a continuous data stream to the RPi where planning and recording
  takes place.  The RPi on board the robot uses a local touch display for direct input when needed but will primarily operate headless
  using VNC.
      
  My goal is to get to where the robot can operate autonomously once a mission has been ordered, i.e. "go to this location".
  
  The current status of my project:
  1. RPLidar is working and provides a contiuous stream of data to the RPi, where it is collected and stored in a file.
  2. The BNO055 IMU is working and providing a continuous stream of heading data. This currently used to orient the lidar map and provide absolute 
     bearing data for the surrounding environment.
  3. The VL53L0X sensors provide a continuous stream of 12 data points; 8 sensors are aimed down at a 45 degree angle and provide information about 
     the terrain and any object that is too close. 4 sensor are aimed at 45 degrees up and will detect any overhead obstruction.
  4. The drive motors are functional with Hall effect encoders. Currently the motor control arduino has a 2 PID loops that control distance moved for
     each of two tank treads.
  5. Currently I am struggling with appropriate drive speed control to provide accurate steering and the ability to orient and move on a specific heading.   
      
  Constantly learning something new is the best way to maintain the brain's capacity and fend off the decline that comes with age. 

<!---
CharlesBirks/CharlesBirks is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
