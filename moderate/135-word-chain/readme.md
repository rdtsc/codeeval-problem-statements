<h2>Word chain</h2>

<h3>Challenge Description:</h3>
<p>
    In this challenge, we suggest playing &quot;Word chain&quot; - a well-known game in which players come up with words that
    begin with the letter that the previous word ended with. Your task is to determine the maximum length of a chain
    that can be created from a list of words.
</p>

<h3>Input sample:</h3>

<p>
    Your program should accept a path to a filename as its first argument. Each line of the file contains a list of
    words separated by comma.
</p>

<p>For example:</p>

<pre class="description-input-output">soup,sugar,peas,rice
ljhqi,nrtxgiu,jdtphez,wosqm
cjz,tojiv,sgxf,awonm,fcv</pre>

<h3>Output sample:</h3>

<p>
    Print out the length of the longest chain or print out &quot;None&quot; if there is no chain.
</p>

<p>For example:</p>

<pre class="description-input-output">4
None
2</pre>

<h3>Constraints:</h3>

<ul>
<li>The length of a list of words is in a range from 4 to 35.</li>
<li>A word in a list is represented by a random lowercase ASCII string with the length from 3 to 7 letters.</li>
<li>The words in a list do not repeat.</li>
</ul>