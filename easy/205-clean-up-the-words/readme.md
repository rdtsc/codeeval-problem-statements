<h2>Clean up the words</h2>

<h3>Challenge Description:</h3>

<p>
    You have a list of words. Letters of these words are mixed with extra symbols, so it is hard to define
    the beginning and end of each word. Write a program that will clean up the words from extra numbers and symbols.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with a list of words:
    letters are both lowercase and uppercase, and are mixed with extra symbols.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">(--9Hello----World...--)
Can 0$9 ---you~
13What213are;11you-123+138doing7</pre>

<h3>Output sample:</h3>

<p>
    Print the cleaned up words separated by spaces in lowercase letters.
</p><p>
    For example:
</p>

<pre class="description-input-output">hello world
can you
what are you doing</pre>

<h3>Constraints:</h3>
<ol>
<li>Print the words separated by spaces in lowercase letters.</li>
<li>The length of a test case together with extra symbols can be in a range from 10 to 100 symbols.</li>
<li>The number of test cases is 40.</li>
</ol>