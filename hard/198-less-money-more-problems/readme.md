<h2>Less Money, More Problems</h2>

<h3>Challenge Description:</h3>

<p>
<small>This challenge appeared in Google Code Jam competition, licensed under
<a href="http://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution License</a></small>
</p>

<p>
    Up until today, the nation you live in has used <strong>D</strong> different positive integer denominations of coin for
    all transactions. Today, the queen got angry when a subject tried to pay his taxes with a giant sack of low-valued coins,
    and she just decreed that no more than <strong>C</strong> coins of any one denomination may be used in any one purchase.
    For instance, if C = 2 and the existing denominations are 1 and 5, it is possible to buy something of value 11 by using
    two 5s and one 1, or something of value 12 by using two 5s and two 1s, but it is impossible to buy something of
    value 9 or 17.
</p>
<p>
    You cannot directly challenge the queen&apos;s decree, but you happen to be in charge of the mint, and you can issue new
    denominations of coin. You want to make it possible for any item of positive value at most <strong>V</strong> to be
    purchased under the queen&apos;s new rules. (Note that this may not necessarily have been possible before the queen&apos;s
    decree.) Moreover, you want to introduce as few new denominations as possible, and your final combined set of
    pre-existing and new denominations may not have any repeats.
</p>
<p>
    What is the smallest number of new denominations required?
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line of the input file contains one test case. Each test case consists
    of three parts separated by pipe symbol: 1) an integer <strong>C</strong>; 2) an integer <strong>V</strong>;
    3) sorted list of space separated integers - all current denominations.
</p>

<pre class="description-input-output">1 | 3 | 1 2
1 | 6 | 1 2 5
2 | 3 | 3
1 | 100 | 1 5 10 25 50 100</pre>

<h3>Output sample:</h3>

<p>
    For each test case, output one line containing the minimum number of new denominations required, as described above.
</p>

<pre class="description-input-output">0
1
1
3</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of test cases is 40.</li>
<li>1 &#x2264; C &#x2264; 100.</li>
<li>1 &#x2264; V &#x2264; 10<sup>9</sup>.</li>
<li>The number of current denominations is in range from 1 to 100.</li>
</ol>