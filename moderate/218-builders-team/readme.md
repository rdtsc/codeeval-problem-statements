<h2>Builders team.</h2>

<h3>Challenge Description:</h3>

<p>
    A team of builders have a task to lay pipes in a new city district: they lay out cables, electricity, phone, and
    other pipes. They lay each pipe according to the given route &#x2014; starting from house 1 to house 25 as shown on a map
    (see Picture #1). Houses with all laid communication pipes are those where all pipes form a square. <br>
    Let&#x2019;s consider a map on Picture #2. It shows that the water will be in houses 1, 2, 3, 6, 7, 8, 11, 12, and 13.
    While in house 4 and all the other houses, there will be no water.<br>
    Your task is to count the number of squares of laid pipes between houses on a map. The answer to picture #2 will
    be 2 squares. If there were pipes between houses 7 and 8, then the number of squares would be 3. If there were
    pipes between houses (7 and 8) and (7 and 12), then the number would be 5 squares.
<br>
</p>

<p>
    <img src="assets/fig-1.png" alt="Figure 1">
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case, which contains the coordinates by which
    pipes should be laid. Coordinates are separated by a pipeline &apos;|&apos;.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">1 2 | 6 7 | 7 2 | 1 6 | 2 3
1 2 | 6 7 | 7 2 | 1 6 | 2 3 | 7 8 | 3 8
1 2 | 1 6 | 6 7</pre>

<h3>Output sample:</h3>

<p>
    You need to count all squares of laid pipes on a district map.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">1
2
0</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of coordinates in one test case can be from 4 to 60.</li>
<li>The number of test cases is 40.</li>
</ol>
