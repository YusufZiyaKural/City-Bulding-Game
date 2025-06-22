# Basic City Building Simulation Game (Console-Based, C++)

A **primitive console-based construction and management simulation (CMS) game** written in C++. Players can build cities, manage resources, and make strategic decisions to grow their urban space within a simple yet functional terminal interface.

---

## Game Description

This project simulates the core mechanics of a city builder game where players can:

- Place buildings on a 60x20 grid map
- Manage limited actions per round (turn-based system)
- Control income and happiness based on building proximity and types
- Interact entirely via the console using C++ standard input/output

---

## Game Features

- **City Grid Map (60x20):** The game board where all constructions are placed.
- **Buildings Available:**
  - House
  - Hospital
  - School
  - Lumberjack
  - Mine
- **Key Mechanics:**
  - Buildings generate money or happiness based on type and location.
  - Hospitals and schools increase happiness of nearby houses (within a 5x5 range).
  - Lumberjacks and mines generate money per action.
  - Limited to **5 actions per turn** (Tour).
- **Game Loop:**
  - Input coordinates and building type
  - Map updates and displays
  - Income and happiness are recalculated
  - Game ends when player inputs `q`

---

## 📂 Project Structure

````
CityBuilderGame/
├── src/
│ ├── main.cpp
│ ├── map.h / map.cpp
│ ├── basebuilding.h / basebuilding.cpp
│ ├── house.cpp / hospital.cpp / school.cpp
│ ├── mine.cpp / lumberjack.cpp
│ └── utils/
│ └── inputhandler.cpp
├── UML_Diagram.pdf
├── .gitignore
├── README.md
└── LICENSE
````
[Whole Program UML + FC.pdf](https://github.com/user-attachments/files/20854866/Whole.Program.UML.%2B.FC.pdf)

## How to Play

1. **Compile the program:**
   ```bash
   g++ -o citygame src/*.cpp

2. **Run the game:**
   ````
   ./citygame
   ````
2. **Commands:**
-Input a building type (e.g., h for house, m for mine, etc.)

-Then provide x and y coordinates

-Repeat until q is entered to quit

---

## **Sample Gameplay**
````
Enter building type (h/m/s/l/p/q): h
Enter x coordinate: 5
Enter y coordinate: 10
Building placed at (5,10)

Current Income: 120
Happiness Score: 35%
...
````
---

## **Authors**
Developed by:

-Dirsehan Başaran

-Yusuf Ziya Kural

-Gökmen Veyisoğlu



