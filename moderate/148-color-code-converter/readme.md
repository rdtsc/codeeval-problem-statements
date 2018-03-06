<h2>Color Code Converter</h2>

<h3>Challenge Description:</h3>
<p>
    Your task is to write a program which converts different types of color codes, such as CMYK, Hex, HSL, HSV, and RGB.
    The converter should accept codes formatted as follows:
</p>
<pre>HSL: &quot;HSL(D,P,P)&quot;
HSV: &quot;HSV(D,P,P)&quot;
CMYK: &quot;(F,F,F,F)&quot;
Hex: &quot;#000000&quot;</pre>
<p>
    Where:
</p>
<ul>
<li>&apos;D&apos; is in range [0, 359] degrees,</li>
<li>&apos;P&apos; is in range [0, 100] percent,</li>
<li>&apos;F&apos; is a float, rounded to a second digit after dot in range [0.00, 1.00],</li>

</ul>
<p>
    Hex is in range [#000000, #ffffff]
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a file as its first argument. Each line of the file contains a color code.
</p>
<p>
    For example:
</p>
<br>
<pre class="description-input-output">(0.56,0.94,0.21,0.02)
HSL(359,0,0)
HSV(276,33,7)
#cfa9c4</pre>

<h3>Output sample:</h3>

<p>
    For each line of input, determine the color code, convert it to RGB, and print out the result. You must round all
    floating-point numbers, if any, to integers.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">RGB(110,15,197)
RGB(0,0,0)
RGB(15,12,18)
RGB(207,169,196)</pre>