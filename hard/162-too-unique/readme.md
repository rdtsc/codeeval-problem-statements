<h2>Too unique</h2>

<h3>Challenge Description:</h3>
<p>
    You are given a matrix of size N&#xD7;M elements, filled with lowercase ASCII letters from &#x2018;a&#x2019; to &#x2018;z&#x2019;. Find the max size
    of rectangular contiguous submatrix of unique (i.e. non repeated within a given submatrix) elements. Find all
    submatrices of unique elements of this size and replace their elements with asterisks &#x2018;*&#x2019;.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains the input matrix. E.g.
</p>

<pre>rzqicaiiaege
ccwnulljybtu
jxtxupauwuah
oqikzgqrzpdq
vblalwdjbdwn
ahjeencuclbo</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the result of the matrix with replaced elements, where all elements of the biggest submatrixes
    of unique elements are replaced with asterisks &#x2018;*&#x2019;. E.g.
</p>

<pre>rzqicaiiae**
ccwnulljyb**
jxtx***uwu**
oqik****zp**
vbla****bd**
ahje****cl**</pre>

<h3>Constraints:</h3>
<ol>
<li>The size of matrix in the input is 60&#xD7;20 elements.</li>
</ol>