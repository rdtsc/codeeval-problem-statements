<h2>Lucky tickets</h2>

<h3>Challenge Description:</h3>

<p>
    We can receive a lucky ticket in a public transport. How to reveal whether the ticket is lucky or not? We call a
    ticket lucky if the sum of its digits in the first half equals to the sum of digits in the second half.
    For example, ticket 328940 is a lucky one because 3+2+8=9+4+0. <br>
    Write a program that will count the maximum number of lucky tickets depending on the length of the ticket number.
    In other words, how many lucky combinations can be if a ticket number comprises 4, 6, 8, &#x2026; digits ?
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with an even number that
    indicates the length of the ticket number.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">4
6
8</pre>

<h3>Output sample:</h3>

<p>
    Count and print the maximum possible number of lucky tickets depending on the length of the ticket number.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">670
55252
4816030</pre>

<h3>Constraints:</h3>
<ol>
<li>The length of a ticket number can be from 2 to 100 digits.</li>
<li>Tickets 000000 and 999999 should be also counted.</li>
<li>All the input numbers are even.</li>
<li>The number of test cases is 40.</li>
</ol>