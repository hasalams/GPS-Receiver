# GPS-Receiver
Arduino based GPS receiver
## 1.	Introduction

This document gives you an explanation about the GPS Receiver device which can send its location data into a web server over Ethernet. Arduino platform is used to build both hardware and software elements of the GPS receiver. 

## 2.	List of Components

Hardware
Arduino UNO R3
Arduino Ethernet Shield 2
Adafruit ultimate GPS logger
GPS External Antenna
SMA to uFL RF Adapter Cable
Shield Stacking Headers
Software
Arduino IDE (v 1.7.6)

Please refer to **Items List** to view detailed information on the hardware components.

## 3.	How to build

### 3.1 Hardware

**Step 1:**
Assemble the Adafruit ultimate GPS logger using **Shield Stacking Headers** (do not use male headers) as instructed in the Adafruit GPS Shield Documentation.

**Step 2:**
Connect the GPS external antenna to the antenna connector using SMA to uFL RF Adapter Cable.

**Step 3:**
Connect the Arduino Ethernet Shield on top of Arduino UNO and then connect the Adafruit GPS shield on top of Arduino Ethernet Shield.

### 3.2 Software

Complete source code is available in the Code directory.

## How to use the device

**Step 1:**
Place the external antenna in a place where it is exposed to outdoor.
**Step 2:**
Connect one end of RJ45 cable into Ethernet shield and the other end to a router (connected to Internet) which has DHCP enabled. Once done, the device will automatically get its IP address.
**Step 3:**
Connect the power supply jack to the Arduino UNO and turn on the power. 
**Step 4:**
Identify the device status 
RED LED near GPS shield’s antenna connector
- Blinks every 1 second – GPS does not have a fix
- Blinks once in 15 seconds – GPS has a fix

Once the GPS has a fix, it will send data to sever in every minute. 


