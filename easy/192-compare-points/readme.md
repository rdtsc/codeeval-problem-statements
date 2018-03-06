<h2>Compare Points</h2>

<h3>Challenge Description:</h3>

<p>
    Bob&apos;s hiking club is lost in the mountains on the way to a scenic overlook. Fortunately, Bob has a GPS device,
    so that he can see the coordinates where the group is currently at. The GPS gives the current X/Y coordinates
    as O, P, and the scenic overlook is located at Q, R. Bob now just needs to tell the group which way to go
    so they can get to the overlook in time for s&apos;mores.
</p>

<h3>Input sample:</h3>

<p>
    The input is a file with each line representing a test case. Each test case consists of four integers O, P, Q, R
    on a line, separated by spaces.
</p>

<pre class="description-input-output">0 0 1 5
12 13 12 13
0 1 0 5</pre>

<h3>Output sample:</h3>

<p>
    For each test case print a line containing one of the following:
<code>N, NE, E, SE, S, SW, W, NW, here</code> if the coordinates Q, R are (respectively) north, northeast, east,
    southeast, south, southwest, west, northwest, or already at (&quot;here&quot;) the coordinates O, P. Note that N, S, E and W
    mean <i>directly</i> North, South, East or West respectively, i.e. X or Y coordinates of two points are exactly
    the same. In all other cases your output should be one of the NW, NE, SW, SE or here.
</p>

<pre class="description-input-output">NE
here
N</pre>

<h3>Constraints:</h3>
<ol>
<li>All coordinates -10000 &lt; |O,P,Q,R| &lt; 10000</li>
<li>Number of test cases is 40</li>
</ol>