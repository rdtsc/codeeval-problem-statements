<h2>Brainf*ck</h2>

<h3>Challenge Description:</h3>

<p>
    Looking for something utterly mind-blowing? Look no further, you hit the right place!<br>
    This challenge is inextricably linked with Brainf*ck, the most famous esoteric programming
    language invented by Urban M&#xFC;ller. Is this the first time you hear about Brainf*ck? Find out more
<a href="https://en.wikipedia.org/wiki/Brainfuck" target="_blank">Brainf*ck (wiki)</a>
</p>

<p>
    Brainf*ck consists of only 8 basic commands:<br>
<b>&gt;</b> - move to the next cell;<br>
<b>&lt;</b> - move to the previous cell;<br>
<b>+</b> - increment the value in the current cell by 1;<br>
<b>-</b> - decrement the value of the current cell by 1;<br>
<b>.</b> - output the value of the current cell;<br>
<b>,</b> - input the value outside and store it in the current cell;<br>
<b>[</b> - if the value of the current cell is zero, move forward on the text to the program to] taking into account
    nesting;<br>
<b>]</b> - if the value of the current cell is not zero, go back on the text of the program to [considering nesting;
</p>

<p>
    So, you should write a program that will get the code on the Brainf*ck language, calculate this code, and display
    the final result of the program. It can be a simple output of letters or a complex cycle; in any case,
    your program should handle it.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case where there is a program written
    on the Brainf*ck language.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">+[---&gt;++&lt;]&gt;+++.[-&gt;+++++++&lt;]&gt;.[---&gt;+&lt;]&gt;----.
++++++++++[&gt;+++++++&gt;++++++++++&gt;+++&gt;+&lt;&lt;&lt;&lt;-]&gt;++.&gt;+.+++++++..+++.&gt;++.&lt;&lt;+++++++++++++++.&gt;.+++.------.--------.&gt;+.</pre>

<h3>Output sample:</h3>

<p>
    You should print the result of the program that you will get.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">Yo!
Hello World!</pre>

<h3>Constraints:</h3>
<ol>
<li>Programs can include the code of any complexity.</li>
<li>The number of test cases is 10.</li>
</ol>