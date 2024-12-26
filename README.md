MOBILE GAME DEVELOPMENT FINAL PROJECT REPORT
TOPIC: Romp of Mazes (Maze Adventure Game)

-------------------------------------------------------
GAME DESIGN DOCUMENT (GDD) TEMPLATE
Game Name: Romp of Mazes
Genre: 2D Adventure Game

-------------------------------------------------------
Game Elements
There are 2D game objects such as walls, doors, keys, players, slimes, etc.

Player: Only one player can play the game at a time.

-------------------------------------------------------
TECHNICAL SPECIFICATIONS
Technical Form: The game consists of 2D objects like walls, doors, keys, players, and slimes.

View: Romp of Mazes is a 2D game offering a top-down view of characters and objects like walls, doors, and other elements.

Platform: Currently, the game is designed to run on PCs with the required specifications. It can be updated to run on Android, iOS, and Mac devices with minor adjustments.

Language: C# is used in the scripts to control player movement and handle specific actions when conditions are met.

Device: PC

-------------------------------------------------------
GAMEPLAY
Romp of Mazes is a single-player game where the user controls the player's movements. The game consists of complex mazes separated by levels. Upon completing one level, the player advances to the next. The ultimate objective is to save the princess.

Game Objects: Walls, doors, keys, and slimes (enemies).

Objective:

Avoid slimes.
Collect keys.
Open doors.
Navigate through the maze to save the princess.
Victory Condition: When the player reaches and touches the princess, the game ends, displaying a “You Win” screen. Players can then restart the game from the beginning.

Exit Option: Players can exit the game at any time by pressing the Escape key.

Gameplay Outline:

Open the game application.
Select the "Play" option.
Load game objects.
Move the player.
Collect keys.
Open doors.
Pass levels.
Save the princess.
Finish the game.
Replay or quit.

-------------------------------------------------------
Key Features
Goal: Save the princess after overcoming all challenges.
Challenge: Difficulty increases with each level.
No Retry for Entire Game: Players must restart a level upon failing, but progress within the game is continuous.

-------------------------------------------------------
DESIGN DOCUMENT
Walls:

Rigid game objects that limit player motion.
Arranged to form the maze (prefabs).
Doors:

Prevent players from progressing to the next level.
Destroyed when the required keys are collected.
Keys:

Collected by the player in each level.
Upon collection, the key disappears. All keys must be collected to destroy the door and advance to the next level.
Slimes:

Act as enemies.
Move along predefined paths in loops.
Colliding with a slime destroys the player and restarts the current level.
Player:

Controlled by the user to navigate the maze, avoid slimes, and collect keys.
The player's objective is to save the princess.

-------------------------------------------------------
DESIGN GUIDELINES
All game objects must have a Rigidbody and Collider attached for collision-based gameplay mechanics.
The player must collect all keys and avoid slimes to complete each level.

-------------------------------------------------------
GAME DESIGN DEFINITIONS
Win State: When the player touches the princess, the game displays a “You Win” screen.
No Lose State: Upon failure (colliding with a slime), the level restarts automatically.
Level Progression: Collect all keys, open the door, and pass through to the next level.

-------------------------------------------------------
PLAYER DEFINITION
The player moves using keyboard controls (A, D, W, S) and interacts with the game environment.

Player Properties:

Tag: Used in scripts to reference the player.
Sprite Renderer: Renders the player sprite.
Box Collider: Enables collision detection.
Rigidbody: Adds physical properties.
Audio Source: Plays sounds when interacting with keys or slimes.
Movement Script: Governs the player's movement.
Player Mechanics:

Touch all three keys to destroy the door and advance to the next level.
Avoid slimes to avoid restarting the level.

-------------------------------------------------------
USER INTERFACE (UI)
The UI is minimal:

Keyboard Controls: A, D for horizontal movement, and W, S for vertical movement.
Buttons: Present in start and end scenes to initiate gameplay or quit.
Escape Key: Allows players to pause or quit.

-------------------------------------------------------
FUTURE SCOPE
The game can be improved by:

Adding more levels.
Refining the UI.
Providing players with more control options.
