<h2>Code combinations</h2>

<h3>Challenge Description:</h3>

<p>
    You definitely know the game where you have to make as many words from the given letters as possible. In our case,
    the rules are a bit different: you need to check whether it is possible to make the word &apos;code&apos; with the four given
    letters, and, if possible, count how many times you can do this. Letters can be in a various order.
</p>

<p>
    Solution example:
</p>

<pre class="description-input-output">| * * * * |
| * c o * |     | c o |  =  1
| * d e * |     | d e |</pre>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with symbol matrix. Each line of the matrix
    is separated by a pipeline  &apos;|&apos;.
</p>

<pre class="description-input-output">**** | *co* | *de* | ****
codx | decx
co | dx</pre>

<h3>Output sample:</h3>

<p>
    You need to calculate and print a number that will tell how many times you can make the word &#x2018;code&#x2019; from the
    letters in the matrix, using a 2x2 submatrix.
</p>

<pre class="description-input-output">1
2
0</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of rows or columns in the matrix can be from 2 to 10.</li>
<li>Matrix can include one face for 2 solutions in case.</li>
<pre class="description-input-output">| c o d x |     | c o |     | o d |  =  2
| d e c x |     | d e |     | e c |</pre>
<li>The number of test cases is 40.</li>
</ol>