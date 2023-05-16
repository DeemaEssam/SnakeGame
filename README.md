****************************************# SnakeGame**************************************
*****************************************************************************************

The SnakeGame class is a JavaFX application
that implements the classic Snake game. The game consists of a snake that moves around the game board
and eats food that appears randomly on the board. The game ends when the snake collides with the wall or
with its own body. The class has a set of constants and variables that define the game’s behavior and state,
including the speed of the snake, the size of the game board, the snake’s position and direction, and the
location and color of the food. The class also has a nested Corner class that represents a single cell of the
game board, and a nested Speedup class that can be used to increase the speed of the snake as the player’s
score increases. The class has two methods: start, which creates the game’s start screen, and startGame,
which starts the game by creating the game board and updating the frames of the snake’s movement on the
screen.
The Corner class is a simple class that represents a single cell of the game board. It has two integer
instance variables, x, and y, that represent the cell’s position on the board. The class has a constructor that
takes two integer parameters and initializes the instance variables.
The Speedup class is a class that can be used to increase the speed of the snake as the player’s score
increases. The class has an integer instance variable scoreThreshold that stores the score at which the speed
will be increased. The class has a constructor that takes an integer parameter and assigns it to the instance
variable. The class also has a method increaseSpeed that takes an integer parameter score and increases the
speed of the snake based on the score. If the score is equal to 3, the speed is set to 7. If the score is equal
to 6, the speed is set to 10. If the score is equal to 8, the speed is set to 14. If the score does not match any
of these values, the method does nothing. The class is used in the SnakeGame class to create an instance of
the class with a score threshold of 3.

# execution
![lose](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/ed634157-c19d-47e4-b59d-d1d4e3b5b286)
![win](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/de65181e-3908-4948-a9d6-84fc2b2c3437)

