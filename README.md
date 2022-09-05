# Project 1 A Naive Human-Machine Interface (HMI)

## Background
A Human-Machine Interface (HMI) is widely used in indutrial robots and other industrial processes. It is a very useful tool for a human operator to monitor a device's status, visualize data and carry out commands. In this project, we will build a basic HMI using some low-cost components.

Imagine we are developing a HMI for a house cleaning robot (e.g. Roomba). We would like to 
- Indicate robot's status using LEDs.
- Change robot's working mode using switch buttons.

## Requirements:

### (85%) Programming
Our robot has 3 modes: **WORK, PAUSE, DEV**. We use 4 LEDs (`GREEN`, `YELLOW`, `RED`, `BLUE`) to indicate the robot mode and status. 
1. (10%) Initialize the robot: blink all the LEDs at the same time with frequency of 4 Hz, last 2 seconds. Then the robot enters **PAUSE** mode.
2. (20%) When in **PAUSE** mode: `GREEN` LED endlessly fades in and fades out with frequency of 1 Hz. Press and release the button to switch mode to **WORK**.
3. (20%) When in **WORK** mode: `GREEN` LED is constantly turned on. Press and release the button to switch mode to **PAUSE**.
4. (20%) No matter in **WORK** or **PAUSE** mode, press and hold the button for 3 seconds to enter **DEV** mode. When in **DEV** mode, `BLUE` LED is constantly turned on and other LED should be turned off. 
5. (15%) Time **WORK** mode. If the accumulated **WORK** time exceeds 15 seconds, turn on `YELLOW` LED (in **WORK** or **PAUSE** mode). If accumulated **WORK** time over 20 seconds, blink `RED` LED with frequency of 10 Hz for 2 seconds, then turn all the LEDs off and shutdown the system.

### (15%) Documentation
Complete the following sections in this README. Please refer to [Github formatting guide](https://docs.github.com/en/get-started/writing-on-github).

## (5%) Hardware Table
> Name, Description, Quantity

## (5%) Wiring Diagram

## (5%) Summary
