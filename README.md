# Non-plussed
Non-plussed solves all your nonogram puzzles for you, letting you see what you should have ended up with had you solved it yourself.

## Usage
Each nonogram puzzle is described by a grid, with each row and column defined by a sequence of numbers. This solver takes two arrays of arrays (```[][]uint64```), one each for rows and columns, where each element of the array defines the nest row or column.

For example, the arrays ```[[2,1],[]]```, ```[[1],[1],[],[1]]``` define the grid:
X X . X
. . . .

To solve your puzzle you can run ```nono rows columns [-f format]``` where ```rows``` and ```columns``` are the previously mentioned ```[][]uint64``` values describing the puzzle and the optional flag ```-f``` defines the desired output for the solution.

The output depends on the value passed to the optional output flag ```-f``` but will either be a ```.png```, ```.csv```  or terminal (default) output, with the value passed to f being equal to the desired filetype.

If the solver is unable to solve the puzzle passed to it, please raise it as an issue along with the solution. If a solution is not provided I will ignore the issue as I will have nothing to verify it as a valid problem.
