<h2>Shortest Repetition</h2>

<h3>Challenge Description:</h3>

<p>
    Write a program to determine the shortest repetition in a string.
<br>
    A string is said to have period <b>p</b> if it can be formed
    by concatenating one or more repetitions of another string of length
<b>p</b>. For example, the string &quot;xyzxyzxyzxyz&quot; has period 3, since it is
    formed by 4 repetitions of the string &quot;xyz&quot;. It also has periods 6
    (two repetitions of &quot;xyzxyz&quot;) and 12 (one repetition of &quot;xyzxyzxyzxyz&quot;).
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line will contain a string of up to 80 non-blank characters. E.g.
</p>
<pre>abcabcabcabc
bcbcbcbcbcbcbcbcbcbcbcbcbcbc
dddddddddddddddddddd
adcdefg</pre>

<h3>Output sample:</h3>

<p>
    Print out the smallest period of the input string. E.g.
</p>

<pre>3
2
1
7</pre>