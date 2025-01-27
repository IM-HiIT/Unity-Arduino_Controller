# Unity + Arduino Controller
version: 1.0.0  

  
# Requires
+ Arduino Uno  
+ Unity 5.4.1f1  
  
  
## Features
1. Reads the Input from an Arduino Uno JoyStick
2. Sends the Joystick Input to Unity
3. Simply Rotates a Cube GameObject in Unity MainScene
4. Reads out the Transform values of the Cube
  
  
## Installation
1. Download or Clone this Repository
2. Setup an Arduino Uno as Simple Single JoyStick Controller (See Guide for Tutorial)
3. Upload the "Arduino-Unity.ino" file to your Arduino
4. Run the MainScene in Unity
5. Enjoy the Results!
  
  
## Guides
+ For an extensive guide on How-To-Use and a Tutorial on How-To-Make see below

  
## ChangeLog
v.1.0.0
+ Created the initial Arduino Uno script
+ Created the initial Unity SerialRead script
+ Created the initial Unity SerailRead2 script
+ Api Compability Level to .NET 2.0. (instead of .NET 2.0 Subset)
+ Made simple MainScene for instant result feedback

  
# Extensive Tutorial Arduino - Unity
version: 0.1.0

## Description
A detailed how-to for creating a Controller with Arduino Uno and read the inputs in Unity 3D.  
This how-to is still in progress, you can find the finished project in the Repository.  

## ContentTable:
1. Making an Arduino Uno Controller
2. Creating the Arduino Uno script **(Not Finished)**
3. Setting up the Unity Project **(Not Finished)**
4. Creating the SerialRead script in Unity **(Not Finished)**
5. Creating an Simple Rotating Cube and UserInterface **(Not Finished)**

## 1. Making an Arduino Uno Controller
### Step 0) What is the Arduino Uno?
+ See the link below for the Official Arduino Website

[Official Arduino Website](https://www.arduino.cc/en/Main/ArduinoBoardUno "Visit the Official Website")

### Step 1) What do we Need?
1. An Arduino Uno
2. An Arduino Uno USB cable
3. 7x PinCables
4. 1x Arduino Parallax 2Axis JoyStick

### Step 2) Setting up the Arduino Schematic
![The Schematic](https://www.arduino.cc/en/uploads/Tutorial/joy_sch_480.jpg "Official Ardiono Schematic")

### Step 3) How does it Work?
The joystick in the picture below is nothing but two potentiometers that allow us to messure the movement of the stick in 2-D.

Potentiometers are variable resistors and, in a way, they act as sensors providing us with a variable voltage depending on the rotation of the device around its shaft.

![A Simple JoyStick](https://www.arduino.cc/en/uploads/Tutorial/joy_pic_480.jpg "A Simple JoyStick Example")

The kind of program that we need to monitor the joystick has to make a polling to two of the analog pins. 

We can send these values back to the computer, but then we face the classic problem that the transmission over the communication port has to be made with 8bit values, while our DAC (Digital to Analog Converter - that is messuring the values from the potentiometers in the joystick) has a resolution of 10bits.

In other words this means that our sensors are characterized with a value between 0 and 1024.

The following code includes a method called treatValue() that is transforming the sensor's messurement into a value between 0 and 9 and sends it in ASCII back to the computer.

This allows to easily send the information into e.g. Flash and parse it inside your own code. 

<!--

### Step 4) Colored Schematic
![]()


## 2. Creating the Arduino Uno script
### Step 1) Choosing an Arduino Uno ".INO file" Editor
We need an Arduino Uno Compiler to create and test your software
For this project in used [CodeBender Site](https://CodeBender.cc/ "CodeBender")

### Step 2)
### Step 3)
### Step 4)
### Step 5)
### Step 6)
### Step 7)
### Step 8)
### Step 9)

## 3. Setting up the Unity Project
### Step 1)
### Step 2)
### Step 3)
### Step 4)
### Step 5)
### Step 6)
### Step 7)
### Step 8)
### Step 9)

## 4. Creating the SerialRead script in Unity
### Step 1)
### Step 2)
### Step 3)
### Step 4)
### Step 5)
### Step 6)
### Step 7)
### Step 8)
### Step 9)

## 5. Creating an Simple Rotating Cube and UserInterface
### Step 1)
### Step 2)
### Step 3)
### Step 4)
### Step 5)
### Step 6)
### Step 7)
### Step 8)
### Step 9)
-->
