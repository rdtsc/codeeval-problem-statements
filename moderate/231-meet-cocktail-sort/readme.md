<h2>Meet Cocktail sort</h2>

<h3>Challenge Description:</h3>

<p>
    Quite often we need to arrange items in a certain order: numbers in an ascending or descending order, words &#x2013; in an
    alphabetical order, people &#x2013; according to their height, and so on. There are many different sorting algorithms.
    Some of them are quick, while others seem to suit in a particular case only. <br>
    In this challenge, your task is to use a cocktail sort.

</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with numbers that you need to order using
    cocktail sort. There is also a number of iterations for an algorithm to carry out. The numbers themselves and the
    number of iterations are separated by a pipeline &apos;|&apos;.
</p>

<pre class="description-input-output">5 4 9 10 7 3 2 1 6 | 1
9 8 7 6 5 4 3 2 1 | 3</pre>

<h3>Output sample:</h3>

<p>
    Print sorted numbers after they pass the required number of iterations. One iteration of a cocktail sort is a pass
    through the list of numbers in both directions: from the beginning to the end and from the end to the beginning.
</p>

<pre class="description-input-output">1 4 5 9 7 3 2 6 10
1 2 3 6 5 4 7 8 9</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of iterations can be from 1 to 30.</li>
<li>One iteration of a cocktail sort is a pass through the list of numbers in both directions: from the beginning
        to the end and from the end to the beginning.</li>
<li>The number of test cases is 40.</li>
</ol>