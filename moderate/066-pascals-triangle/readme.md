<h2>Pascals Triangle</h2>

<h3>Challenge Description:</h3>

<p>
    A Pascals triangle row is constructed by looking at the previous row and
    adding the numbers to its left and right to arrive at the new value.
    If either the number to its left/right is not present, substitute a zero
    in it&apos;s place. More details can be found here:
<a href="http://en.wikipedia.org/wiki/Pascal&apos;s_triangle">Pascal&apos;s triangle</a>. E.g.
    a Pascal&apos;s triangle upto a depth of 6 can be shown as:
</p>
<pre>            1
          1   1
        1   2   1
       1  3   3   1
     1  4   6   4   1
    1  5  10  10  5   1
</pre>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains a positive integer which indicates the
    depth of the triangle (1 based). E.g.
</p>
<pre>6</pre>

<h3>Output sample:</h3>

<p>
    Print out the resulting pascal triangle upto the requested depth in
    row major form. E.g.
</p>
<pre>1 1 1 1 2 1 1 3 3 1 1 4 6 4 1 1 5 10 10 5 1</pre>