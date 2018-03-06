<h2>Split The Number</h2>

<h3>Challenge Description:</h3>
<p>
    You are given a number N and a pattern. The pattern consists of lowercase latin letters and one operation &quot;+&quot; or &quot;-&quot;.
    The challenge is to split the number and evaluate it according to this pattern e.g.
<br>
    1232 ab+cd -&gt; a:1, b:2, c:3, d:2 -&gt; 12+32 -&gt; 44
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line of the file is a test case, containing
    the number and the pattern separated by a single whitespace. E.g.
</p>

<pre class="description-input-output">3413289830 a-bcdefghij
776 a+bc
12345 a+bcde
1232 ab+cd
90602 a+bcde</pre>

<h3>Output sample:</h3>

<p>
    For each test case print out the result of pattern evaluation. E.g.
</p>

<pre class="description-input-output">-413289827
83
2346
44
611</pre>
<p>
    Constraints:
<br>
    N is in range [100, 1000000000]
</p>