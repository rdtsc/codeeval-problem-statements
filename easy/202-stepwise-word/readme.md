<h2>Stepwise word</h2>

<h3>Challenge Description:</h3>

<p>
    Print the longest word in a stepwise manner.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line contains a test case with a list of words
    that have different or the same length.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">cat dog hello
stop football play
music is my life</pre>

<h3>Output sample:</h3>

<p>
    Find the longest word in each line and print it in  one line in a stepwise manner.
    Separate each new step with a space. If there are several words of the same length and
    they are the longest, then print the first word from the list.
</p>

<pre class="description-input-output">h *e **l ***l ****o
f *o **o ***t ****b *****a ******l *******l
m *u **s ***i ****c</pre>

<h3>Constraints:</h3>
<ol>
<li>The word length is from 1 to 10 characters.</li>
<li>The number of words in a line is from 5 to 15.</li>
<li>If there are several words of the same length and they are the longest, then print the first word from the list.</li>
<li>The number of test cases is 40.</li>
</ol>