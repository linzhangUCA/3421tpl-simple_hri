# Project 1: A Naive Human-Machine Interface (HMI)

## Background
A Human-Machine Interface (HMI) is widely used in robotics and other industrial processes. It is a very useful tool for a human operator to monitor machines' status and carry out commands. In this project, we will build a basic HMI using LEDs and a switching button.

Imagine we are developing a HMI for a house cleaning robot (e.g. Roomba). We would like to 
- Indicate the robot's status using LEDs.
- Change the robot's mode using the button.

## Requirements:

### (85%) Coding
Our robot has 3 modes: **WORK, PAUSE, DEV**. We use 4 LEDs (`GREEN`, `YELLOW`, `RED`, `BLUE`) to indicate the robot's mode and battery health. The requirement is as follows: 
1. (10%) Initialization (one-time): blink all the LEDs at the same time with frequency of 4 Hz, last 2 seconds. Then the robot enters **PAUSE** mode.
2. (20%) When in **PAUSE** mode (endless loop): `GREEN` LED endlessly fades in and fades out at frequency of 1 Hz. Press and release the button to switch mode to **WORK**.
3. (20%) When in **WORK** mode (endless loop): `GREEN` LED is constantly turned on. Press and release the button to switch mode to **PAUSE**.
4. (20%) When in **WORK** or **PAUSE** mode, press and hold the button for 3 seconds to enter **DEV** mode (break the endless loop). When in **DEV** mode: `BLUE` LED is constantly turned on and other LED should be turned off. 
5. (15%) Time **WORK** mode. If the accumulated **WORK** time exceeds 15 seconds, turn on `YELLOW` LED (in **WORK** or **PAUSE** mode). If accumulated **WORK** time over 20 seconds, blink `RED` LED at frequency of 10 Hz. If `RED` LED blinked 2 seconds, then turn all the LEDs off and shutdown the system. 

### (15%) Documentation
**It is important to guide your successors with a good documentation.** Complete the following sections in this README. Please refer to [Github formatting guide](https://docs.github.com/en/get-started/writing-on-github) to get familiar with Markdown formatting.
1. (5%) Hardware Table: list the names, descriptions and quantities of physical components used in this project.
2. (5%) Wiring Diagram: attach a drawing to illustrate components connection.
3. (5%) Summary: a few words to wrap up this project.

## Hardware Table
> Name, Description, Quantity

## Wiring Diagram
> ![image name](link)

## Summary
> What has been done? What are learned? Any thoughts? Any discussions?
