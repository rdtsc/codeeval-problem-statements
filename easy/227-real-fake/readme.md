<h2>Real fake</h2>

<h3>Challenge Description:</h3>

<p>
    The police caught a swindler with a big pile of credit cards. Some of them are stolen and some are fake. It would
    take too much time to determine which ones are real and which are fake, so you need to write a program to check
    credit cards. <br>
    To determine which credit cards are real, double every third number starting from the first one, add them
    together, and then add them to those figures that were not doubled. If the total sum of all numbers is divisible
    by 10 without remainder, then this credit card is real. <br>

</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each row includes a test case with a credit card number that you need to
    check.
</p>

<pre class="description-input-output">9999 9999 9999 9999
9999 9999 9999 9993</pre>

<h3>Output sample:</h3>

<p>
    If a credit card is fake &#x2013; print Fake, if it&#x2019;s real &#x2013; print Real.
</p>

<pre class="description-input-output">Fake
Real</pre>

<h3>Constraints:</h3>
<ol>
<li>The credit card number is 16 digits in length.</li>
<li>The number of test cases is 40.</li>
</ol>