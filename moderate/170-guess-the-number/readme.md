<h2>Guess the Number</h2>

<h3>Challenge Description:</h3>

<p>
    Let&#x2019;s play &#x201C;Guess the number&#x201D; game. This game is for two players, and it has simple rules:
</p>
<ul>
<li>one person (master) picks an integer in a certain range (for example, from 0 to 100 inclusive)</li>
<li>another person (you) tries to guess it in a certain number of attempts.</li>
</ul>
<p>
    The task is facilitated by the fact that after each attempt, a master gives you a hint whether the number is
    higher or lower.
</p>

<p>
    A reasonable approach to this game is to use the &#x201C;divide and conquer&#x201D; principle: in a range of numbers, always select
    a middle number. Then, based on the received response, discard the upper or the lower half of this range
    (together with the selected number) as it cannot contain the right answer.
    Now, the range of numbers is halved. Again, select the middle number. (If the number of integers in the range is even,
    select the greater one out of two middle numbers.) Repeat until you hear &#x201C;Yay!&#x201D; from a master&#xA0;&#x2014; you guessed the number.
</p>

<p>
    With this algorithm, you can win in at most log<sub>2</sub> N attempts, where N is the range size.
</p>

<h3>Game example</h3>

<p>
    Guess the number in an inclusive range 0..9, where computer is a master (also see the diagram below):
</p>

<pre>Computer: range form 0 to 9
Player:   5
Computer: Higher!
Player:   8
Computer: Lower!
Player:   7
Computer: Yay!</pre>

<h3>Input sample:</h3>

<p>
    The task in this challenge is to guess the number. Because you have to use the proposed algorithm, we know all your
    answers in advance. Thus, your program should take the path to the file, in which each row stands for a different
    game, as first argument.

    At the beginning of each line, upper bound of the range is specified (the lower bound is 0, both are included in the
    range).
    Then, master&#x2019;s answers go, separated by spaces. E.g.
</p>

<pre class="description-input-output">100 Lower Lower Higher Lower Lower Lower Yay!
948 Higher Lower Yay!</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout a single guessed number for each row. E.g.
</p>

<pre class="description-input-output">13
593</pre>