<h2>Happy Numbers</h2>

<h3>Challenge Description:</h3>

<p>
    A happy number is defined by the following process. Starting with any
    positive integer, replace the number by the sum of the squares of its
    digits, and repeat the process until the number equals 1 (where it
    will stay), or it loops endlessly in a cycle which does not include 1.
    Those numbers for which this process ends in 1 are happy numbers, while
    those that do not end in 1 are unhappy numbers.
</p>

<h3>Input sample:</h3>
<p>
    The first argument is the pathname to a file which contains test data,
    one test case per line. Each line contains a positive integer. E.g.
</p>

<pre>1
7
22</pre>

<h3>Output sample:</h3>

<p>
    If the number is a happy number, print out 1. If not, print out 0. E.g
</p>

<pre>1
1
0</pre>

<p>
    For the curious, here&apos;s why 7 is a happy number: 7-&gt;49-&gt;97-&gt;130-&gt;10-&gt;1.
    Here&apos;s why 22 is NOT a happy number:
    22-&gt;8-&gt;64-&gt;52-&gt;29-&gt;85-&gt;89-&gt;145-&gt;42-&gt;20-&gt;4-&gt;16-&gt;37-&gt;58-&gt;89 ...
</p>