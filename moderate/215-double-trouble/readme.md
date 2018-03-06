<h2>Double trouble</h2>

<h3>Challenge Description:</h3>

<p>
    Historians have discovered a mysterious lost code that until this day remains undeciphered. Looks like the code
    dates back to the 5th century AD. Scientists were trying to decipher the code, which could reveal many details
    about our ancestors&#x2019; life, but they failed. Could you help them? <br>
    According to the analysis, there can be only 2 letters in the code: A and B. All messages are transmitted in a
    form of two equal parts (ABAB, AAAA, BABA, and so on).
<br>
    Some messages are so mutilated that scientists need to know how many correct variants of the messages might exist
    to decide whether it would make sense to decipher their meaning, and how long it would take. Therefore, you need
    to calculate the number of possible correct variants for each message.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case containing one message that includes
    three symbols: <br>
    A and B &#x2013; deciphered code; <br>
    * - lost letter;
</p>

<p>
    For example:
</p>

<pre class="description-input-output">ABA*
BAA*
A*A*</pre>

<h3>Output sample:</h3>

<p>
    Print the number of possible correct variants of each message.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">1
0
2</pre>

<h3>Constraints:</h3>
<ol>
<li>A message may be from 2 to 70 letters long.</li>
<li>All messages have an even number of letters.</li>
<li>Some messages may be incorrect. In such cases, print 0.</li>
<li>The number of test cases is 40.</li>
</ol>