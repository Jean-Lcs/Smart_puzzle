# Smart_puzzle

![Cover](https://github.com/Jean-Lcs/Smart_puzzle/blob/main/steps_smart_puzzle.png)



This personal project has the same purpose than the older one 'Non_optimized_maze_soler" but is actually quite different in its structure and method.
Therefore we aim to solve a puzzle, following these steps:
  - Take any initial image
  - Cut it into a certain number of pieces (this number being modifiable)
  - Shuffle it randomly, except for the top left piece which stays where it is

Then, we try to find the correct position for each sub-image but in a smarter way:
  - STEP 1: First, we start with the top left piece (which still is at the first position) and we try to look for the bottom neighboor by minimzing the "TOP-BOTTOM" discontinuity. We reitate in order to have the entire first column.
  - STEP 2: Still from the top left piece, we look for the bottom neighboor by minimzing the "LEFT-RIGHT" discontinuity. We reitate to have the entire first line
  - STEP 3: For each line, we strat by the left element (that we already have since it's the first column) and we try to look for the right neighboor by minimizing the "TOP-BOTTOM" AND "LEFT-RIGHT" discontinuities, which insures some better results and allows use to raise the number of puzzle pieces.

Finally, we have all the positions so we reassemble the image


![alt tag](https://github.com/Jean-Lcs/Smart_puzzle/blob/main/RM_pic.jpg)
