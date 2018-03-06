<h2>Justify the Text</h2>

<h3>Challenge Description:</h3>
<p>
    Write a program that reformats the text into lines of 80 symbols by stretching the text to full line width by adding
    extra spaces.
</p>
<p>
    Longer series of spaces should go first. For example:
</p>
<ul>
<li>if you need to add just one extra space, add it between the first and the second word</li>
<li>if there are 4 words in a line, and you need 10 spaces to stretch the text up to 80 symbols, add 4 spaces
        between the first and the second word, 3 spaces between the second and the third word, and 3 spaces between
        the third and the fourth word.
</li>
</ul>
<p>
    The last line of the paragraph remains unchanged.
</p>

<h3>Input sample:</h3>
<p>
    The first argument is a filename. The input file contains a text.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">Hello, World!
The precise 50-digits value of Pi is 3.14159265358979323846264338327950288419716939937510.
But he who would be a great man ought to regard, not himself or his interests, but what is just, whether the just act be his own or that of another. Next as to habitations. Such is the tradition.</pre>

<h3>Output sample:</h3>
<p>
    Print to stdout the text, reformatted into lines of 80 symbols by stretching the text to the full line width
    by adding extra spaces.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">Hello, World!
The         precise         50-digits        value        of        Pi        is
3.14159265358979323846264338327950288419716939937510.
But  he  who would be a great man ought to regard, not himself or his interests,
but what is just, whether the just act be his own or that of another. Next as to
habitations. Such is the tradition.</pre>