<h2>Strings and arrows</h2>

<h3>Challenge Description:</h3>

<p>
    You have a string composed of the following symbols: &apos;&gt;&apos;, &apos;&lt;&apos;, and &apos;-&apos;. Your task is to find, count,
    and print to the output a number of arrows in the string. An arrow is a set of the following symbols: &apos;&gt;&gt;--&gt;&apos; or &apos;&lt;--&lt;&lt;&apos;. <br>
    Note that one character may belong to two arrows at the same time. Such example is shown in the line #1.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with a string of
    different length from 10 to 250 characters. The string consists of &apos;&gt;&apos;, &apos;&lt;&apos;, and &apos;-&apos; symbols.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">&lt;--&lt;&lt;--&lt;&lt;
&lt;&lt;&gt;&gt;--&gt;&lt;--&lt;&lt;--&lt;&lt;&gt;&gt;&gt;--&gt;&lt;
&lt;--&gt;&gt;</pre>

<h3>Output sample:</h3>

<p>
    Print the total number of found arrows for each test case.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">2
4
0</pre>

<h3>Constraints:</h3>
<ol>
<li>An arrow is a set of the following symbols: &apos;&gt;&gt;--&gt;&apos; or &apos;&lt;--&lt;&lt;&apos;.</li>
<li>One symbol may belong to two arrows at the same time.</li>
<li>The number of test cases is 40.</li>
</ol>