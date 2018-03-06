<h2>Read More</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a text. Write a program which outputs its lines according to the following rules:
</p>
<ol>
<li>If line length is &#x2264; 55 characters, print it without any changes.</li>
<li>If the line length is &gt; 55 characters, change it as follows:</li>
<ol>
<li>Trim the line to 40 characters.</li>
<li>If there are spaces &#x2018;<span> </span>&#x2019; in the resulting string, trim it once again to the last space (the space should be trimmed too).</li>
<li>Add a string &#x2018;<span>... &lt;Read More&gt;</span>&#x2019; to the end of the resulting string and print it.</li>
</ol>
</ol>

<h3>Input sample:</h3>

<p>
    The first argument is a file. The file contains a text.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">Tom exhibited.
Amy Lawrence was proud and glad, and she tried to make Tom see it in her face - but he wouldn&apos;t look.
Tom was tugging at a button-hole and looking sheepish.
Two thousand verses is a great many - very, very great many.
Tom&apos;s mouth watered for the apple, but he stuck to his work.</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the text lines with their length limited according to the rules described above.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">Tom exhibited.
Amy Lawrence was proud and glad, and... &lt;Read More&gt;
Tom was tugging at a button-hole and looking sheepish.
Two thousand verses is a great many -... &lt;Read More&gt;
Tom&apos;s mouth watered for the apple, but... &lt;Read More&gt;</pre>

<h3>Constraints:</h3>
<ol>
<li>The maximum length of a line in the input file is 300 characters.</li>
<li>There cannot be more than one consequent space character in the input data.</li>
</ol>