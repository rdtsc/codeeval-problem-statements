<h2>Detecting Cycles</h2>

<h3>Challenge Description:</h3>

<p>
    Given a sequence, write a program to detect cycles within it.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename
    containing a sequence of numbers (space delimited). The file can have multiple such lines. E.g
</p>
<pre class="description-input-output">2 0 6 3 1 6 3 1 6 3 1
3 4 8 0 11 9 7 2 5 6 10 1 49 49 49 49
1 2 3 1 2 3 1 2 3</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the first cycle you find in each sequence. Ensure that there are no trailing empty
    spaces on each line you print. E.g.
</p>
<pre class="description-input-output">6 3 1
49
1 2 3</pre>
<p>
    The cycle detection problem is explained more widely on <a href="http://en.wikipedia.org/wiki/Cycle_detection">wiki</a>
<br>
    Constrains:
<br>
    The elements of the sequence are integers in range [0, 99]
<br>
    The length of the sequence is in range [0, 50]
</p>