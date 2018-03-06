<h2>Chardonnay or Cabernet</h2>

<h3>Challenge Description:</h3>

<p>
    Your good friend Tom is admirer of tasting different types of fine wines. What he loves even more is to guess their
    names. One day, he was sipping very extraordinary wine. Tom was sure he had tasted it before, but what was its name?
    The taste of this wine was so familiar, so delicious, so pleasant&#x2026; but what is it exactly?
    To find the answer, Tom decided to taste the wines we had. He opened wine bottles one by one, tasted different
    varieties of wines, but still could not find the right one. He was getting crazy, &#x201C;No, it&#x2019;s not that!&#x201D; desperately
    breaking a bottle of wine and opening another one. Tom went off the deep end not knowing what this wine was.
    Everything he could say is just several letters of its name. You can no longer look at it and decided to help him.
<br>Your task is to write a program that will find the wine name, containing all letters that Tom remembers.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case, which contains names of wines and letters
    that Tom remembers. Names and letters are separated by a vertical bar &apos;|&apos;.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">Cabernet Merlot Noir | ot
Chardonnay Sauvignon | ann
Shiraz Grenache | o</pre>

<h3>Output sample:</h3>

<p>
    You should print wine names, containing all letters that Tom remembered. Letters can be anywhere in wine names.
    If there is no name with all letters, print False.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">Merlot
Chardonnay Sauvignon
False</pre>

<h3>Constraints:</h3>
<ol>
<li>Wine name length can be from 2 to 15 characters.</li>
<li>Number of letters that Tom remembered does not exceed 5.</li>
<li>Number of wine names in a test case can be from 2 to 10.</li>
<li>If there is no wine name containing all letters, print False.</li>
<li>The number of test cases is 40.</li>
</ol>