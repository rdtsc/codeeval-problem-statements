<h2>Meet Comb sort</h2>

<h3>Challenge Description:</h3>

<p>
    Comb sort is a simplified sorting algorithm, an improvement of a bubble sort algorithm. It competes in speed with
    a well-known quick sort algorithm. <br>
    The main idea of this sorting algorithm is that a gap between elements can be more than 1.<br>
    Such algorithm is used in this challenge.<br>

</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Every row includes a test case with numbers that you need to sort using
    comb sort algorithm.
</p>

<pre class="description-input-output">3 1 2
5 4 3 2 1</pre>

<h3>Output sample:</h3>

<p>
    Count and print number of iterations it will take to sort the test case using comb sort. Iteration is a pass
    through the list of numbers using the same range between the compared elements. When a pass starts from the
    beginning &#x2013; it&#x2019;s a new iteration. If a range is, for example, 3, then take elements 0 and 3, then 1 and 4 etc.
</p>

<pre class="description-input-output">2
3</pre>

<h3>Constraints:</h3>
<ol>
<li>Decrease factor for the algorithm is 1.25; round the result to a smaller number.</li>
<li>If a range is, for example, 3, then take elements 0 and 3, then 1 and 4 etc.</li>
<li>One iteration for this algorithm is a pass through the list of numbers to the end using the same range
        between the compared elements.</li>
<li>The number of test cases is 40.</li>
</ol>