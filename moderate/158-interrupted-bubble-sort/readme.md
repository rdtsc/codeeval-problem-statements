<h2>Interrupted Bubble Sort</h2>

<h3>Challenge Description:</h3>

<p>Bubble sort is the simplest algorithm for elements sorting. At each iteration we sequentially compare values of subsequent elements and swap them if necessary.</p>
<p>Your job is to write a program which finds a state of a given list of positive integer numbers after applying a given count of bubble sort iterations.</p>

<h3>Input sample:</h3>

<p>Your program should accept as its first argument a path to a filename. Each line in this file contains a space-separated list of positive integers and ends with a number of iterations, separated by vertical line &#x2018;|&#x2019;. E.g.:</p>

<pre class="description-input-output">36 47 78 28 20 79 87 16 8 45 72 69 81 66 60 8 3 86 90 90 | 1
40 69 52 42 24 16 66 | 2
54 46 0 34 15 48 47 53 25 18 50 5 21 76 62 48 74 1 43 74 78 29 | 6
48 51 5 61 18 | 2
59 68 55 31 73 4 1 25 26 19 60 0 | 2</pre>

<h3>Output sample:</h3>

<p>Print to stdout the state of given lists after applying a given count of bubble sort iterations. E.g.:</p>

<pre class="description-input-output">36 47 28 20 78 79 16 8 45 72 69 81 66 60 8 3 86 87 90 90
40 42 24 16 52 66 69
0 15 25 18 34 5 21 46 47 48 48 1 43 50 53 29 54 62 74 74 76 78
5 48 18 51 61
55 31 59 4 1 25 26 19 60 0 68 73</pre>