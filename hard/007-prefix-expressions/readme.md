<h2>Prefix expressions</h2>

<h3>Challenge Description:</h3>
<p>
    You are given a prefix expression. Write a program which evaluates it.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a file as its first argument. The file contains one prefix expression per line.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">* + 2 3 4</pre>
<p>
    Your program should read this file and insert it into any data structure you like. Traverse this data structure
    and evaluate the prefix expression. Each token is delimited by a whitespace. You may assume that sum &#x2018;+&#x2019;,
    multiplication &#x2018;*&#x2019; and division   &#x2018;/&#x2019; are the only valid operators appearing in the test data.
</p>

<h3>Output sample:</h3>
<p>
    Print to stdout the output of the prefix expression, one per line.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">20</pre>

<h3>Constraints:</h3>
<ul>
<li>The evaluation result will always be an integer &#x2265; 0.</li>
<li>The number of the test cases is &#x2264; 40.</li>
</ul>