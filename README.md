# Msebetsi_Solutions_Kids

Msebetsi Solutions Space Kids Game
Introduction
Welcome to the Msebetsi Solutions Space Kids Game! This game is a space-themed shooter where players control a spaceship, navigate through levels, and defeat waves of enemies.


Table of Contents
Introduction
Installation
How to Play
Game Mechanics



Installation
Clone the Repository
git clone https://github.com/yourusername/space-kids-game.git

Navigate to the project directory:
cd space-kids-game

Install the required dependencies:
Make sure you have Python and pip installed. Then, run:
pip install pygame

Ensure the assets are in place:
Ensure the assets directory is in the project folder and contains all necessary images:
pixel_ship_red_small.png
pixel_ship_green_small.png
pixel_ship_blue_small.png
pixel_ship_yellow.png
pixel_laser_red.png
pixel_laser_green.png
pixel_laser_blue.png
pixel_laser_yellow.png
background-black.png


How to Play
Run the Game:
Execute the following command in your terminal:
python main.py
Game Controls:

Move Left: A key
Move Right: D key
Move Up: W key
Move Down: S key
Shoot: SPACE key
Objective:

Navigate your spaceship to avoid enemy ships and lasers.
Shoot down enemy ships to progress through levels.
Survive as long as possible with the given lives and health.
Game Mechanics
Classes and Their Functions
Laser Class:

__init__(self, x, y, img): Initializes the laser.
draw(self, window): Draws the laser on the window.
move(self, vel): Moves the laser by a given velocity.
off_screen(self, height): Checks if the laser is off the screen.
collision(self, obj): Checks if the laser collides with an object.
Ship Class:

__init__(self, x, y, health=100): Initializes the ship with position and health.
draw(self, window): Draws the ship on the window.
move_lasers(self, vel, obj): Moves the ship's lasers and checks for collisions.
cooldown(self): Manages the shooting cooldown.
shoot(self): Fires a laser if not in cooldown.
get_width(self): Returns the width of the ship.
get_height(self): Returns the height of the ship.
Player Class (inherits from Ship):

__init__(self, x, y, health=100): Initializes the player with position and health.
move_lasers(self, vel, objs): Moves the player's lasers and checks for collisions with enemies.
draw(self, window): Draws the player and its health bar on the window.
healthbar(self, window): Draws the player's health bar.
Enemy Class (inherits from Ship):

__init__(self, x, y, color, health=100): Initializes the enemy with position, color, and health.
move(self, vel): Moves the enemy ship by a given velocity.
shoot(self): Fires a laser if not in cooldown.
Main Functions
collide(obj1, obj2): Checks for a collision between two objects.
main(): The main game loop managing the game state, player input, and updates.
main_menu(): Displays the main menu and starts the game when prompted.
Credits
Game Development: Msebetsi Solutions
Libraries Used: Pygame
Assets: Various assets used in this game (images and fonts) are credited to their respective creators.
