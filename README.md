# AI Driver for TORCS – Autonomous Racing Controller

Team project for the **Artificial Intelligence** course: a Java client for the TORCS racing simulator (Simulated Car Racing championship protocol) that drives a car autonomously using sensor data.

## What it does
- **Rule-based driver** (`SimpleDriver.java`): computes steering, acceleration/braking, gear shifting and clutch from track-edge sensors, with ABS filter and automatic recovery when the car is stuck.
- **Data collection** (`FileService.java`): logs sensor readings (speed, track position, edge sensors, RPM, …) together with the driver's actions to build a training dataset.
- **Learning-based driving** (`Sample.java`, `KDTree.java`): K-Nearest Neighbours classifier on a KD-Tree, mapping the current sensor state to the most similar recorded situations to choose the next action.
- **Simulator communication** (`Client.java`, `SocketHandler.java`, `MessageParser.java`): socket connection and parsing of the TORCS sensor messages.

## Tech stack
Java · TORCS / SCR · KNN · KD-Tree · Sockets

## Team
University team project. Original repository: [gerdo16/ai_project](https://github.com/gerdo16/ai_project) – this fork is kept as part of my portfolio.

Team member: **Maria Pia Pagano**
