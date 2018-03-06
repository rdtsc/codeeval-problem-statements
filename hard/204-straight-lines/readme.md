<h2>Straight lines</h2>

<h3>Challenge Description:</h3>

<p>
    It&#x2019;s high time you remembered geometry lessons at school: graphs, coordinates, shapes, and others.<br>
    You have the coordinates of the points. The point location is determined by X and Y coordinate system.
    Your task is to count how many straight lines that will cross three or more points you can create.<br>
    For example, in the figure #1, the number of such lines is one, while in the figures #2 and #3,
    we can create two lines.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with point coordinates that are
    separated by the pipe symbol &apos;|&apos;. Point coordinates might be negative; they are in a range from -20 to 20.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">1 1 | 1 2 | 1 4 | 3 2
1 1 | 1 2 | 1 4 | 3 2 | 4 2
1 2 | 1 4 | 2 3 | 3 2 | 3 4</pre>

<h3>Output sample:</h3>

<p>
    Print the number of lines that cross three or more points in a straight line.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">1
2
2</pre>

<h3>Constraints:</h3>
<ol>
<li>
        A straight line is a line that contains three or more coordinate points.
        That is, if you add a point with coordinates [2, 2] to the figure #2, there will be two straight lines anyway.
</li>
<li>Point coordinates can be in a range from -20 to 20.</li>
<li>The number of test cases is 40.</li>
</ol>