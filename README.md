## Optimize Histogram Filter
Optimizing 2D histrogram filter code in C++

### Project Files
instructions.md

This file contains further instructions about how to complete and run the project.

hints.md

The optimized_code files already have ideas about what to optimize. The hints file contains more explicit ideas but does not give the actual code. You are not required to read this file, and we encourage you to try optimizing the code first before reading the hints file.

### Explanation of the Code
In `main.cpp`, you'll find a vector called grid. Grid is a char vector holding the color values of a 2-dimensional square grid.

The `initialize_beliefs` function takes in the char grid and outputs the initial probabilities for each square on the grid.

Then the `sense` function takes a measurement of the current grid space's color. The measurement is used to update the probabilities of each space on the grid.

Next, the `blur` function passes the grid through a smoothing algorithm.

Then the probabilities are normalized with the `normalize` function.

Finally, the robot moves to a new space on the board, and the probabilities are updated appropriately.

Each function is run ten-thousand times. You can adjust the number of times by changing the value in the iterations variable.

### Order
As a suggestion, do the project in the following order:

  1. Read through the instructions in instructions.md
  2. Run the code in the andy_histogram_filter folder (see instructions.md for how to run the code)
  3. Open main.cpp and look through the code. You do not need to change anything in this file. Note that each function is run the same number of times. And each function is wrapped with a clock.
  4. Read through each of the .cpp files to become familiar with the code.
  5. Optimize the code in the optimized_code folder. For each optimization, make sure to run the code to see if the results have in fact improved.
  
Here is a suggested order for optimizing the files:

  - zeros.cpp
  - initialize_beliefs.cpp
  - sense.cpp
  - blur.cpp
  - normalize.cpp
  - move.cpp
