# Project 1: A Naive Human-Machine Interface (HMI)

## Background
A Human-Machine Interface (HMI) is widely used in robotic applications (See Roomba's HMI below). It allows humans to easily interact with machines. An HMI usually provides information about a machine's status, as well as executes command from human operators. In this project, we will build a basic HMI using LEDs and a tactile switch button.

![roomba_hmi](https://miro.medium.com/v2/resize:fit:640/format:webp/1*nLjM3CHVIxvbTAc3EuUpvg.gif)

## Requirements:
1. Imagine we are developing an HMI for a house cleaning robot (e.g. Roomba). Code a Raspberry Pi Pico to: 
    - Indicate the robot's status using the LEDs.
    - Switch the robot's working modes using the button.
2. Document this project.

### (85%) Coding
> Upload your script to this repository.

- The robot has 2 modes: **WORK MODE, PAUSE MODE**.
- Use the tactile button to switch among the modes.
- Use 3 LEDs (`GREEN`, `YELLOW`, `RED`) to indicate the robot's status.

Refer to the following steps to code:
1. (10%) Initialization (_hint: one-time_): blink all the LEDs at the same time with frequency of 5 Hz, last 2 seconds. Then the robot enters **PAUSE MODE**.
2. (20%) When **PAUSE MODE** is activated: `GREEN` LED fades in and fades out at frequency of 1 Hz. Press the button to ***immediately*** switch to the **WORK MODE**.
3. (20%) When **WORK MODE** is activated: `GREEN` LED stays constantly on. Press the button to switch back to the **PAUSE MODE**.
4. (20%) Time **WORK MODE**. If the accumulated **WORK MODE** time exceeds 45 seconds, turn on `YELLOW` LED. If accumulated **WORK MODE** time over 55 seconds, blink `RED` LED at frequency of 10 Hz.
5. (15%) Termination: turn off everything (_hint: break the endless loop_) if `RED` LED blinked 5 seconds, or **press and hold**_ the button for 3 seconds. 

**NOTE**: 
- Mode switching is NOT a one-time function. Make sure you can switch between the modes back and forth.
- The `YELLOW` LED and the `RED` LED are suppose to functional in both **WORK MODE** and **PAUSE MODE**
- Once the system is shutdown (terminated), LEDs should not be able to turned back on any more. And pressing the button will no longer cause any consequences.

### (15%) Documentation
**It is important to guide other people with a good documents.** Complete the following sections in this README. Please refer to [Github formatting guide](https://docs.github.com/en/get-started/writing-on-github) to get familiar with Markdown formatting.
1. (5%) Hardware Table: list the names, descriptions and quantities of physical components used in this project.
2. (5%) Wiring Diagram: attach a drawing to illustrate components connection.
3. (5%) Summary: a few words to wrap up this project.

## Hardware Table
| Name | Description | Quantity |
| :--- | :---        |  :---:   |
|      |             |          |
|      |             |          |

## Wiring Diagram
![image name](link)

## Usage Instructions
> Use bulleted or indexed steps to instruct users of your product.
