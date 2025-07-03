# Bidirectional-Visitor-Counter (using Arduino Uno)
This project implements a bidirectional visitor counter using an Arduino Uno. It counts the number of people entering and exiting a room using two IR sensors. The count is displayed on a 16x2 LCD screen via the I2C interface. This system is useful for applications like room occupancy tracking, event halls, libraries, or any place where knowing the number of people is important.

## Features
- Counts people entering and exiting through a single passage
- Uses two IR sensors to detect direction of movement
- Displays current count on LCD in real-time
- Resets counter if it goes below zero
- Compact and efficient code
- User-friendly interface

## Components Used

| Component              | Quantity  |
| ---------------------- | --------- |
| Arduino Uno            | 1         |
| IR Sensors             | 2         |
| 16x2 LCD Display (I2C) | 1         |
| I2C Module             | 1         |
| Jumper Wires           | As needed |
| Breadboard             | 1         |
| USB Cable              | 1         |

## Working Principle
- Entry Detection:

   - If IR Sensor 1 is triggered before Sensor 2, the system assumes a person has entered.

   - Visitor count is incremented.

- Exit Detection:

  - If IR Sensor 2 is triggered before Sensor 1, it assumes a person has exited.

  - Visitor count is decremented.

- The current count is updated and displayed on the 16x2 LCD.
