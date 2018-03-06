<h2>Fizz Buzz</h2>

<h3>Challenge Description:</h3>

<p>
    Players generally sit in a circle. The first player says the number &#x201C;1&#x201D;, and each player says next number in turn.
    However, any number divisible by X (for example, three) is replaced by the word <em>fizz</em>, and any divisible
    by Y (for example, five) by the word <em>buzz</em>. Numbers divisible by both become <em>fizz buzz</em>. A player
    who hesitates, or makes a mistake is eliminated from the game.
</p>
<p>
    Write a program that prints out the final series of numbers where those divisible by X, Y and both are replaced
    by &#x201C;F&#x201D; for <em>fizz</em>, &#x201C;B&#x201D; for <em>buzz</em> and &#x201C;FB&#x201D; for <em>fizz buzz</em>.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a file as its first argument. The file contains multiple separated lines; each line
    contains 3 numbers that are space delimited. The first number is the first divider (X), the second number is
    the second divider (Y), and the third number is how far you should count (N). You may assume that the input file
    is formatted correctly and the numbers are valid positive integers.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">3 5 10
2 7 15</pre>

<h3>Output sample:</h3>

<p>
    Print out the series 1 through N replacing numbers divisible by X with &#x201C;F&#x201D;, numbers divisible by Y with &#x201C;B&#x201D;
    and numbers divisible by both with &#x201C;FB&#x201D;. Since the input file contains multiple sets of values, your output
    should print out one line per set. Ensure that there are no trailing empty spaces in each line you print.
</p>

<pre class="description-input-output">1 2 F 4 B F 7 8 F B
1 F 3 F 5 F B F 9 F 11 F 13 FB 15</pre>
<h3>Constraints:</h3>
<ul>
<li>The number of test cases &#x2264; 20</li>
<li>&quot;X&quot; is in range [1, 20]</li>
<li>&quot;Y&quot; is in range [1, 20]</li>
<li>&quot;N&quot; is in range [21, 100]</li>
</ul>