<h2>Digit statistics</h2>

<h3>Challenge Description:</h3>
<p>
    Given the numbers &quot;a&quot; and &quot;n&quot; find out how many times each digit from zero to nine
    is the last digit of the number in a sequence [ a, a<sup>2</sup>, a<sup>3</sup>, ... a<sup>n-1</sup>, a<sup>n</sup> ]
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line of input contains two space separated integers &quot;a&quot; and &quot;n&quot; E.g:
<br>
</p>
<pre class="description-input-output">2 5</pre>

<h3>Output sample:</h3>

<p>
    For each line of input print out how many times the digits zero, one, two ... nine
    occur as the last digit of numbers in the sequence E.g:
</p>

<pre class="description-input-output">0: 0, 1: 0, 2: 2, 3: 0, 4: 1, 5: 0, 6: 1, 7: 0, 8: 1, 9: 0</pre>
<p>
    In this example, the sequence consists of numbers 2, 4, 8, 16 and 32.
    Among the last digits, the digit two occurs twice, and each of the digits four,
    six and eight occurs once.
</p>
<p>
<b>Constraints:</b>
<br>
    1 &#x2264; n &#x2264; 1 000 000 000 000,
<br>
    2 &#x2264; a &#x2264; 9
</p>