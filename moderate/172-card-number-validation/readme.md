<h2>Card number validation</h2>

<h3>Challenge Description:</h3>

<p>
    To check whether a bank card number is valid or it is it just a set of random numbers, <a href="http://en.wikipedia.org/wiki/Luhn_algorithm">Luhn formula</a> is used.
</p>
<p>
    The formula verifies a number against its included check digit, which is usually appended to a partial account
    number to generate the full account number. This account number must pass the following test:
</p>
<ol>
<li>From the rightmost digit, which is the check digit, moving left, double the value of every second digit;
        if the product of this doubling operation is greater than 9 (for example, 7&#xD7;2=14), then sum the digits
        of the products (for example, 12:1+2=3, 14:1+4=5).
</li>
<li>Take the sum of all the digits.</li>
<li>If the total modulo 10 is equal to 0 (if the total ends in zero) then, according to the Luhn formula,
        the number is valid; otherwise, it is not valid.
</li>
</ol>
<p>
    Examples of formula calculation and result checking:
</p>
<p>
    Checking number <strong>1556 9144 6285 339</strong>
</p>
<pre>1   <u>5</u>   5   <u>6</u>   9   <u>1</u>   4   <u>4</u>   6   <u>2</u>   8   <u>5</u>   3   <u>3</u>   9
1   10  5   12  9   2   4   8   6   4   8   10  3   6   9
1 + 1 + 5 + 3 + 9 + 2 + 4 + 8 + 6 + 4 + 8 + 1 + 3 + 6 + 9 = 70
</pre>
<br>
<p>
    70 mod 10 = 0, card number is valid
</p>
<p>
    Checking number <strong>6363 1811 2857 7650</strong>
</p>
<pre><u>6</u>   3   <u>6</u>   3   <u>1</u>   8   <u>1</u>   1   <u>2</u>   8   <u>5</u>   7   <u>7</u>   6   <u>5</u>   0
12  3   12  3   2   8   2   1   4   8   10  7   14  6   10  0
3 + 3 + 3 + 3 + 2 + 8 + 2 + 1 + 4 + 8 + 1 + 7 + 5 + 6 + 1 + 0 = 57
</pre>
<br>
<p>
    57 mod 10 = 7 &lt;&gt; 0, card number is not valid
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains bank card numbers, one per line. For better readability, numbers are split into groups of 4 digits separated by spaces.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">6011 5940 0319 9511
5537 0213 6797 6815
5574 8363 8022 9735
3044 8507 9391 30
6370 1675 9034 6211 774</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the results of bank card numbers validation, one per line. If the number is correct &#x2013; print 1, otherwise &#x2013; print 0.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">0
1
0
0
1</pre>

<h3>Constraints:</h3>
<ol>
<li>Bank card numbers can be from 12 to 19 digits length.</li>
<li>Numbers are split into groups of 4 digits separated by spaces, spaces should be ignored.</li>
<li>Number of test cases is 100.</li>
</ol>