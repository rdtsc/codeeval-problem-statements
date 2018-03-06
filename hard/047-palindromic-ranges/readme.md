<h2>Palindromic Ranges</h2>

<h3>Challenge Description:</h3>
<p>
    A positive integer is a palindrome if its decimal representation (without leading zeros) is a palindromic string
    (a string that reads the same forwards and backwards). For example, the numbers 5, 77, 363, 4884, 11111, 12121
    and 349943 are palindromes.
<br>
<br>
    A range of integers is interesting if it contains an even number of palindromes. The range [L, R], with L &lt;= R,
    is defined as the sequence of integers from L to R (inclusive): (L, L+1, L+2, ..., R-1, R).
    L and R are the range&apos;s first and last numbers.
<br>
<br>
    The range [L1,R1] is a subrange of [L,R] if L &lt;= L1 &lt;= R1 &lt;= R. Your job is to determine how
    many interesting subranges of [L,R] there are.

</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line in this file is one test case.
    Each test case will contain two positive integers, L and R (in that order), separated by a space. eg.
<br>
</p>

<pre>1 2
1 7
87 88</pre>

<h3>Output sample:</h3>

<p>
    For each line of input, print out the number of interesting subranges of [L,R] eg.
<br>
</p>

<pre>1
12
1</pre>
<p>
    For the curious: In the third example, the subranges are: [87](0 palindromes),
    [87,88](1 palindrome),[88](1 palindrome). Hence the number of interesting palindromic ranges is 1
</p>