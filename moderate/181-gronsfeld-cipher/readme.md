<h2>Gronsfeld cipher</h2>

<h3>Challenge Description:</h3>

<p>You are given a key and an enciphered message. The message was enciphered with the following vocabulary:</p>

<pre> !&quot;#$%&amp;&apos;()*+,-./0123456789:&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz</pre>

<p>Note: The first symbol is space.</p>

<p>Your task is to decipher the message that was enciphered with the Gronsfeld cipher using the given key.</p>

<p>
    The Gronsfeld cipher is a kind of the
<a href="http://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher" target="_blank">Vigen&#xE8;re cipher</a>
    and is similar to the <a href="http://en.wikipedia.org/wiki/Caesar_cipher" target="_blank">Caesar cipher</a>.
    The only difference is that in the Caesar cipher, each character is shifted along by the same number, while in the
    Gronsfeld cipher, each character has its own number of shifts. It means that the length of key for the Gronsfeld
    cipher must be the same as the length of the message. But since it is difficult to remember such a key, especially
    if the message is long, the key of the message is repeated until it has the same length as the message.
</p>

<p>For example:</p>

<p>For the word &quot;EXALTATION&quot; and the key &quot;31415&quot;, the ciphertext is the following:</p>

<p>Accordingly, enciphered message is the following:</p>

<pre>HYEMYDUMPS</pre>

<h3>Input sample:</h3>

<p>
    The first argument is a file with different test cases (there are possible test cases with spaces at enciphered message).
    Each test case contains a key and an enciphered message separated by semicolon.<br>
    For example:
</p>

<pre class="description-input-output">31415;HYEMYDUMPS
45162;M%muxi%dncpqftiix&quot;
14586214;Uix!&amp;kotvx3</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout a deciphered message.<br>
    For example:
</p>

<pre class="description-input-output">EXALTATION
I love challenges!
Test input.</pre>

<h3>Constraints:</h3>
<ol>
<li>To decode a message, use the following alphabet: &quot; !&quot;#$%&amp;&apos;()*+,-./0123456789:&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz&quot;</li>
<li>Number of test cases is 40.</li>
</ol>