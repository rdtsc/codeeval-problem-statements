<h2>A Pile of Bricks</h2>

<h3>Challenge Description:</h3>

<p>
    You have a pile of bricks.
    Every brick has it&apos;s index number and coordinates of opposite vertices.
<br>
    You know that somewhere on the wall there is a rectangular hole,
    and you are given coordinates of opposite vertices of that hole.
<br>
    Determine which bricks may pass through that hole.
<br>
    In situations where brick and hole have an equal sizes, we assume that it can pass through this hole.
<br>
    All the holes are two-dimensional.
    All of the bricks are three-dimensional.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    The input file contains several lines. Each line is one test case.
<br>
<br>
    Each line contains coordinates of opposite vertices of a hole (before the vertical bar)
    separated by space bar and the list of bricks you need to check.
    Each brick is enclosed in parentheses where the 1st number is a brick&apos;s index number,
    the 2nd and 3rd group of numbers are brick&apos;s coordinates of opposite vertices (separated by a space bar),
    each brick is divided by semicolon. E.g.
</p>
<pre class="description-input-output">[4,3] [3,-3]|(1 [10,9,4] [9,4,2])
[-1,-5] [5,-2]|(1 [4,7,8] [2,9,0]);(2 [0,7,1] [5,9,8])
[-4,-5] [-5,-3]|(1 [4,8,6] [0,9,2]);(2 [8,-1,3] [0,5,4])</pre>

<h3>Output sample:</h3>

<p>
    For each set of bricks produce a list of bricks (their index numbers in ascending order
    separated by comma) that can pass through the hole. E.g.
</p>

<pre class="description-input-output">1
1,2
-</pre>

<p>
<b>Constraints:</b>
<br>
    Coordinates are in range [-100, 100]
<br>
    There might be up to 15 bricks you need to check.
</p>