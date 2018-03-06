<h2>Ugly Numbers</h2>

<h3>Challenge Description:</h3>

<span class="p-like">
    Credits: This challenge has appeared in a google competition before.
</span>
<p>
    Once upon a time in a strange situation, people called a number ugly
    if it was divisible by any of the one-digit primes (2, 3, 5 or 7).
    Thus, 14 is ugly, but 13 is fine. 39 is ugly, but 121 is not.
    Note that 0 is ugly. Also note that negative numbers can also be ugly:
    -14 and -39 are examples of such numbers.
</p>
<p>
    One day on your free time, you are gazing at a string of digits,
    something like:
</p>
<pre>123456</pre>
<p>
    You are amused by how many possibilities there are if you are allowed
    to insert plus or minus signs between the digits. For example you
    can make:
<br>

</p>
<pre>1 + 234 - 5 + 6 = 236</pre>
<p>
    which is ugly. Or

</p>
<pre>123 + 4 - 56 = 71</pre>
<p>
    which is not ugly.
<br>
<br>
    It is easy to count the number of different ways you can play with the
    digits: Between each two adjacent digits you may choose put a plus sign,
    a minus sign, or nothing. Therefore, if you start with D digits there
    are 3^(D-1) expressions you can make. Note that it is fine to have
    leading zeros for a number. If the string is &apos;01023&apos;, then &apos;01023&apos;,
    &apos;0+1-02+3&apos; and &apos;01-023&apos; are legal expressions.
<br>
<br>
    Your task is simple: Among the 3^(D-1) expressions, count how many of
    them evaluate to an ugly number.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is one test case. Each test case will be a single
    line containing a non-empty string of decimal digits. The string in
    each test case will be non-empty and will contain only characters &apos;0&apos;
    through &apos;9&apos;. Each string is no more than 13 characters long. E.g.
</p>
<pre>1
9
011
12345</pre>

<h3>Output sample:</h3>

<p>
    Print out the number of expressions that evaluate to an ugly number for
    each test case, each one on a new line. E.g.
</p>
<pre>0
1
6
64</pre>