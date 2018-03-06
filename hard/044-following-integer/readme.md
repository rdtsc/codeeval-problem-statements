<h2>Following Integer</h2>

<h3>Challenge Description:</h3>
<p>
    Credits: This challenge has appeared in a past google competition
<br>
<br>
    You are writing out a list of numbers.Your list contains all numbers with exactly
    Di digits in its decimal representation which are equal to i, for each i between 1 and 9, inclusive.
    You are writing them out in ascending order. For example, you might be writing every number with
    two &apos;1&apos;s and one &apos;5&apos;. Your list would begin 115, 151, 511, 1015, 1051. Given N,
    the last number you wrote, compute what the next number in the list will be.
    The number of 1s, 2s, ..., 9s is fixed but the number of 0s is arbitrary.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is one test case. Each test case will contain an integer n &lt; 10^6. E.g.
</p>
<pre>115
842
8000</pre>

<h3>Output sample:</h3>

<p>
    For each line of input, generate a line of output which is the next integer in the list. E.g.
</p>
<pre>151
2048
80000</pre>