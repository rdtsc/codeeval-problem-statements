<h2>Cash Register</h2>

<h3>Challenge Description:</h3>

<p>
    The goal of this challenge is to design a cash register program.
    You will be given two float numbers. The first is the purchase price (PP) of the item.
    The second is the cash (CH) given by the customer.
    Your register currently has the following bills/coins within it:
</p>

<pre>&apos;PENNY&apos;: .01,
&apos;NICKEL&apos;: .05,
&apos;DIME&apos;: .10,
&apos;QUARTER&apos;: .25,
&apos;HALF DOLLAR&apos;: .50,
&apos;ONE&apos;: 1.00,
&apos;TWO&apos;: 2.00,
&apos;FIVE&apos;: 5.00,
&apos;TEN&apos;: 10.00,
&apos;TWENTY&apos;: 20.00,
&apos;FIFTY&apos;: 50.00,
&apos;ONE HUNDRED&apos;: 100.00</pre>

<p>
    The aim of the program is to calculate the change that has to be returned to the customer.
</p><h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    The input file contains several lines. Each line is one test case.
    Each line contains two numbers which are separated by a semicolon.
    The first is the Purchase price (PP) and the second is the cash(CH) given by the customer. eg.
</p>
<pre class="description-input-output">15.94;16.00
17;16
35;35
45;50</pre>

<h3>Output sample:</h3>

<p>
    For each set of input produce a single line of output which is the change to be returned to the customer.
    In case the CH &lt; PP, print out ERROR. If CH == PP, print out ZERO.
    For all other cases print the amount that needs to be returned, in terms of the currency values provided.
    The output should be sorted in highest-to-lowest order (DIME,NICKEL,PENNY). eg.
</p>

<pre class="description-input-output">NICKEL,PENNY
ERROR
ZERO
FIVE</pre>