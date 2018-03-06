<h2>Sudoku</h2>

<h3>Challenge Description:</h3>

<p>
    Sudoku is a number-based logic puzzle. It typically comprises of a 9*9 grid
    with digits so that each column, each row and each of the nine 3*3
    sub-grids that compose the grid contains all the digits from 1 to 9. For this challenge, you will be given an N*N grid populated with numbers from 1 through N and you have to determine if it is a valid sudoku solution. You may assume that N will be either 4 or 9. The grid can be divided into square regions of equal size, where the size of a region is equal to the square root of a side of the entire grid. Thus for a 9*9 grid there would be 9 regions of size 3*3 each.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains the value of N, a semicolon and the sqaure
    matrix of integers in row major form, comma delimited. E.g.
</p>
<pre>4;1,4,2,3,2,3,1,4,4,2,3,1,3,1,4,2
4;2,1,3,2,3,2,1,4,1,4,2,3,2,3,4,1</pre>

<h3>Output sample:</h3>

<p>
    Print out True/False if the grid is a valid sudoku layout. E.g.
</p>

<pre>True
False</pre>