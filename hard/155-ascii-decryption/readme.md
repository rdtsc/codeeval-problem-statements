<h2>ASCII Decryption</h2>

<h3>Challenge Description:</h3>

<p>
    You are an analyst at the Central Intelligence Agency, and you have intercepted a top secret encrypted message which
    contains numbers. Each number is obtained by taking an ASCII code of the original character and adding some unknown
    constant <em>N</em>.
</p>
<p>
    For example, you can encrypt the word &apos;test&apos; with the condition that <em>N</em> = 11.
</p>
<p>
    &apos;test&apos; to ASCII -&gt; 116 101 115 116 -&gt; add <em>N</em> to each number-&gt; 127 112 126 127
</p>
<p>
    Based on previous intelligence reports, you know that the original message includes two identical words consisting
    of <em>X</em> characters and you know the last letter in the word.
</p>
<p>
    Your challenge is to decrypt the message.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
</p>
<p>
    Each line of input consists of three parts: length of a word, which is repeated twice, the last letter of this word,
    and an encrypted message separated with space:
</p>

<pre class="description-input-output">5 | s | 92 112 109 40 118 109 109 108 123 40 119 110 40 124 112 109 40 117 105 118 129 40 119 125 124 127 109 113 111 112 40 124 112 109 40 118 109 109 108 123 40 119 110 40 124 112 109 40 110 109 127 54 40 53 40 91 120 119 107 115</pre>

<h3>Output sample:</h3>

<p>
    For each line of input print out decrypted message:
</p>

<pre class="description-input-output">The needs of the many outweigh the needs of the few. - Spock</pre>

<br>