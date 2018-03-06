<h2>Lakes, not cakes</h2>

<h3>Challenge Description:</h3>

<p>
    It was a dark and stormy night when Alice was wandering in the black forest. The rain fell in torrents into deep
    lakes scattered all over the area&#x2026; Wait! Lakes&#x2026; forest&#x2026;? Really? Well, yeah, it&#x2019;s not a true horror story, but it
    is fits our challenge perfectly. So, you have a map of the forest. You are sure there are some lakes in there,
    but you do not know their number.
<br>
    Write a program that will count how many lakes are in the forest. We count all adjacent <b>o</b> symbols as one lake
    (by adjacent we mean symbols that are located one cell up, down, left, right, or diagonally from the needed symbol).
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case, which contains a map of the forest of
    different size. Forest areas are separated by a vertical bar <b>|</b>. <br>
<b>#</b> - forest <br>
<b>o</b> - lake
</p>

<p>
    For example:
</p>

<pre class="description-input-output">o # o | # # # | o # o
o # o | # o # | o # o</pre>

<h3>Output sample:</h3>

<p>
    Print the number of lakes for each test case.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">4
1</pre>

<h3>Constraints:</h3>
<ol>
<li>A forest may be of different width and height from 3 to 30 symbols.</li>
<li>Diagonal symbols are also counted as adjacent.</li>
<li>The number of test cases is 40.</li>
</ol>