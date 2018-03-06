<h2>Hidden Digits</h2>

<h3>Challenge Description:</h3>
<p>
    In this challenge you&apos;re given a random string containing hidden and visible digits.
    The digits are hidden behind lower case latin letters as follows:
    0 is behind &apos;a&apos;, 1 is behind &apos; b &apos; etc., 9 is behind &apos;j&apos;. Any other symbol in the string means nothing and has to be ignored.
    So the challenge is to find all visible and hidden digits in the string and print them out in order of their appearance.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains a string. You may assume that
    there will be no white spaces inside the string. E.g.
</p>
<pre>abcdefghik
Xa,}A#5N}{xOBwYBHIlH,#W
(ABW&gt;&apos;yy^&apos;M{X-K}q,
6240488</pre>

<h3>Output sample:</h3>

<p>
    For each test case print out all visible and hidden digits in order of their appearance. Print out NONE in case
    there is no digits in the string. E.g.
</p>
<pre>012345678
05
NONE
6240488</pre>