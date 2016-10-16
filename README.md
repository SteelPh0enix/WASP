# WASP
CanSat "WASP" sattelite project, based on Arduino

## Sensors and modules list with *[interfaces]*:
- **GLONASS NEO-7M-C** *[serial]* GPS Module 
- **HC-12** *[serial]* communication module (RF) 
- **IMU 9DOF** *[I2C]*, which contains
  * **LSM6DS33** 3-axis gyroscope/accelerometer
  * **LIS3MDL** 3-axis magnetometer
- **DHT11** *[Serial Single-Bus]* temperature and humidrity sensor
- Pololu *[analog]* gas sensors
  * **MQ-4** methane sensor
  * **MQ-131** ozone sensor
  * **MQ-8** hydrogen sensor
  * **MQ-5** LPG sensor
  * **MQ-7** carbon monoxide sensor
- **MOD-13** SD card reader

Additionaly, two servomotors for parachute, voltage converters (**D24V3F3** and **D24V22F5**), Li-Pol battery (**Dualsky 45C 2S**) and THT buzzer

Most basic quest, which our WASP have to do is temperature and humidrity measurement. Of course, we are expanding it by using a lot of sensors.
CanSat will send data to base, and write it to SD card (so it's not lost when we will loose contact with sattelite)
Also, there will be provided interface to see the data when it's received in base.

Second quest is tracking down WASP while it's falling down on parachute. We will try to create algorithm for landing in designated area, even autonomiccaly - just by sending coordinates of area. But that's so difficut, we don't know if it will work.

Also, another features - sattelite control, by turning on/off sensors for example. Also, we will be able to make maneuvers, by controlling parachute (with 2 servomotors).

WASP Team:
* Wojciech Olech (main programmer)
* Tomasz Jakubowski (electronics)
* Grzegorz Szczepański (sponsors and antenna)
* Mikołaj Sawa (casing and misc stuff)

We are from Poland, we learn in Electronic School Group in Lublin. We are starting in 2017 edition of CanSat competition. Wish us luck.