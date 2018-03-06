<h2>Double Squares</h2>

<h3>Challenge Description:</h3>

<span>
    Credits: This challenge appeared in the Facebook Hacker Cup 2011.
</span>

<p>
    A double-square number is an integer X which can be expressed as the sum
    of two perfect squares. For example, 10 is a double-square because
    10 = 3^2 + 1^2. Your task in this problem is, given X, determine the
    number of ways in which it can be written as the sum of two squares.
</p>
<p>
    For example, 10 can only be written as 3^2 + 1^2
    (we don&apos;t count 1^2 + 3^2 as being different).
    On the other hand, 25 can be written as 5^2 + 0^2 or as 4^2 + 3^2.
<br>
    NOTE: Do NOT attempt a brute force approach. It will not work.
    The following constraints hold:
<br>
    0 &lt;= X &lt;= 2147483647
<br>
    1 &lt;= N &lt;= 100
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    You should first read an integer N, the number of test cases.
    The next N lines will contain N values of X.
</p>
<pre class="description-input-output">5
10
25
3
0
1</pre>

<h3>Output sample:</h3>

<p>
    E.g.
</p>
<pre class="description-input-output">1
2
0
1
1</pre>