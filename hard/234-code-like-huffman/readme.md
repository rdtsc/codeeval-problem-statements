<h2>Code like Huffman</h2>

<h3>Challenge Description:</h3>

<p>
    One of the first algorithms for efficient information coding was proposed by David A. Huffman in 1952. The idea of
    the algorithm is the following: knowing the estimated probability or frequency of occurrence for each possible
    value of the source symbol, we can describe the procedure for building variable-length code table for encoding a
    source symbol.<br>
    This algorithm is currently used in many data compression applications, including this challenge.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case which contains letters from which you
    have to build a code table for each character using Huffman algorithm.
</p>

<pre class="description-input-output">abc
ilovecodeeval</pre>

<h3>Output sample:</h3>

<p>
    Use this algorithm to build a code table for each character and print it in an alphabetical order in the
    following way.
</p>

<pre class="description-input-output">a: 10; b: 11; c: 0;
a: 1000; c: 1001; d: 1010; e: 01; i: 1011; l: 110; o: 111; v: 00;</pre>

<h3>Constraints:</h3>
<ol>
<li>The test case can include lowercase characters only.</li>
<li>
        When building a binary tree, if the priority of items is the same, the sorting should be done in an
        alphabetical order, that is: <br>
<br>
        If the priority of items is the same then Node has higher priority than symbol. If 2 Nodes have same priority
        then sorting should be done in an alphabetical order.
</li>
<li>Test case can include from 3 to 30 characters.</li>
<li>The number of test cases is 40.</li>
</ol>