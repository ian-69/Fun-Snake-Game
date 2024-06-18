# Fun-Snake-Game
This is a Snake game Program. The program allows the player to control a snake that moves 
around the screen to collect apples while avoiding obstacles. The game has three main 
states: MENU, PLAYING, and GAME_OVER. In the MENU state, the player can start the game 
or quit. In the PLAYING state, the player controls the snake's movement to collect apples 
and avoid obstacles. When the snake collides with an obstacle, the game transitions to the 
GAME_OVER state, displaying the player's score and allowing them to restart or quit.

HOW THE FUNCTIONS AND PROCEDURES ARE ACTUALLY WORKING

Functions and Procedures:

• void update_snake(snake &s): Updates the snake's position and movement. It 
calculates the new position of the snake's head based on the direction and speed, 
shifts the positions of body segments to create movement, and handles screen edge 
wrapping and collision with the snake's body.

• bool has_collided_with_apple(const snake &s, const apple &a): Checks if the snake 
has collided with an apple by comparing the distance between the snake's head and 
the apple's position.

• bool has_collided_with_obstacle(const snake &s, const obstacle &o): Checks if the 
snake has collided with an obstacle by comparing the distance between the snake's 
head and the obstacle's position.

• void generate_new_item(point &item): Generates a new random position for an 
item (apple or obstacle) within the screen bounds.

• void draw_menu(): Draws the main menu screen, including background, title, and 
instructions.
• void draw_game_over(int score): Draws the game over screen with the player's 
score and options to play again or quit.
• int main(): The main function where the game logic resides. It initializes the game 
window, resources, and the game loop. It handles user input, updates the game 
state, and draws the game elements based on the current state (MENU, PLAYING, or 
GAME_OVER).
