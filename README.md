# Digital Coin Counter

An embedded system designed to automatically detect and count coins of different values, displaying the running total on an LCD screen. The system provides feedback through LEDs and a reset mechanism when the maximum sum is reached, making it a practical and interactive solution for managing coins.

## Features
- Detects multiple coin types (1, 5, 10, 50 bani) using dedicated sensors  
- Real-time total displayed on an LCD (I2C)  
- LED indicators for system status (green = active, red = full)  
- Reset button to restart the counting process when the maximum sum is reached  
- Modular C++ classes for sensor management and sum calculation  

## Components
- Arduino-compatible microcontroller  
- 4 sensors (one for each coin type)  
- LCD I2C module  
- LEDs (green and red)  
- Push button  
- USB connection  

## Demo
🎥 Watch the full project demonstration on YouTube:  
👉 https://youtu.be/nvCHDwIAAuY

## Code
The code is written in **C++ for Arduino**, with separate classes for sensors and sum management.  
You can find the full implementation in the repository under `src/`.

## How It Works
1. Insert a coin – the corresponding sensor is triggered.  
2. The system adds the coin’s value to the running total.  
3. The LCD displays the current amount in **lei.bani** format.  
4. When the maximum sum is reached, the green LED turns off, the red LED turns on, and a message prompts to empty the box.  
5. Press the reset button to restart counting from zero.  
