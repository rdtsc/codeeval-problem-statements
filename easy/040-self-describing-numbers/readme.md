<h2>Self Describing Numbers</h2>

<h3>Challenge Description:</h3>

<p>
    A number is a self-describing number when (assuming digit positions
    are labeled 0 to N-1), the digit in each position is equal to the
    number of times that that digit appears in the number.
</p>

<h3>Input sample:</h3>
<p>
    The first argument is the pathname to a file which contains test data,
    one test case per line. Each line contains a positive integer.
    E.g.
</p>
<pre>2020
22
1210</pre>

<h3>Output sample:</h3>

<p>
    If the number is a self-describing number, print out 1. If not, print
    out 0. E.g.
</p>

<pre>1
0
1</pre>

<p>
    For the curious, here&apos;s how 2020 is a self-describing number:
    Position &apos;0&apos; has value 2 and there is two 0 in the number.
    Position &apos;1&apos; has value 0 because there are not 1&apos;s in the number.
    Position &apos;2&apos; has value 2 and there is two 2.
    And the position &apos;3&apos; has value 0 and there are zero 3&apos;s.
</p>