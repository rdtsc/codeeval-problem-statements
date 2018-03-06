<h2>Game of Life</h2>

<h3>Challenge Description:</h3>

<p>
    The challenge is based on John&#x2019;s Conway &#x2018;Game of Life&#x2019;. The Game of Life is a cellular automaton developed by
    the British mathematician John Conway in 1970. The universe of the game is an infinite two-dimensional orthogonal
    grid of square cells, each of which is in one of two possible states, alive or dead. Every cell that is
    horizontally, vertically, or diagonally adjacent interacts with its eight neighbors. At each step in time, the
    following iterations occur:
</p>
<ul>
<li>Any live cell with fewer than two live neighbors dies, as if caused by under-population.</li>
<li>Any live cell with two or three live neighbors lives on to the next generation.</li>
<li>Any live cell with more than three live neighbors dies, as if by overcrowding.</li>
<li>Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.</li>
</ul>
<p>
    The initial pattern constitutes the seed of the system. The first generation is created by applying the above
    rules simultaneously to every cell in the seed &#x2014; births and deaths occur simultaneously. The rules continue to be
    applied repeatedly to create further generations.
</p>

<p>
    You have a grid of size N&#xD7;N, seeded with some live cells. Your task is to determine the state of the grid after
    10 iterations.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file with the initial state of the grid. Alive cells are shown as asterisks &#x2018;*&#x2019;, and dead
    cells are shown as points &#x2018;.&#x2019;. E.g.
</p>

<pre>.........*
.*.*...*..
..........
..*.*....*
.*..*...*.
.........*
..........
.....*..*.
.*....*...
.....**...</pre>

<h3>Output sample:</h3>

<p>Print to stdout the state of the grid after 10 iterations. E.g.</p>

<pre>..........
...*......
..*.*.....
..*.*.....
...*......
..........
..........
..........
..........
..........</pre>

<h3>Constraints:</h3>
<ol>
<li>The size of the grid in real input is 100&#xD7;100 cells.</li>
<li>The cells outside the grid borders are assumed to be dead.</li>
</ol>