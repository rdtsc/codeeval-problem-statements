<h2>Closest Pair</h2>

<h3>Challenge Description:</h3>
<p>
    Credits: Programming Challenges by Steven S. Skiena and Miguel A. Revilla
<br>
<br>
    You will be given the x/y co-ordinates of several locations.
    You will be laying out 1 cable between two of these locations.
    In order to minimise the cost, your task is to find the shortest distance between a pair of locations,
    so that pair can be chosen for the cable installation.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    The input file contains several sets of input. Each set of input starts with an integer N (0&lt;=N&lt;=10000),
    which denotes the number of points in this set.
    The next N line contains the coordinates of N two-dimensional points.
    The first of the two numbers denotes the X-coordinate and the latter denotes the Y-coordinate.
    The input is terminated by a set whose N=0. This set should not be processed.
    The value of the coordinates will be less than 40000 and non-negative. eg.
</p>
<pre class="description-input-output">5
0 2
6 67
43 71
39 107
189 140
0</pre>

<h3>Output sample:</h3>

<p>
    For each set of input produce a single line of output containing a floating point number
    (with four digits after the decimal point) which denotes the distance between the closest two points.
    If there is no such two points in the input whose distance is less than 10000, print the line INFINITY. eg.

</p><pre class="description-input-output">36.2215</pre>