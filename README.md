# Sudoku
Inprocess sudoku player/solver

This is my first independent project. It is built with python 3 in tkinter

As of now, majority of work was completed without git or github. As of now, I have a gui which will:

- display the board, 
- allow the selection of individual squares/cells by either clicking them or with arrow keys if a cell as already been 
selected
- add a number to a cell if it does not lead to a contradiction(by calling methods of the board class)
- remove number from a cell (by calling methods of the board class)
- Solve by use of a button (by calling methods of the board class)

I also have a class to represent the board. It stores information in as series of nested lists. It can:
- return the value of a cell by row and column
- return the contents of a particular row or column
- add or remove contents from a cell
- check for contradictions
- Solve the board by backtracking (note: This has worked on examples, but has not yet been thoroughly tested)

How to use:

-Download all three files and run the integration file. 

Room for improvement -

- Creation of a valid unique puzzle to make it a working player
      - A way to specify contents which cannot be changed (values provided at onset of the puzzle).
          - Give these values a different color
      - A way to specify difficult and select the provided cells
      
- Improving the solver
      - Needs better testing, which requires the implementation of a rigorous testing method
      - Code was on the fly and could stand to be streamlined for space and readability
      - The backtracking approach is slow and crude. Upon finishing, I read this article (norvig.com/sudoku.html)
      to see what I could have done differently and I may implement some of these methods later on to optimize
      
 Self critiques and lessons learned- 
 
 This was my first project without being a part of a course outline. As a result, there was less of a path 
 to follow. I wanted this to be purely a test of my problem solving skills and so the only thing I looked up 
 was the wikipedia of sudoku solvers (https://en.wikipedia.org/wiki/Sudoku_solving_algorithms). As a result, 
 I went at this head first, figuring out each problem as it arose. As a result, certain aspects are clunky and, 
 reading the norvig article. I see there are a lot of more efficient ways I could implemented things (my nested 
 series of lists is overly complicated and much of my work from that point was figuring out how to manipulate that list)
 
 Had I started with a clear outline, I could have prevented problems rather than solving them and wound up with cleaner 
 code and more time conserved.
