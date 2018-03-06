<h2>Sequence Transformation</h2>

<h3>Challenge Description:</h3>
<p>
    There are two sequences. The first sequence consists of digits &quot;0&quot; and &quot;1&quot;, the second one consists of letters &quot;A&quot; and &quot;B&quot;.
    The challenge is to determine whether it&apos;s possible to transform a given binary sequence into a string sequence using the following rules:
<br>
    1. &quot;0&quot; can be transformed into non empty sequence of letters &quot;A&quot; (&quot;A&quot;, &quot;AA&quot;, &quot;AAA&quot; etc.)
<br>
    2. &quot;1&quot; can be transformed into non empty sequence of letters &quot;A&quot; (&quot;A&quot;, &quot;AA&quot;, &quot;AAA&quot; etc.) or to non empty sequence of letters &quot;B&quot; (&quot;B&quot;, &quot;BB&quot;, &quot;BBB&quot; etc) e.g.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line in this file contains a binary
    sequence and a sequence of letters &quot;A&quot; and &quot;B&quot; separated by a single whitespace. E.g.
</p>

<pre class="description-input-output">1010 AAAAABBBBAAAA
00 AAAAAA
01001110 AAAABAAABBBBBBAAAAAAA
1100110 BBAABABBA</pre>

<h3>Output sample:</h3>

<p>
    For each test case print out &quot;Yes&quot; if the transformation is possible, otherwise print &quot;No&quot;. E.g.
</p>

<pre class="description-input-output">Yes
Yes
Yes
No</pre>
<p>
    Constraints:
<br>
    The length of a binary sequence is in range [1, 150]
<br>
    The length of a string sequence is in range [1, 1000]
<br>
    The number of test cases is &lt;= 50
</p>