<h2>Number Pairs</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a sorted array of positive integers and a number &apos;X&apos;.
    Print out all pairs of numbers whose sum is equal to X.
    Print out only unique pairs and the pairs should be in ascending order
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a filename.
    This file will contain a comma separated list of sorted numbers and then the sum &apos;X&apos;,
    separated by semicolon. Ignore all empty lines. If no pair exists, print the string NULL e.g.
</p>
<pre>1,2,3,4,6;5
2,4,5,6,9,11,15;20
1,2,3,4;50</pre>

<h3>Output sample:</h3>

<p>
    Print out the pairs of numbers that equal to the sum X.
    The pairs should themselves be printed in sorted order i.e the first
    number of each pair should be in ascending order. E.g.
</p>

<pre>1,4;2,3
5,15;9,11
NULL</pre>