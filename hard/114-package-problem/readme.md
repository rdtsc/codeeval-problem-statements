<h2>Package Problem</h2>

<h3>Challenge Description:</h3>

<p>
    You want to send your friend a package with different things.
<span class="p-like">
    Each thing you put inside the package has such parameters as index number, weight and cost.
</span>
<span class="p-like">
    The package has a weight limit.
</span>
    Your goal is to determine which things to put into the package so that the total weight is less than or equal
    to the package limit and the total cost is as large as possible.
</p>
<p>
    You would prefer to send a package which  weights less in case there is more than one package with the same price.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. The input file contains several lines.
    Each line is one test case.
</p>
<p>
    Each line contains the weight that the package can take (before the colon) and the list of things you need
    to choose. Each thing is enclosed in parentheses where the 1<sup>st</sup> number is a thing&apos;s index number,
    the 2<sup>nd</sup> is its weight and the 3<sup>rd</sup> is its cost. E.g.
</p>

<pre class="description-input-output">81 : (1,53.38,$45) (2,88.62,$98) (3,78.48,$3) (4,72.30,$76) (5,30.18,$9) (6,46.34,$48)
8 : (1,15.3,$34)
75 : (1,85.31,$29) (2,14.55,$74) (3,3.98,$16) (4,26.24,$55) (5,63.69,$52) (6,76.25,$75) (7,60.02,$74) (8,93.18,$35) (9,89.95,$78)
56 : (1,90.72,$13) (2,33.80,$40) (3,43.15,$10) (4,37.97,$16) (5,46.81,$36) (6,48.77,$79) (7,81.80,$45) (8,19.36,$79) (9,6.76,$64)</pre>

<h3>Output sample:</h3>

<p>
    For each set of things that you put into the package provide a list (items&#x2019; index numbers are separated by comma).
    E.g.
</p>

<pre class="description-input-output">4
-
2,7
8,9</pre>

<h3>Constraints:</h3>
<ol>
<li>Max weight that a package can take is &#x2264; 100</li>
<li>There might be up to 15 items you need to choose from</li>
<li>Max weight and cost of an item is &#x2264; 100</li>
</ol>