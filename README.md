CAP-3
1. Game Initialization:
The game initializes a Pygame window with a width of 600 pixels and a height of 400 pixels.
It creates a screen object representing the game window.
Sixteen obstacles are generated as rectangles with random positions within the window.
A starting point for a line is set at the center of the window.

2. Collision Detection Function:

The detect_collision function takes an obstacle (rectangle), a starting point for a line (line_start), and an ending point for the line (mouse_pos).
It uses the clipline method of the Pygame Rect class to check if the line intersects with the obstacle.

3. Unit Tests:

The TestCollisionGame class is a subclass of unittest.TestCase and includes two test methods.
test_initialize_game checks if the initialization function returns objects of the correct types (Pygame Surface, list, and tuple).
test_detect_collision tests the collision detection function with two scenarios: one where there should be a collision and one where there should not be.

4. Running Tests:

The script checks if it's being run directly (__name__ == '__main__') and, if so, executes the unit tests using unittest.main().
