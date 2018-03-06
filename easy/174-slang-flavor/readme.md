<h2>Slang Flavor</h2>

<h3>Challenge Description:</h3>
<p>
    Long serious texts are boring. Write a program that will make texts more informal: replace every
    other end punctuation mark (period &#x2018;.&#x2019;, exclamation mark &#x2018;!&#x2019;, or question mark &#x2018;?&#x2019;) with one of
    the following slang phrases, selecting them one after another:
</p>
<style>
    span.fw {
        color: #000000;
        font-family: "andale mono", consolas, monaco, "lucida console", "courier new", courier, monospace;
    }
</style>
<ol>
<li>&#x2018;<span class="fw">, yeah!</span>&#x2019;</li>
<li>&#x2018;<span class="fw">, this is crazy, I tell ya.</span>&#x2019;</li>
<li>&#x2018;<span class="fw">, can U believe this?</span>&#x2019;</li>
<li>&#x2018;<span class="fw">, eh?</span>&#x2019;</li>
<li>&#x2018;<span class="fw">, aw yea.</span>&#x2019;</li>
<li>&#x2018;<span class="fw">, yo.</span>&#x2019;</li>
<li>&#x2018;<span class="fw">? No way!</span>&#x2019;</li>
<li>&#x2018;<span class="fw">. Awesome!</span>&#x2019;</li>
</ol>
<p>
    The result should be funny.
</p>

<h3>Input sample:</h3>
<p>
    The first argument is a file that contains a text.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">Lorem ipsum dolor sit amet. Mea et habeo doming praesent. Te inani utroque recteque has, sea ne fugit verterem!
Usu ei scripta phaedrum, an sed salutatus definiebas? Qui ut recteque gloriatur reformidans. Qui solum aeque sapientem cu.
Eu nam nusquam quaestio principes.</pre>

<h3>Output sample:</h3>
<p>
    Print to stdout the results: the text with slang phrases.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">Lorem ipsum dolor sit amet. Mea et habeo doming praesent, yeah! Te inani utroque recteque has, sea ne fugit verterem!
Usu ei scripta phaedrum, an sed salutatus definiebas, this is crazy, I tell ya. Qui ut recteque gloriatur reformidans. Qui solum aeque sapientem cu, can U believe this?
Eu nam nusquam quaestio principes.</pre>

<h3>Constraints:</h3>
<ol>
<li>In the input text, end punctuation mark cannot come one after another (consequent).</li>
<li>Input text contains 40 lines.</li>
</ol>