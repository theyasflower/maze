# Maze Project

## About 

The spark for this game ignited during the intro to the portfolio projects and made me start reminiscing about childhood. I recollected our love for puzzles, the thrilling joy of solving mazes in magazines, and the frustration when hitting a dead-end. As I dived into these memories, I felt a strong urge to rekindle that experience, but this time with a digital twist. This project isn't just about navigating mazes; it's about recapturing those childhood joys and sharing them with the world. It took me numerous brainstorming sessions, and countless testing hours to get this game to you. And while this serves as my Portfolio Project for Holberton School, its roots lie in nostalgia.

## Desciption

The goal of this project is to create a game in 3D using raycasting. Ray-casting is a technique that transforms a limited form of data (a very simplified map or floor plan) into a 3D projection by tracing rays from the viewpoint into the viewing volume.

![maze using raycasting](/images/maze1.png)

## General Requirements

    * All your files will be compiled on Ubuntu 14.04 LTS, using gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4
    * We will use the gcc flags -Wall -Werror -Wextra and -pedantic
    * All your functions must be commented
    * Your functions should be a maximum of 40 lines long (one statement per line)
    * Your functions should be a maximum of 80 columns long
    * No more than 5 functions per file
    * Your entire repository will be checked using Betty

![door_open](/images/maze44.png)

## How It Works
   * The project first creates the window and initializes the game with some default value
   * It then displays the map and the game zone to the user
   * The user uses keys (like w, a, s, d, e & arrow keys) to move & rotate the player
   * the system continuously checks the input key provided by the user
   * if an Escape key or Quit button is tapped or clicked, it quits the game and destroys the window

## System Usage

   * Download the source file from the githbub.com into your local machine
   * Navigate to the Maze folder
   * Compile all source codes ending with .c extension using the following flag:
        gcc -Wall -Werror -Wextra -pedantic ./src/*.c -lm $(sdl2-config --cflags --libs) -lSDL2_ttf -lSDL2_image -o maze
   * Launch the executable file like ./maze if you want to use the default map
   * Launch the executable file by passing the name of the map file if you want to provide your own map like "./maze map"  Here map is the name of your file
   * The system then displays the map & the game zone on the screen
   * Press the up arrow key or w key to move the player to the upper position
   * Press the down arrow key or s key to move the player to the lower position
   * Press the left arrow key or a key to rotate the player in counter-clockwise direction
   * Press the right arrow key or d key to rotate the player in a clockwise direction
   * Press the key to open the door
   * Press the Escape key or click the Quit button to exit the game

![door_open](/images/maze33.png)

## Content of the Maze project
| File name       | Description |
---               | ---    |
main.c            | a c file which contains the main method and the display function
cast.c            | a c file which defines the main component of casting through the methods ray_cast, horizontal collision, vertical collision
drow.c            | a c file which contains methods used to draw a map, player, wall, roof & floor
map.c             | a c file which defines a map coordinates and method to access them
texture           | a c file which defines a texture value and method to access them
window            | a c file which contains method used to define the window and input keyboards
