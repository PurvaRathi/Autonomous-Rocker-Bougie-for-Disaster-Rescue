# Autonomous Rocker-Bogie Vehicle for Disaster Rescue


### Overview

This project presents an **IoT-based autonomous rescue vehicle** designed using a **rocker-bogie mechanism** for navigating rough and uneven terrains typically found in disaster-hit areas. The system integrates **Raspberry Pi** and **Arduino Uno** to perform intelligent operations such as **human detection, location mapping, obstacle avoidance, and autonomous navigation**.

The primary goal is to assist rescue teams by identifying trapped individuals and sharing their locations efficiently.


###  System Architecture

 #### Raspberry Pi (High-Level Processing)

* Performs **Computer Vision (CV)** using camera input
* Detects **human presence** in disaster environments
* Extracts location data and **marks detected humans on a map**
* Sends signals/coordinates to assist rescue operations

 #### Arduino Uno (Low-Level Control)

* Handles **autonomous navigation**
* Controls **motor drivers and movement**
* Performs **obstacle detection and avoidance** using sensors
* Ensures stable traversal using rocker-bogie mechanism


###  Features

*  Autonomous movement in rough terrains
*  Real-time **human detection using computer vision**
*  Location marking for rescue teams
*  Obstacle detection and avoidance
*  IoT-based communication between modules
*  Efficient division of tasks between Raspberry Pi and Arduino


### Technologies Used

* **Hardware:**

  * Raspberry Pi
  * Arduino Uno
  * Rocker-Bogie chassis
  * Motor Drivers (e.g., L298N)
  * Ultrasonic/IR Sensors
  * Camera Module

* **Software:**

  * Python (for CV on Raspberry Pi)
  * OpenCV (for human detection)
  * Arduino IDE (C/C++)
  * IoT communication protocols


### Working Principle

1. The vehicle moves autonomously using Arduino-controlled motors.
2. Sensors continuously scan for obstacles and adjust movement.
3. The Raspberry Pi processes camera input using CV algorithms.
4. When a human is detected:

   * The system captures the location
   * Sends coordinates/pin to a map interface
5. Rescue teams can use this data for quick response.


### Applications

* Disaster rescue missions (earthquakes, landslides, floods)
* Search and rescue in hazardous environments
* Military or surveillance operations
* Remote exploration
