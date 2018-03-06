<h2>Jolly Jumpers</h2>

<h3>Challenge Description:</h3>
<p>
    Credits: Programming Challenges by Steven S. Skiena and Miguel A. Revilla
<br>
<br>
    A sequence of n &gt; 0 integers is called a jolly jumper if the absolute values of the differences
    between successive elements take on all possible values 1 through n - 1. eg.
<br>
</p>
<pre>1 4 2 3 </pre>
<p>
    is a jolly jumper, because the absolute differences are 3, 2, and 1, respectively.
    The definition implies that any sequence of a single integer is a jolly jumper. Write a program to determine
    whether each of a number of sequences is a jolly jumper.
<br>
</p>
<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is one test case. Each test case will contain an integer n &lt; 3000 followed by n integers
    representing the sequence. The integers are space delimited.
</p>

<p>For example:</p>

<pre class="description-input-output">4 1 4 2 3
3 7 7 8
9 8 9 7 10 6 12 17 24 38</pre>

<h3>Output sample:</h3>
<p>
    For each line of input generate a line of output saying &apos;Jolly&apos; or &apos;Not jolly&apos;.
</p>

<p>For example:</p>

<pre class="description-input-output">Jolly
Not jolly
Not jolly</pre>