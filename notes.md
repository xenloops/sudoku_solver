## TODOs

* ```ImportPuzzle()``` imports incomplete puzzle from text file
* ```ExportPuzzle()``` writes to text file
* Check functions check for an existing value _n_ like so:
  * ```CheckRow(n, y)``` returns True if _n_ exists in Row _y_
  * ```CheckCol(n, x)``` returns True if _n_ exists in Column _x_
  * ```CheckSquare(n, x, y)``` returns True if _n_ exists in the square centered at (_x_, _y_)
* ```MakePuzzle(n)``` creates a random sudoku with _n_ randomly-placed blanks. (Maybe I'll add symmetry to the blanks at some point, but even then these won't be as good as hand-crafted sudoku!)

## Conventions

* The code implements a sudoku internally as a List of Lists. The coordinate system starts at the bottom left of the sudoku tableau. This is due to my background interest in mathematics; applying the cartesian coordinate system, all coordinates in sudoku should be positive.
* The text format for importing a puzzle is a simple 2-dimensional array with blanks represented by perids or dashes, e.g.:
  ```
  -5-----7-
  ---4-7---
  2-6---1-4
  -9--8--5-
  5-------2
  -2--3--1-
  9-2---7-6
  ---6-1---
  -8-----3-
  ```

