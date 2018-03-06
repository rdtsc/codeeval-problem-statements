<h2>Grinch</h2>

<h3>Challenge Description:</h3>

<p>
    Every year, Grinch wants to destroy New Year holidays in any possible way. This year is not an exception. Somehow
    he found out Santa&#x2019;s route and wants to steal the gifts from him. To make it possible, he needs to know the time
    during which he can get from one point of the route to another. Let&#x2019;s help him calculate the route. Anyway,
    he won&#x2019;t&#x2019; make it. :)
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case, containing a map with routes. Routes are
    separated by comma. Each route contains three numbers: the first two numbers are the start and end points of the
    route, and the third one &#x2013; the length between these two points. Also, there are to numbers in a test case (A and B)
    that show where Grinch should start and where he should get to. The map and points A and B are separated by a
    pipeline `|`.
</p>

<pre class="description-input-output">1 2 2, 1 3 3, 3 4 3, 2 4 6, 4 5 16, 3 5 7 | 1 5
1 2 3, 2 8 10, 1 9 4, 8 9 2 | 2 8</pre>

<h3>Output sample:</h3>

<p>
    Print the length of the shortest route from point A to point B. If you cannot get from A to B that means that an
    avalanche has blocked the way. In this case, print False.
</p>

<pre class="description-input-output">10
9</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of routes in the map can be from 4 to 20.</li>
<li>If you cannot get from point A to B, print False.</li>
<li>The number of test cases is 15.</li>
<li>Happy New Year 2016!</li>
</ol>