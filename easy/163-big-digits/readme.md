<h2>Big Digits</h2>

<h3>Challenge Description:</h3>
<p>
    In this challenge you&apos;re presented with a situation in which you need to output big symbols on devices which only
    support ASCII characters and single, fixed-width fonts. To do this you&apos;re going to use pseudo-graphics to &#x2018;draw&#x2019;
    these big symbols.
</p>
<p>
    Here is an example of the font with digits from 0 to 9:
</p>

<pre class="description-input-output">-**----*--***--***---*---****--**--****--**---**--
*--*--**-----*----*-*--*-*----*-------*-*--*-*--*-
*--*---*---**---**--****-***--***----*---**---***-
*--*---*--*-------*----*----*-*--*--*---*--*----*-
-**---***-****-***-----*-***---**---*----**---**--
--------------------------------------------------</pre>

<p>Each pixel is marked either with asterisk &#x2018;*&#x2019; or with minus &#x2018;-&#x2019;. Size of a digit is 5&#xD7;6 pixels.</p>

<p>Your task is to write a program, which outputs the numbers given to you with the font as in the example.</p>

<h3>Input sample:</h3>

<p>The first argument is a file that contains the lines with digits sequences you need to magnify. E.g.:</p>

<pre class="description-input-output">3.1415926
1.41421356
01-01-1970
2.7182818284
4 8 15 16 23 42</pre>

<h3>Output sample:</h3>

<p>Print to stdout the magnified digits:</p>

<pre class="description-input-output">***----*---*-----*--****--**--***---**--
---*--**--*--*--**--*----*--*----*-*----
-**----*--****---*--***---***--**--***--
---*---*-----*---*-----*----*-*----*--*-
***---***----*--***-***---**--****--**--
----------------------------------------
--*---*-----*---*---***----*--***--****--**--
-**--*--*--**--*--*----*--**-----*-*----*----
--*--****---*--****--**----*---**--***--***--
--*-----*---*-----*-*------*-----*----*-*--*-
-***----*--***----*-****--***-***--***---**--
---------------------------------------------
-**----*---**----*----*---**--****--**--
*--*--**--*--*--**---**--*--*----*-*--*-
*--*---*--*--*---*----*---***---*--*--*-
*--*---*--*--*---*----*-----*--*---*--*-
-**---***--**---***--***--**---*----**--
----------------------------------------
***--****---*---**--***---**----*---**--***---**---*---
---*----*--**--*--*----*-*--*--**--*--*----*-*--*-*--*-
-**----*----*---**---**---**----*---**---**---**--****-
*-----*-----*--*--*-*----*--*---*--*--*-*----*--*----*-
****--*----***--**--****--**---***--**--****--**-----*-
-------------------------------------------------------
-*----**----*--****---*---**--***--***---*---***--
*--*-*--*--**--*-----**--*-------*----*-*--*----*-
****--**----*--***----*--***---**---**--****--**--
---*-*--*---*-----*---*--*--*-*-------*----*-*----
---*--**---***-***---***--**--****-***-----*-****-
--------------------------------------------------</pre>

<h3>Constraints:</h3>
<ol>
<li>Input lines are up to 16 symbols long.</li>
<li>Input can contain some other symbols, which should be ignored (i.e. points, hyphens, spaces);
        only numbers must be printed out.</li>
</ol>