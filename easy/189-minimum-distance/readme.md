<h2>Minimum Distance</h2>

<h3>Challenge Description:</h3>

<p>
    Alice is looking for a sorority to join for her first year at Acme
    University. There is a street consisting entirely of sorority houses
    near the university, and some of her high school friends have already
    joined sorority houses on the street. (More than one of her friends
    may live at the same sorority house.)
</p>

<p>
    Alice wants to visit her friends frequently, and needs a program that
    will help her pick an optimal house to visit them from. Each sorority
    house has a street number that indicates its location on the
    street. The optimal location will minimize the sum of differences
    between the number of Alice&apos;s house and the number of her friends&apos;
    houses.
</p>

<p>For example: Alice&apos;s friends live at houses 3, 3, 5, and 7.  Alice moves
in at house 4. Then the distances to her friends&apos; houses are 1, 1, 1,
and 3, totaling 6.</p>

<h3>Input sample:</h3>

<p>The input consists of several integers on a line, separated by
spaces. The first integer F contains the number of friends (0 &lt; F &lt;
100). Then F street addresses A follow (0 &lt; A &lt; 10000).</p>

<p>For example:</p>

<pre class="description-input-output">4 3 3 5 7
3 20 30 40</pre>

<h3>Output sample:</h3>

<p>Print a line containing the minimal sum of distances for an optimal
sorority location.</p>

<p>For example:</p>

<pre class="description-input-output">6
20</pre>

<h3>Constraints:</h3>

<ol>
<li>Number of friends: 0 &lt; F &lt; 100</li>
<li>Street addresses: 0 &lt; A &lt; 10000</li>
<li>Number of test cases is 10.</li>
</ol>