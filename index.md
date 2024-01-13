# Kailas B. Kahler's "website"

## Hello!

<img src="me.jpg" width="500">

My name is Kailas B. Kahler, and I am currently an undergraduate at MIT, in the class of 2024, studying course 6-2 (Electrical Engineering and Computer Science).
I plan to return to MIT for an additional year to complete an MEng degree in 2025.

Outside of academics, I am also an avid tennis player (playing on the varsity team at MIT) and skier, and like spending time outdoors, especially in the cold and snow.

If you are looking to get in touch, I can be reached at [kailasbk@mit.edu](mailto:kailasbk@mit.edu).

## My Projects

Below is a compilation of technical projects, including personal, academic, and professional, that I have worked on, in order of most recent to least.

### Automatic Mesh-LODs
*Final Project for 6.4400(6.837): Computer Graphics*

In this class, assignments were completed in C++ using a OpenGL wrapper developed for the course.
Assignments included implementing Bezier and B-spline curves and surfaces, skeletal subspace deformation, phyiscally-based simulations, a ray tracer, and shadow mapping for rasterized rendering.
Inspired by UE5's Nanite system, I chose to make a automatic mesh level-of-detail system for my final project.
It includes both a mesh simplifier based on the Garland and Heckbert's quadric error metric, and a LOD selector based on projected error.

 - date: December 2023
 - collaborators: none
 - demo: [video](https://youtu.be/4kjIwtg-ffA)
 - report: [pdf](6_4400_project_report.pdf)


### FPGA-360: a 3D model viewer on an FPGA
*Final Project for 6.205(6.111): Digital Systems Laboratory*

In this class, assignments were completed in SystemVerilog and deployed to Xilinx FPGAs.
Sample lab assignment tasks included a decoder for a PS/2 keyboard, a VGA controller, and an Ethernet NIC.
The class concluded with a open-ended final project, and my partner and I decided to create a 3D model viewer which would render arbitrary 3D meshes to a monitor and provide controls to move the camera view of the scene.
Models in the OBJ file format can be uploaded to the FPGA over UART via a Python script.
The graphics pipeline then renders the model in 320x240 pixel resolution in RGB color.
The view of the scene can be adjusted by using two joysticks which are connected to the integrated analog-digital-coverters on the FPGA board.

 - date: November 2022
 - collaborators: Ritik Patnaik
 - contribution: implemented most of the floating point units, graphics pipeline and framebuffer module
 - code: [github.com/kailasbk/fpga-360](https://github.com/kailasbk/fpga-360)
 - demo: [video](https://youtu.be/IygtqOMrrTU)
 - report: [pdf](fpga_360_report.pdf)
  
### MITScript Bytecode Interpreter
*Final Project for 6.1120(6.818): Dynamic Computer Language Engineering*

The main assignment in this class was a group project where the task was to create, from scratch using only the C++ standard library and the ANTLR4 lexer libary, a bytecode interpreter for the MITScript language.
The MITScript language is a dynamic computer language that includes features such as if/else statements, loops, and functions, along with datatypes like booleans, integers, strings, dictionaries, and closures.
The bytecode interpreter includes a compiler from MITScript code first to an abstract syntax tree and then to an internal bytecode representation, which is executed by a bytecode virtual machine that includes a garbage collector.
The final phase of the project included adding various performance optimizations to the interpreter to improve overall performance on a set of sample benchmarks.

 - date: October 2022
 - collaborators: Jeremiah DeGreeff, Danny Mittal
 - contribution: implemented compilation from abstract syntax tree to bytecode, virtual machine stack optimizations, threaded code, and added a control-flow graph to compilation flow to enable optimizations like null-sequence removal
 - results: ranked #2 in the class performance derby with the maximum score

### Mini-Engine: a mininal game engine
*Personal Project*

Starting in the summer of 2022, I worked on a personal graphics and game engine project, which I call *mini-engine*.
The project is programmed in C++, and uses the SDL2 and GLEW libaries.
The goal of the project was to learn OpenGL, and later Vulkan, by creating a minimal game engine.
The engine provides a rendering interface which is agnostic of the graphics API, and the first implementation uses OpenGL 4.6, with plans to make a Vulkan version in the future.
The engine also provides event-based user input and an entity-component-system framework for writing game logic.

 - date: June 2022
 - collaborators: none
 - code: [github.com/kailasbk/mini-engine](https://github.com/kailasbk/mini-engine)
 - demo: [windows executable](https://github.com/kailasbk/mini-engine/releases/tag/demo-v0.0)

### Internet Chess
*Final Project for 6.08: Intro to EECS via Interconnected Embedded Systems*

This class focused on building embedded systems using an ESP32 microcontroller connecting to various peripherals like buttons, a TFT display, and a speaker, and to the Internet for further interactivity.
For the final project, my group developed an chess game that would allow two microcontroller-based consoles to play against each other remotely over the Internet.
The system allowed for players to join games either against specified opponents, or through a ranked matchmaking queue.
In addition, there was a spectator website where games could be watched from a web browser on a computer.

 - date: April 2021
 - collaborators: Monica Busza, Manuel Valencia, Ryan Yang, Kartikesh Mishra
 - contribution: implemented server API endpoints for joining games and taking turns in Python, reviewed C/C++ code for the ESP32, made the spectator webpage with HTML and JavaScript
 - demo: [video](https://www.youtube.com/watch?v=2V3sLyXiYjc)


### Kaido: a Pokerbot
*Submission for 6.176: Pokerbots Competition*

For the 2021 MIT Pokerbots competition, the game was heads-up Texas hold'em poker, with bots competing in 1v1 matchups and ranked by an ELO system.
Our bot, named Kaido, was implemented using Python, after a brief attempt in C++.
The first iteration of our bot played by comparing pot odds to the likelihood of winning the hand as determined by Monte-Carlo simulations.
In a second iteration, to learn how to best play different hands and scenarios, the bot was trained by playing against itself repeatedly and adjusting its strategy towards an optimal one by attempting to minimize counter-factual regret.

 - date: January 2021
 - collaborators: Mehrab Jamee
 - contribution: implemented counter-factual regret training model, implemented original Monte-Carlo simulation based model
 - code: [github.com/kailasbk/pokerbots-21](https://github.com/kailasbk/pokerbots-21)
 - results: bot peaked at #1 on the live standings, finished #9 in final standings

### Pronouncit: a web app for learning names
*Senior Project*

For my high school senior project, I created a web application to solve an issue I often face: my name being mispronounced.
The app, called *pronouncit*, draws off of the flashcard and studying website Quizlet, but includes additions to make it more suited for learning names.
The frontend of the application was programmed using React, while the backend was programmed using ExpressJS and stored user data in a PostgreSQL database.
Users can make accounts with their name, profile picture and email address, and they can then upload a recording of how to properly pronounce their name.

 - date: May 2020
 - collaborators: none
 - code (frontend): [github.com/kailasbk/pronounce-web](https://github.com/kailasbk/pronounce-web)
 - code (backend): [github.com/kailasbk/pronounce-api](https://github.com/kailasbk/pronounce-api)
 - presentation: [video](https://youtu.be/dKFUNTD7mCg)

<meta name="robots" content="noindex,nofollow">
