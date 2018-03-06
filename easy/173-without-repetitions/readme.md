<h2>Without Repetitions</h2>

<h3>Challenge Description:</h3>

<p>
    In a given text, if there are two or more identical characters in sequence, delete the repetitions and leave only
    the first character.
</p>
<p>
    For example:
</p>
<pre>Shellless mollusk lives in wallless house in wellness. Aaaarrghh!

&#x2193;

Sheles molusk lives in wales house in welnes. Aargh!</pre>

<h3>Input sample:</h3>

<p>
    The first argument is a file. The file contains a text.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">But as he spake he drew the good sword from its scabbard, and smote a heathen knight, Jusssstin of thee Iron Valley.
No matttter whom you choose, she deccccclared, I will abide by your decision.
Wwwhat is your will?
At his magic speech the ground oppened and he began the path of descent.
I should fly away and you would never see me again.</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the text in which all repetitions are deleted.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">But as he spake he drew the god sword from its scabard, and smote a heathen knight, Justin of the Iron Valey.
No mater whom you chose, she declared, I wil abide by your decision.
Wwhat is your wil?
At his magic spech the ground opened and he began the path of descent.
I should fly away and you would never se me again.</pre>

<h3>Constraints:</h3>
<ol>
<li>The text is case-sensitive:  &#x2018;a&#x2019; and &#x2018;A&#x2019; are <strong>different</strong> characters.</li>
<li>The input consists of 40 text lines.</li>
<li>The maximum size of the text is 10 KB.</li>
</ol>