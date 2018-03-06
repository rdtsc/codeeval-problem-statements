<h2>Reverse and Add</h2>

<h3>Challenge Description:</h3>

<span class="p-like">
    Credits: Programming Challenges by Steven S. Skiena and
    Miguel A. Revilla
</span>
<p>

    The problem is as follows: choose a number, reverse its digits and
    add it to the original. If the sum is not a palindrome (which means,
    it is not the same number from left to right and right to left), repeat
    this procedure.
</p>
<p>
    For example:
</p>
<pre>195 (initial number) + 591 (reverse of initial number) = 786

786 + 687 = 1473

1473 + 3741 = 5214

5214 + 4125 = 9339 (palindrome)</pre>
<p>
    In this particular case the palindrome 9339 appeared after the
    4th addition. This method leads to palindromes in a few step for
    almost all of the integers. But there are interesting exceptions.
    196 is the first number for which no palindrome has been found.
    It is not proven though, that there is no such a palindrome.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is one test case. Each test case will contain
    an integer n &lt;  10,000. Assume each test case will always have an answer
    and that it is computable with less than 100 iterations (additions).
</p>

<h3>Output sample:</h3>

<p>
    For each line of input, generate a line of output which is the number
    of iterations (additions) to compute the palindrome and the
    resulting palindrome. (they should be on one line and separated
    by a single space character).
</p>
<p>
    For example:
</p>
<pre>4 9339</pre>