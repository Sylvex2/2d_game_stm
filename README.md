1. Project description 
The project consists of the design and implementation of an Embedded Maze Game developed on 
the STM32L476RG (Nucleo) platform. This application integrates hardware control, serial 
communication (SPI), and real-time game logic to provide an interactive user experience. 
Project Overview 
The main objective of the game is for the player to navigate a character through a maze, starting 
from a fixed point and reaching a target destination. The game utilizes an ST7735 color LCD (128x128 
resolution) for the graphical interface and four physical push-buttons for directional movement. 
Core Functionalities 
• Startup Menu: Upon power-up, the system displays a "START JOC" screen on a yellow 
background. The game remains in standby until any button is pressed. 
• Maze Navigation: The player controls the character's movement (Up, Down, Left, Right) 
using buttons connected to the GPIOB and GPIOC ports. 
• Heads-Up Display (HUD): A dedicated status bar at the top of the screen tracks and displays 
the elapsed time in seconds and the total number of steps taken by the player. 
• Audio Feedback: A piezo buzzer, controlled via bit-banging on the PA10 pin, provides 
auditory cues for the start of the game and a celebratory melody upon reaching the goal. 
• Victory Condition: When the player reaches the predefined goal coordinates, the screen 
turns green and displays "VICTORIE!", and the game enters a finished state. 
