<h2>Juggling With Zeros</h2>

<h3>Challenge Description:</h3>
<p>
    In this challenge, you will deal with zero-based numbers.  A zero-based number has the following form: &quot;flag&quot;
    &quot;sequence of zeroes&quot; &quot;flag&quot; &quot;sequence of zeroes&quot;, and so on. The numbers are separated by a single space.
</p>
<pre>00 0 0 00 00 0</pre>
<p>
    You have to convert zero-based numbers into integers. To do this,  you need to perform the following steps:
</p><ol>
<li>Convert a zero-based number into a binary form using the following rules:
<p>a) flag &quot;0&quot; means that the following sequence of zeroes should be appended to a binary string.</p>
<p>b) flag &quot;00&quot; means that the following sequence of zeroes should be transformed into a sequence of ones
            and be appended to a binary string.</p>
<pre>00 0 0 00 00 0 --&gt; 1001</pre>
</li>

<li>Convert the obtained binary string into an integer.
<pre>1001 --&gt; 9</pre>
</li>
</ol>

<h3>Input sample:</h3>
<p>
    The first argument is a file where each line of input contains a string with zero-based number.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">00 0 0 00 00 0
00 0
00 0 0 000 00 0000000 0 000
0 000000000 00 00</pre>

<h3>Output sample:</h3>
<p>
    For each line of input, print an integer converted from a zero-based number.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">9
1
9208
3</pre>