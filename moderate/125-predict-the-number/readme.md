<h2>Predict the Number</h2>

<h3>Challenge Description:</h3>
<p>
    The sequence &quot;011212201220200112 ...&quot; is constructed as follows:<br>
    first goes 0, and then the following action is repeated: existing part is added to the right, but 0 is replaced
    with 1, 1 with 2, and 2 with 0.
</p>

<pre>0 -&gt; 01 -&gt; 0112 -&gt; 01121220 -&gt; ...</pre>

<p>Write an algorithm that determines what number is on the N-th position in the sequence.</p>

<h3>Input sample:</h3>

<p>
    Your program should accept a path to a filename as its first argument. Each line in the file contains a number N.
</p>

<p>For example:</p>

<pre class="description-input-output">0
5
101
25684</pre>

<h3>Output sample:</h3>

<p>Print out a number that is on the N-th position in the sequence.</p>

<pre class="description-input-output">0
2
1
0</pre>

<h3>Constraints:</h3>

<ol>
<li>0 &lt;= N &lt;= 3000000000.</li>
</ol>