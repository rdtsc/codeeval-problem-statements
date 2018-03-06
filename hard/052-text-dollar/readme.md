<h2>Text Dollar</h2>

<h3>Challenge Description:</h3>
<p>
    Credits: This challenge has been authored by Terence Rudkin
<br>
<br>
    You are given a positive integer number. This represents the sales made that day in your department store.
    The payables department however, needs this printed out in english. NOTE: The correct spelling of 40 is Forty.
    (NOT Fourty)
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.The input file contains several lines.
    Each line is one test case. Each line contains a positive integer. E.g.
</p>
<pre>3
10
21
466
1234</pre>

<h3>Output sample:</h3>

<p>
    For each set of input produce a single line of output which is the english textual representation of that integer.
    The output should be unspaced and in Camelcase. Always assume plural quantities.
    You can also assume that the numbers are &lt; 1000000000 (1 billion). In case of ambiguities e.g.
    2200 could be TwoThousandTwoHundredDollars or TwentyTwoHundredDollars, always choose the representation with the
    larger base i.e. TwoThousandTwoHundredDollars. For the examples shown above, the answer would be:
</p>

<pre>ThreeDollars
TenDollars
TwentyOneDollars
FourHundredSixtySixDollars
OneThousandTwoHundredThirtyFourDollars</pre>