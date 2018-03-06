<h2>Not so clever</h2>

<h3>Challenge Description:</h3>

<p>
    Imagine that you have to arrange items in a certain order: pencils from black to white in a color palette,
    photographs by the date taken, banknotes from the highest to the lowest, etc. To do this, you definitely don&#x2019;t
    need to use the Stupid sort algorithm. <br>
<br>
    After each action, you need to come back to the beginning and start all over again. Not so clever, is it? But,
    you need to know about this algorithm, that&#x2019;s why it is used in this challenge.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case which contains numbers that you need to
    sort using the Stupid sort algorithm. There is also a number of iterations for an algorithm to carry out. The
    numbers themselves and the number of iterations are separated by a pipeline &apos;|&apos;.
</p>

<pre class="description-input-output">4 3 2 1 | 1
5 4 3 2 1 | 2</pre>

<h3>Output sample:</h3>

<p>
    Print sorted numbers after they pass the required number of iterations. One iteration of this sort is a pass to
    the moment of making changes. Once changing the order of the digits, passing starts from the very beginning.
    Hence, this is another iteration.
</p>

<pre class="description-input-output">3 4 2 1
4 3 5 2 1</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of iterations can be from 1 to 8.</li>
<li>One iteration of this sort is a pass to the moment of making changes.</li>
<li>The number of test cases is 40.</li>
</ol>