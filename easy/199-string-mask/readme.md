<h2>String mask</h2>

<h3>Challenge Description:</h3>

<p>
    You&#x2019;ve got a binary code which has to be buried among words in order to unconsciously pass the cipher. <br>
    Create a program that would cover the word with a binary mask. If, while covering, a letter finds itself as 1, you
    have to change its register to the upper one, if  it&#x2019;s 0, leave it as it is. Words are always in lower case
    and in the same row with the binary mask.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each row contains a test case with a word and a binary code separated
    with space, inside of it. The length of each word is equal to the length of the binary code.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">hello 11001
world 10000
cba 111</pre>

<h3>Output sample:</h3>

<p>
    Print the encrypted words without binary code.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">HEllO
World
CBA</pre>

<h3>Constraints:</h3>
<ol>
<li>Words are from 1 to 20 letters long.</li>
<li>The number of test cases is 40.</li>
</ol>