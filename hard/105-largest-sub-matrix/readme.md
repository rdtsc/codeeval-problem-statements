<h2>Largest Sub-Matrix</h2>

<h3>Challenge Description:</h3>
<p>
    You have the matrix of positive and negative integers. Find a sub-matrix with the largest sum of its elements.
    In this case sub-matrix means a continuous rectangular part of the given matrix. There is no limitation for
    sub-matrix dimensions. It only has to be rectangular.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Read the matrix from this file.
    Example of the matrix is the following:
</p>

<pre>-1 -4 -5 -4
-5 8 -1 3
-2 1 3 2
1 5 6 -9</pre>

<p>
    After some calculations you may find that the sub-matrix with the largest sum of the input is:
</p>

<pre>8 -1
1 3
5 6</pre>

<h3>Output sample:</h3>

<p>
    Print out the sum of elements for the largest sub-matrix. For the given
    input it is:
</p>

<pre>22</pre>

<h3>Costraints:</h3>
<ol>
<li>Each element in the matrix is in range [-100, 100].</li>
<li>Input matrix has an equal number of rows and columns.</li>
<li>There are up to 20 rows and columns in the input file.</li>
</ol>