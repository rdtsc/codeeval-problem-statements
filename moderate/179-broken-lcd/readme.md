<h2>Broken LCD</h2>

<h3>Challenge Description:</h3>

<p>
    You have a 12-digit LCD, each digit consists of 8 segments: 7 segments to display numbers and one segment to display
    a decimal mark:
</p>

<p>
    The number in each digit is displayed by turning segments on or off. It can be represented as a binary 8-bit number,
    each bit of which is a segment, ordered in the following binary representation:
</p>

<p>
    For example, number &#x2018;4.&#x2019; (with the decimal mark turned on) corresponds to the following binary representation:
</p>

<p>
    Some segments of the display are damaged and are always turned off. Your task is to determine whether a given number
    can be displayed on the damaged LCD. You can start displaying the number with the arbitrary digit of the LCD.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a filename. Each line of the file contains binary 8-bit numbers, which represents the state of
    the segments, starting from the most left digit, and the number that you must show on the display. The binary
    numbers are separated by spaces, the number to display is separated by a semicolon.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">10110001 11111000 11111110 11111111 11111111 11111111 11111111 11101101 11111111 01111111 11110010 10100111;84.525784
11111111 11110110 11101111 11110111 10111110 11110110 10111011 10100111 11111100 01100100 11111101 01011110;5.57
11000010 00001111 11111111 10111111 11101011 11110011 01111110 11011111 11111111 11111111 11111001 01101110;857.71284
11111111 01110111 10111011 11001101 11111011 11101010 11110100 01001101 11011111 11111010 10010110 10111111;66.92
11111011 10010001 11111011 11111101 10011111 10111110 01111100 11011101 10111001 11111110 11101111 11110110;188.87</pre>

<p>
    Every binary number represents the state of the segments in one digit. 1 means that a segment is working and can be
    turned on or off, 0 means that a segment is damaged and is always turned off.
</p>

<h3>Output sample:</h3>

<p>
    Print to stdout 1 for each test case if the number can be displayed on a given LCD, or 0 &#x2013; if the number cannot be
    displayed. Print out one number in a line.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">1
1
1
0
0</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of test cases is 100.</li>
<li>The damaged segments are always turned off.</li>
<li>The number can be displayed starting from any digit.</li>
<li>Every number has a decimal mark (if it is an integer, a decimal mark is placed after the last digit).</li>
</ol>