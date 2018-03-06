<h2>Text to Number</h2>

<h3>Challenge Description:</h3>
<p>
    You have a sting which contains a number represented as English text.
    Your task is to translate these numbers into their integer representation.
    The numbers can range from negative 999,999,999 to positive 999,999,999.
    The following is an exhaustive list of English words that your
    program must account for:
</p>
<pre>negative,
zero, one, two, three, four, five, six, seven, eight, nine,
ten, eleven, twelve, thirteen, fourteen, fifteen, sixteen, seventeen, eighteen, nineteen,
twenty, thirty, forty, fifty, sixty, seventy, eighty, ninety,
hundred,
thousand,
million
</pre>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Input example is the following
</p>
<pre>fifteen
negative six hundred thirty eight
zero
two million one hundred seven</pre>
<p>
    - Negative numbers will be preceded by the word negative.
<br>
    - The word &quot;hundred&quot; is not used when &quot;thousand&quot; could be. E.g. 1500 is written &quot;one thousand five hundred&quot;, not &quot;fifteen hundred&quot;.
</p>

<h3>Output sample:</h3>

<p>
    Print results in the following way.
</p>

<pre>15
-638
0
2000107</pre>