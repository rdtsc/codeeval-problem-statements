<h2>Roller Coaster</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a piece of text. Your job is to write a program that sets the case of text characters according to
    the following rules:
</p>
<ol>
<li>The first letter of the line should be in uppercase.</li>
<li>The next letter should be in lowercase.</li>
<li>The next letter should be in uppercase, and so on.</li>
<li>Any characters, except for the letters, are ignored during determination of letter case.</li>
</ol>

<h3>Input sample:</h3>

<p>
    The first argument will be a path to a filename containing sentences, one per line. You can assume that all
    characters are from the English language.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">To be, or not to be: that is the question.
Whether &apos;tis nobler in the mind to suffer.
The slings and arrows of outrageous fortune.
Or to take arms against a sea of troubles.
And by opposing end them, to die: to sleep.</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the RoLlErCoAsTeR case version of the string.</p>
<p>
    For example:
</p>

<pre class="description-input-output">To Be, Or NoT tO bE: tHaT iS tHe QuEsTiOn.
WhEtHeR &apos;tIs NoBlEr In ThE mInD tO sUfFeR.
ThE sLiNgS aNd ArRoWs Of OuTrAgEoUs FoRtUnE.
Or To TaKe ArMs AgAiNsT a SeA oF tRoUbLeS.
AnD bY oPpOsInG eNd ThEm, To DiE: tO sLeEp.</pre>

<h3>Constraints:</h3>
<p>
    The length of each piece of text does not exceed 1000 characters.
</p>