# City Scene Animation (OpenGL + GLUT)

## Overview

This project is a **2D City Scene Animation** made using **C++**, **OpenGL**, and **GLUT**.
It shows a city environment with **day and night modes**, moving **vehicles**, **sun**, **moon**, and **clouds**.

The main goal of this project is to demonstrate:

* Basic OpenGL drawing (shapes, colors)
* Animation using 'glutTimerFunc' 
* Keyboard interaction
* Day and night scene switching

This project is suitable for **computer graphics / OpenGL coursework**.


## Features

###  Day and Night Mode

* **Day Mode**: Blue sky, sun visible, bright colors
* **Night Mode**: Dark sky, moon visible, lights turned on

You can switch modes using the keyboard:

* Press **D** → Day mode
* Press **N** → Night mode


###  Sun and  Moon Animation

* The **sun moves from left to right** during day mode
* The **moon moves from right to left** during night mode
* Sun and moon do not appear at the same time


###  Moving Clouds

* Multiple clouds move continuously across the sky
* Cloud direction and speed change based on day or night


###  Buildings

* Multiple buildings with windows
* Windows change color at night (lighted effect)
* One building contains a **cross-style design** for visual detail


###  Garden and Road

* Green garden area using half-circle grass design
* Road with:

  * Sidewalk
  * Road markings
  * Center dashed line


###  Moving Vehicles

#### Red Car

* Moves from **left to right**
* Headlight turns on at night

#### Blue Car

* Moves from **right to left**
* Headlight beam visible at night
* Rotating wheels

#### Bus

* Moves from **left to right**
* Rotating tires
* Front light visible at night

#### Cargo Truck

* Moves from **right to left**
* Headlight and rear light at night
* Detailed body and rotating wheels


## Controls

| Key   | Action               |
| ----- | -------------------- |
| D / d | Switch to Day Mode   |
| N / n | Switch to Night Mode |


## Technologies Used

* **Language**: C++
* **Graphics Library**: OpenGL
* **Utility Toolkit**: GLUT
* **Math Library**: '<math.h>'

## Program Structure (Simple Explanation)

* `circle()` → Draws a full circle
* `halfCircle()` → Draws a half circle
* Separate functions for each object:

  * `sun()`, `moon()`, `cloud()`, `bus()`, `car()`, `blueCar()`, `cargoTruck()`
* `update` functions control animation using timers
* `display()` draws the full scene
* `keyboardInput()` handles day/night switching


## How Animation Works

* `glutTimerFunc()` updates object positions
* Object movement is done using `glTranslatef()`
* Wheels rotate using `glRotatef()`
* Scene refresh uses `glutPostRedisplay()`


## How to Run

1. Make sure OpenGL and GLUT are installed
2. Compile the program using a C++ compiler
3. Run the executable
4. Press **D** or **N** to change scene mode


## Learning Outcome

From this project, we learn:

* 2D graphics drawing in OpenGL
* Animation using timer functions
* Keyboard interaction
* Scene management (day/night)
* Modular programming in graphics

## Note

This project is created for **educational purposes only** and follows simple OpenGL concepts for learning and demonstration.
