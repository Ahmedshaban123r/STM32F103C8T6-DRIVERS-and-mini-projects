# STM32F1 7-Segment Counter Project

## 📌 Overview
This project demonstrates how to interface a **7-segment display** with an **STM32F1 microcontroller** using **STM32CubeIDE** and simulate it on **Proteus**.  
The program implements a **1-second delay counter** that continuously increments the displayed digit (0–9) on the 7-segment.

---

## 🛠 Tools & Technologies
- **Microcontroller:** STM32F103C8T6 (Blue Pill)  
- **IDE:** STM32CubeIDE  
- **Simulation:** Proteus 8 Professional  
- **Language:** C (HAL Library)  

---

## ⚙️ Hardware Connections
The 7-segment display is connected to **PORTA pins A0–A6**, mapped to segments `a–g`.

| Segment | Pin  |
|---------|------|
| a       | PA0  |
| b       | PA1  |
| c       | PA2  |
| d       | PA3  |
| e       | PA4  |
| f       | PA5  |
| g       | PA6  |

> ⚠️ Common Cathode 7-segment is assumed. For Common Anode, invert the logic.

---

## 🚀 Features
- Displays digits `0–9` sequentially.  
- Delay of **1 second** between updates.  
- Clean modular code with `HAL_Delay()`.  
- Fully tested on **Proteus simulation**.  

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/stm32-7seg-counter.git
Open the project in STM32CubeIDE.

Build & flash the code to your STM32F103C8T6 board (or run only on Proteus).

Open the provided Proteus simulation file (.pdsprj).

Run the simulation and observe the counting on the 7-segment display.
STM32F1-7Segment-Counter/
│── Core/
│   ├── Inc/
│   │   └── main.h
│   ├── Src/
│   │   └── main.c
│── Proteus/
│   └── 7seg_counter.pdsprj
│── README.md
