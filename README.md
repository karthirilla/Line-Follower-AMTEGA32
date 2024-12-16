# Line Follower Robot with ATmega32

The **Line Follower Robot with ATmega32** is an advanced, high-performance robot designed to autonomously follow a line path with precision. Equipped with 16 sensors, a MOSFET-based motor driver, and intelligent control algorithms, this robot is ideal for educational, research, and competition purposes.

Built around the ATmega32 microcontroller, it integrates advanced features such as auto-calibration, optimized path planning, maze-solving capabilities, and Bluetooth Low Energy (BLE) control. The robot's motor system is designed to provide enhanced torque with 24,000 RPM motors, ensuring superior performance in competitive environments.

# Line Follower ATMEGA32

## Images

| **Image 1**                                                               | **Image 2**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 1](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_1.jpg) | ![Image 2](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_2.jpg) |

| **Image 3**                                                               | **Image 4**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 3](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_3.jpg) | ![Image 4](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_4.jpg) |

| **Image 5**                                                               | **Image 6**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 5](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_5.jpg) | ![Image 6](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_6.jpg) |

| **Image 7**                                                               | **Image 8**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 7](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_7.jpg) | ![Image 8](https://github.com/karthirilla/Line_Follower_AMTEGA32/blob/main/LINE_FOLLOWER_ATMEGA32_8.png) |


## Features

### 1. Hardware
- **Microcontroller**: ATmega32
- **Sensors**: 16 Photodiode/IR-based sensors for precise black-and-white line detection
- **Motor Driver**: MOSFET-based motor driver for efficient and high-torque motor control
- **Motors**: DC Motor (24mm, 24,000 RPM) for enhanced speed and torque
- **Battery**: Inbuilt 12V rechargeable battery for autonomous operation
- **Display**: 16x2 LCD for displaying data and settings
- **Motor Driver MOSFET**: High-efficiency motor control for increased torque

### 2. Software Features
- **Auto Calibration**: Automatically adjusts the sensors for varying lighting and track conditions
- **Advanced Path Planning**: Optimized for complex curves, sharp turns, intersections, and advanced path-following algorithms
- **Maze Solver**: Automatically solves maze-type tracks, finding the optimal path from start to finish
- **Memory Management**: 
  - Dual External EEPROM (256 Kbit each) for memory storage
  - 31 Memory Slots for storing track plans
  - Features to Copy, Insert, Mirror, Delete between memory tracks
  - Auto/Manual Mirror Memory for creating mirrored paths easily
- **Control System**:
  - PID Control for smooth and precise movements
  - Plug and Play Mode: Supports Wireless Manual Control via Bluetooth Low Energy (BLE)

## System Architecture

### Components
| Component        | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Microcontroller** | ATmega32                                                                    |
| **Sensors**         | 16 Photodiodes/IR sensors for black/white detection                          |
| **Motor Driver**    | MOSFET-based Motor Driver for high-efficiency and torque control            |
| **Motors**          | 24mm DC Motors, 24,000 RPM, high torque                                    |
| **Display**         | 16x2 LCD                                                                     |
| **Battery**         | 12V rechargeable battery                                                     |
| **External Memory** | Dual 256Kbit EEPROM                                                          |
| **Wireless Control** | Bluetooth Low Energy (BLE) module for manual wireless control               |

### Software Tools
- **Arduino IDE**: Programming the ATmega32 microcontroller
- **CodeVision AVR**: Advanced AVR programming and debugging
- **AVRDUDESS**: Flashing firmware onto the ATmega32 microcontroller
- **DipTrace**: PCB design software for schematic and layout
- **Proteus**: Circuit simulation for testing and validation

## Features Breakdown

### Sensors
- **16 Photodiodes/IR Sensors**: Provides high accuracy for detecting black and white lines, even in challenging lighting conditions.

### Calibration
- **Auto Calibration**: Automatically adjusts sensitivity based on track conditions to ensure consistent performance.

### Memory Management
- **Dual EEPROM**: Stores up to 31 track paths with features to copy, insert, mirror, delete, and manage memory tracks.
- **Auto/Manual Mirror Mode**: Allows quick creation of mirrored paths.

### Path Control
- **PID Controller**: Ensures smooth and precise line-following by dynamically adjusting motor speed and direction.
- **Advanced Path Planning**: Optimized for handling complex curves, sharp turns, intersections, and dynamic track changes.
- **Maze Solver**: Uses advanced algorithms to automatically solve maze-type paths, ensuring the robot can find the optimal route from start to finish.

### Motor and Driver
- **MOSFET-based Motor Driver**: High-efficiency motor control that enables high torque and smooth motion.
- **Motors**: 24mm DC motors with a speed of 24,000 RPM, providing superior torque and fast movements.

### Display and Wireless
- **16x2 LCD**: Displays runtime parameters, settings, and calibration data.
- **Bluetooth Low Energy (BLE) Control**: Allows wireless manual control using a mobile app or Bluetooth terminal for full control and adjustments.

## Circuit Design and Simulation
- **PCB Design**: Created using DipTrace for the ATmega32 and MOSFET-based motor driver circuit.
- **Simulation**: Simulated in Proteus to test the logic and hardware before physical assembly.

## Getting Started

### Prerequisites
Before starting, make sure to install the following software:
- **Arduino IDE**
- **CodeVision AVR**
- **AVRDUDESS**
- **DipTrace**
- **Proteus**

### Hardware Setup
Assemble the hardware components as per the provided PCB design.

### Steps to Run
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/Line-Follower-ATmega32.git
    ```
2. **Upload Code**: 
   - Upload the firmware to the ATmega32 using Arduino IDE or CodeVision AVR.
3. **Calibrate Sensors**:
   - Use the auto-calibration feature to set up the robot for the specific track.
4. **Run the Robot**:
   - Place the robot on the track and let it follow the line autonomously or control it manually via BLE.

## Future Enhancements
- Add **Obstacle Detection** using ultrasonic sensors.
- Implement **Speed Optimization** algorithms for racing competitions.
- Integrate **Wi-Fi Control** for enhanced remote monitoring and control.
- Expand memory capabilities for more track storage.
- Add **Voice Commands** using advanced Bluetooth modules.

## License
This project is licensed under the **MIT License**. See the LICENSE file for details.

## Acknowledgments
- Special thanks to the open-source community for the libraries and tools used in this project.
- Inspired by academic projects and robotics competitions.

## Contact
For any inquiries, feel free to reach out:

- Email: [karthikrilla@gmail.com](mailto:karthikrilla@gmail.com)
- LinkedIn: [Karthi C](https://www.linkedin.com/in/karthic)
