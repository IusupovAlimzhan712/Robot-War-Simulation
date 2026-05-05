# Robot-War-Simulation (C++)

## 📌 Overview
The **Robot War Simulator** is a modular, data-driven simulation system developed in C++. It models autonomous robot entities interacting within a battlefield environment using turn-based mechanics.

This project demonstrates strong application of **object-oriented programming**, **custom data structures**, and **file-driven system design**, with a focus on modularity and scalability.

---

## ⚙️ Features
- Multiple robot types with distinct behaviors and capabilities  
- Turn-based battle simulation engine  
- Dynamic robot initialization via external configuration files  
- Custom-built data structures (Queue and Linked List)  
- Modular architecture with clear separation of responsibilities  

---

## 🧠 System Architecture

### Core Components

**Simulation Engine**
- Controls execution flow and turn progression  
- Manages simulation lifecycle and termination conditions  

**Battlefield**
- Represents the environment where robots interact  
- Handles positioning, movement, and combat resolution  

**Robot System**
- Base `Robot` class with derived robot types  
- Utilizes **inheritance and polymorphism** to define behaviors  

**Data Structures**
- `RobotQueue` → manages turn scheduling  
- `RobotList` → stores and tracks active robots  

---

## 📁 Project Structure

```bash
robot-war-simulator/
│
├── src/                     # Source files
│   ├── Simulation.cpp
│   ├── Battlefield.cpp
│   ├── Robot.cpp
│   ├── UltimateRobot.cpp
│   ├── Terminator.cpp
│   ├── RoboCop.cpp
│   ├── BlueThunder.cpp
│   ├── Madbot.cpp
│   ├── RoboTank.cpp
│   ├── RobotQueue.cpp
│   └── RobotList.cpp
│
├── include/                 # Header files
│   ├── Simulation.h
│   ├── Battlefield.h
│   ├── Robot.h
│   ├── UltimateRobot.h
│   ├── Terminator.h
│   ├── RoboCop.h
│   ├── BlueThunder.h
│   ├── Madbot.h
│   ├── RoboTank.h
│   ├── RobotQueue.h
│   └── RobotList.h
│
├── config/                  # Configuration files
│   ├── battlefield_config.txt
│   └── robots_config.txt
│
├── bin/                     # Executable
│   └── RobotWar.exe
│
├── docs/                    # Documentation
│   └── report.pdf
│
├── build/                   # Build files (optional)
│
├── README.md
├── .gitignore



Getting Started

Run Precompiled Version
./bin/RobotWar.exe

Compile from Source
g++ src/*.cpp -o robot-war


Configuration System
The simulation is fully configurable through external text files located in the config/ directory.

robots_config.txt

Defines robot instances and their initial state.
./robot-war

# type name x y health
Terminator T-800 2 3 100
UltimateRobot X-01 5 6 150
RoboCop RC-1 1 2 120



battlefield_config.txt

Defines battlefield parameters such as size or rules (implementation-dependent).


✔ Benefits

* No hardcoded entities
* Flexible and reusable simulation setup
* Easily extendable for new robot types or behaviors

⸻

🧪 Simulation Workflow

1. Load configuration files
2. Initialize battlefield and robot entities
3. Insert robots into scheduling structures
4. Execute turn-based actions:
    * Movement
    * Combat
    * State updates
5. Repeat until termination condition is reached

⸻

🛠️ Technologies Used

* C++
* Object-Oriented Programming (OOP)
* Custom Data Structures
* File I/O Processing

⸻

Key Learning Outcomes

* Designed a modular simulation system with multiple interacting components
* Applied inheritance and polymorphism in a scalable class hierarchy
* Implemented custom queue and linked list structures
* Developed a data-driven architecture using external configuration files

⸻

Future Improvements

* Add visual battlefield representation (ASCII or GUI)
* Implement advanced AI strategies for robots
* Enhance input validation and error handling
* Introduce logging system for battle replay and analysis



Notes

This project was developed as part of an academic assignment and focuses on demonstrating software engineering principles, system design, and implementation techniques.


Final Remark

This project emphasizes clean structure, extensibility, and separation of concerns — key qualities expected in real-world software systems.

