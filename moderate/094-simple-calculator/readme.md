<h2>Simple Calculator</h2>

<h3>Challenge Description:</h3>
<p>
    The goal of this challenge is to create a simple calculator.
<br>
    The following operations should be supported with
    their order (operator precedence):
<br>
</p>

<pre>1   <b>()</b>       Brackets
2   <b>-</b>        Unary minus
3   <b>^</b>        Exponent
4   <b>*</b>, <b>/</b>     Multiply, Divide (left-to-right precedence)
5   <b>+</b>, <b>-</b>     Add, Subtract (left-to-right precedence)
</pre>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    The input file contains several lines. Each line is one test case.
    Each line contains mathematical expression. E.g.
</p>
<pre>250*14.3
3^6 / 117
(2.16 - 48.34)^-1
(59 - 15 + 3*6)/21</pre>

<h3>Output sample:</h3>

<p>
    For each set of input produce a single line of output which is the
    result of calculation.
</p>

<pre>3575
6.23077
&#x2212;0.02165
2.95238</pre>

<p>
    Note: Don&apos;t use any kind of <b>eval</b> function.
</p>

<p>
<b>Constraints:</b>
<br>
    Each number in input expression is greater than -20,000 and less than 20,000.
<br>
    Each output number is greater than -20,000 and less than 20,000.
<br>
    If output number is a float number it should be rounded to the 5th digit after the dot.
<br>
    E.g 14.132646 gets 14.13265, 14.132644 gets 14.13264, 14.132645 gets 14.13265.
<br>
<br>
    If output number has less than 5 digits after the dot you don&apos;t need to add zeros.
<br>
    E.g. you need to print 16.34 (and not 16.34000) in case the answer is 16.34.
<br>
    And you need to print 16 (and not 16.00000) in case the answer is 16.
</p>