<h2>Burrows-Wheeler transform</h2>

<h3>Challenge Description:</h3>

<p>
    You are trying to unpack a text compressed using run-length encoding (the algorithm described in the Compressed
    Sequence challenge). You are doing everything right, but get absolutely ridiculous results. As it came out, before
    the compression, somebody used the Burrows-Wheeler algorithm. It allows increasing the number of repeated
    characters in the text, and thus, increase the efficiency of compression. This method is used by the bzip2 utility.
</p>

<p>
    Let&#x2019;s examine the line processing using the Burrows-Wheeler algorithm. First of all, we should mark the end of the
    line with a special character (EOF), it is $ in this case. Then, generate all possible rotations of the line,
    sort them alphabetically and construct a new string&#xA0;&#x2014; Burrows-Wheeler transform &#xA0;&#x2014; from the
    last characters of each rotation.
</p><p>
    For example, the line &#x2018;easy-peasy&#x2019; is transformed as follows:
</p>
<table>
<tbody><tr>
<td><pre><b>Input</b></pre></td>
<td><pre><b>All rotations</b></pre></td>
<td><pre><b>Sorted rotations</b></pre></td>
<td><pre><b>Output</b></pre></td>
</tr>
<tr>
<td><pre>easy-peasy$</pre></td>
<td>
<pre>easy-peasy$
$easy-peasy
y$easy-peas
sy$easy-pea
asy$easy-pe
easy$easy-p
peasy$easy-
-peasy$easy
y-peasy$eas
sy-peasy$ea
asy-peasy$e
</pre>
</td>
<td>
<pre>$easy-peasy
-peasy$easy
asy$easy-pe
asy-peasy$e
easy$easy-p
easy-peasy$
peasy$easy-
sy$easy-pea
sy-peasy$ea
y$easy-peas
y-peasy$eas
</pre>
</td>
<td><pre>yyeep$-aass</pre></td>
</tr>
</tbody></table>

<p>
    The Burrows-Wheeler algorithm is valuable not only because it allows introducing more repetitions in the line
    (we can achieve even better results by simple sorting of all characters), but, with Burrows-Wheeler transform you
    can easily and unambiguously recreate the original text. Your task is to print out the original text.
</p>

<h3>Input sample:</h3>

<p>
    Your program should accept a path to a file as its first argument. Each line of the file is a text transformed
    using the Burrows-Wheeler algorithm. The end of each line is marked with &#x2018;|&#x2019; symbol and it should be stripped
    before you start to process the string.
</p>

<pre class="description-input-output">oooooooo$  ffffffff     ffffffffuuuuuuuuaaaaaaaallllllllbbBbbBBb|
edarddddddddddntensr$  ehhhhhhhhhhhJ aeaaaaaaaaaaalhtf thmbfe           tcwohiahoJ eeec t e |
ooooio,io$Nnssshhhjo  ee  o  nnkkkkkkii |</pre>

<h3>Output sample:</h3>

<p>
    For each test case, print to stdout the original text.
</p>

<pre class="description-input-output">Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo$
James while John had had had had had had had had had had had a better effect on the teacher$
Neko no ko koneko, shishi no ko kojishi$</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of test cases is 20.</li>
<li>The length of each line is from 5 to 1500 characters.</li>
<li>The sorting order of the characters is defined by their ASCII code, that is the character $ (code 36) goes
        before the letters of the alphabet.</li>
</ol>