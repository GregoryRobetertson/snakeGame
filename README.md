Core Features and Logic:
DOM Manipulation: The game dynamically updates the DOM to draw the snake and food using createElement, setPosition, and grid-based layout.

Game Board Setup: Elements like the score display, instruction text, and board area are initialized using getElementById.

Snake Movement: The snake moves on a 20x20 grid in one of four directions (up, down, left, right). Movement is handled by updating the snake’s head position and redrawing it on each interval tick.

Food Mechanics: When the snake's head reaches the food location, a new food piece is generated at a random grid position, and the snake grows.

Speed Increase: As the snake eats more, the game speeds up gradually by reducing the interval delay (gameSpeedDelay).

Collision Detection: The game checks if the snake hits the wall or itself. If so, it resets and updates the high score.

Game Start/Reset: The game starts when the user presses the spacebar. It can reset automatically after a collision.

Score Tracking: Tracks both current score and high score and displays them using padded zero formatting for a retro arcade feel.

Clean Separation of Logic: Functions like drawSnake, move, checkCollision, increaseSpeed, and updateScore are modular, making the code easier to maintain and expand.
