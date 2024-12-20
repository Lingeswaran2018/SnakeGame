# Snake Game - Embedded Systems Project

## Overview
This project implements a Snake Game using the **Adafruit ILI9341 display** and a **joystick** on the Wokwi simulator. The game includes interactive gameplay, multiple levels, and hardware interfacing, designed as part of the EE4360 Embedded Systems Design and Programming course at the University of Moratuwa.

## Features
### Basic Gameplay
- The snake moves based on joystick input.
- Food appears randomly on the screen:
  - Eating food increases the snake's length by one unit and adds a point to the score.
- No wall boundaries:
  - The snake reappears on the opposite edge of the screen if it moves out of bounds.
- Game ends if the snake eats its own body.

### Level Progression
1. **Level 1**: Basic gameplay.
2. **Level 2**:  
   - A digit (specific to the group) appears as a barrier:
     - Hitting the digit ends the game.
     - Food does not appear close to this digit.
   - The snake is moved to a corner if it is near the center.
3. **Level 3**:  
   - Food disappears after 5 seconds with a countdown timer displayed.
4. **Level 4**:  
   - Red food appears, reducing the score if eaten.
5. **Level 5+**:  
   - Snake speed increases by 20% with each level.
   - Additional red food items are introduced.

### Additional Features
- Interactive sound effects using a buzzer.
- Simple menu for:
  - Starting a new game.
  - Viewing the high score (saved in EEPROM).
- Joystick-controlled menu navigation.

## Development Tools
- **Simulator**: [Wokwi](https://wokwi.com/)
- **Development Framework**: PlatformIO with Arduino
- **Display**: Adafruit ILI9341
- **Programming Language**: C++
- **Libraries**: External libraries for display and joystick interfacing

## Setup Instructions
1. Clone the repository:
   ```bash
 https://github.com/Lingeswaran2018/SnakeGame.git
   ```
2. Open the project in PlatformIO within VS Code.
3. Ensure the Wokwi simulation environment is properly set up.
4. Upload the code to the Wokwi simulator or the compatible hardware setup.



## Folder Structure
- `src/`: Contains all the source code files.
- `include/`: Header files.
- `lib/`: External libraries used.
- `docs/`: Additional documentation or screenshots.
- `README.md`: This file.

## Evaluation Criteria
This project adheres to the following evaluation criteria:
- Basic Gameplay Mechanics
- Level Progression & Complexity
- Display & Joystick Interfacing
- User Interface Design
- Sound Integration
- Code Quality


