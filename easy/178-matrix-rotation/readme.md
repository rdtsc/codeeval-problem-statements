<h2>Matrix Rotation</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a 2D N&#xD7;N matrix. Each element of the matrix is a letter: from &#x2018;a&#x2019; to &#x2018;z&#x2019;. Your task is to rotate
    the matrix 90&#xB0; clockwise:
</p>

<pre>a b c        g d a
d e f  =&gt;    h e b
g h i        i f c</pre>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains 2D N&#xD7;N matrices, presented in a serialized form (starting from the
    upper-left element), one matrix per line. The elements of a matrix are separated by spaces.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">a b c d
a b c d e f g h i j k l m n o p
a b c d e f g h i</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout matrices rotated 90&#xB0; clockwise in a serialized form (same as in the input sample).
</p>
<p>
    For example:
</p>

<pre class="description-input-output">c a d b
m i e a n j f b o k g c p l h d
g d a h e b i f c</pre>

<h3>Constraints:</h3>
<ol>
<li>The N size of the matrix can be from 1 to 10</li>
<li>The number of test cases is 100</li>
</ol>