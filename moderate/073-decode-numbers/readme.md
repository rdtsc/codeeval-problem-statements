<h2>Decode Numbers</h2>

<h3>Challenge Description:</h3>

<p>
    You are given an encoded message containing only numbers. You are also
    provided with the following mapping:
</p>
<pre>A : 1
B : 2
C : 3
...
Z : 26
</pre>
<p>
    Given an encoded message, count the number of ways it can be decoded.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is a test-case and contains an encoded message of
    numbers. E.g.
</p>
<pre class="description-input-output">12
123</pre>
<p>
    You may assume that the test cases contain only numbers.
</p>

<h3>Output sample:</h3>

<p>
    Print out the different number of ways it can be decoded. E.g.
</p>
<pre class="description-input-output">2
3</pre>
<p>
    NOTE: 12 could be decoded as AB(1 2) or L(12). Hence the number of ways to decode 12 is 2.
</p>