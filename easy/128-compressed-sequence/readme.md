<h2>Compressed Sequence</h2>

<h3>Challenge Description:</h3>
<p>
    Assume that someone dictates you a sequence of numbers, and you need to write it down. For brevity, he dictates
    it as follows: first he dictates the number of consecutive identical numbers, and then - the number itself.
</p>

<p>
    For example:<br>
    The sequence below
</p>

<pre>1 1 3 3 3 2 2 2 2 14 14 14 11 11 11 2</pre>

<p>is dictated as follows:</p>

<pre><i>two times one, three times three, four times two, three times fourteen, three times eleven, one time two</i></pre>

<p>and  you have to write down the sequence</p>

<pre>2 1 3 3 4 2 3 14 3 11 1 2</pre>

<p>Your task is to write a program that compresses a given sequence using this approach.</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a file as its first argument that contains T number of lines. Each line is
    a test case represented by a sequence of integers with the length L, where each integer is N separated by a space.
</p>

<pre class="description-input-output">40 40 40 40 29 29 29 29 29 29 29 29 57 57 92 92 92 92 92 86 86 86 86 86 86 86 86 86 86
73 73 73 73 41 41 41 41 41 41 41 41 41 41
1 1 3 3 3 2 2 2 2 14 14 14 11 11 11 2
7</pre>

<h3>Output sample:</h3>

<p>For each test case, print out a compressed sequence of numbers separated by a single space, one per line.</p>

<p>For example:</p>

<pre class="description-input-output">4 40 8 29 2 57 5 92 10 86
4 73 10 41
2 1 3 3 4 2 3 14 3 11 1 2
1 7</pre>

<h3>Constraints:</h3>

<ul>
<li>T is in a range from 20 to 50.</li>
<li>N is in a range from 0 to 99.</li>
<li>L is in a range from 1 to 400.</li>
</ul>