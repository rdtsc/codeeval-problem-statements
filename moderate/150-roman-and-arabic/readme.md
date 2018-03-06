<h2>Roman and Arabic</h2>

<h3>Challenge Description:</h3>

<p>
This challenge involves calculating the value of &#x201C;aromatic&#x201D; numbers which are a combination of Arabic
digits and Roman numerals.
<br>
An aromatic number is of the form A<sub>1</sub>R<sub>1</sub>A<sub>2</sub>R<sub>2</sub> ... A<sub>n</sub>R<sub>n</sub>,
where each A<sub>i</sub> is an Arabic digit, and each R<sub>i</sub> is a Roman numeral.
Each pair A<sub>i</sub>R<sub>i</sub> contributes a value described below, and by adding or subtracting these values
together we get the value of the entire aromatic number.
<br>
An Arabic digit A can be 0, 1, 2, 3, 4, 5, 6, 7, 8 or 9.
<br>
A Roman numeral R is one of the seven letters I, V, X, L, C, D, or M.
Each Roman numeral has a base value: 1, 5, 10, 50, 100, 500, 1000, respectively.
<br>
The value of a pair AR is A times the base value of R. Normally, you add up the values of the pairs to get the overall value.
However, wherever there are consecutive symbols ARA`R` with R` having a strictly bigger base value than R,
the value of pair AR must be substracted from the total, instead of being added.
<br>
For example, the number 3M1D2C has the value 3 &#xD7; 1000 + 1 &#xD7; 500 + 2 &#xD7; 100 = 3700 and 3X2I4X has the value 3 &#xD7; 10 - 2 &#xD7; 1 + 4 &#xD7; 10 = 68 .
Write a program that calculates the values of aromatic numbers.
<br>
</p>

<h3>Input sample:</h3>
<p>
    The input is a valid aromatic number consisting of between 2 and 20 symbols. Your program should accept as its first argument a path to a filename. E.g.:
</p>
<pre class="description-input-output">3M1D2C
2I3I2X9V1X</pre>

<h3>Output sample:</h3>

<p>
    The output is the decimal value of the given aromatic number.
</p>

<pre class="description-input-output">3700
-16</pre>