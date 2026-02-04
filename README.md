# AnonomousRobot
This project proposes the development of an Autonomous Visual Command Robot simulated in the
Webots environment, designed to interpret both visual and text-based commands for autonomous
decision-making. Using a Vechicle robot model, the system integrates Python and OpenCV to enable real-
time color detection and command interpretation through a lightweight rule-based NLP mechanism.
The robot perceives its surroundings via a camera sensor to identify specific colors, such as red for stop,
green for move forward, and yellow for turn and simultaneously reads an external text file containing
predefined commands like STOP, TURN LEFT, or SLOW DOWN. By combining perception from visual
cues with contextual instructions from text, the robot demonstrates autonomous control and decision-
making without human intervention during runtime. The project emphasizes simplicity and efficiency,
avoiding complex NLP frameworks while maintaining robust and interpretable behavior. The expected
outcome is a fully functional simulation showcasing how lightweight perception and text interpretation
systems can enable intelligent robotic behavior, forming a foundation for future extensions such as real-
time command input, environmental text recognition, and adaptive learning-based control.

## Autonomous Urban Navigator & Traffic System
This repository contains a comprehensive robotics simulation developed for the Webots platform. It features an autonomous vehicle capable of intelligent movement and a multi-node traffic light control system designed to simulate realistic city intersections.

### Core Architecture
The project is divided into two primary environments:

### 1. Robot Controllers
1. Autonomous Controller: A Python-based intelligence module that manages vehicle movement, sensor data, and command execution.
2. Signal Management: Custom C and Python controllers (my_traffic_light.py, generic_traffic_light.c) that handle the logic for intersection safety and timing.
3. Crossroads Logic: Specialized logic for managing complex four-way intersections.

### 2. Simulation World
1. City Environment: A high-fidelity .wbt world file representing a city layout with roads and infrastructure.
2. SUMO Integration: Includes XML configurations (sumo.net.xml, sumo.rou.xml) for advanced traffic flow simulation and vehicle routing.

### Getting Started
1. Software: Install Webots and ensure Python 3 is configured in your environment.
2. Environment Setup: Place the controllers and worlds folders within your Webots project directory.
3. Launch: Open the city.wbt file using Webots to initialize the simulation.
4. Execution: Press the 'Play' button in the simulation interface to start the autonomous vehicle and traffic cycles.

### Technical Details
1. Language Support: The system utilizes a hybrid of Python for high-level logic and C for performance-oriented hardware control.
2. Traffic Routing: Uses the SUMO (Simulation of Urban MObility) framework to define traffic demand and road networks.
