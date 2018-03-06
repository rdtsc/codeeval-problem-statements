<h2>Grid Walk</h2>

<h3>Challenge Description:</h3>

<p>
    There is a monkey which can walk around on a planar grid.
    The monkey can move one space at a time left, right, up or down.
    That is, from (x, y) the monkey can go to (x+1, y), (x-1, y), (x, y+1), and (x, y-1).
</p>
<p>
    Points where the sum of the digits of the absolute value of the x coordinate plus
    the sum of the digits of the absolute value of the y coordinate are lesser than or equal
    to 19 are accessible to the monkey. For example, the point (59, 79) is inaccessible because
    5 + 9 + 7 + 9 = 30, which is greater than 19. Another example: the point (-5, -7) is
    accessible because abs(-5) + abs(-7) = 5 + 7 = 12, which is less than 19.
    How many points can the monkey access if it starts at (0, 0), including (0, 0) itself?
</p>

<h3>Input sample:</h3>
<p>There is no input for this program.</p>

<h3>Output sample:</h3>
<p>Print the number of points the monkey can access. It should be printed as an integer &#x2014; for example, if the number of points is 10, print &quot;10&quot;, not &quot;10.0&quot; or &quot;10.00&quot;, etc.</p>