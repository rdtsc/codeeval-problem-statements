<h2>The Cubes</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a scheme of the labyrinth in the form of a cube with N levels of N&#xA0;&#xD7;&#xA0;N elements.
    The walls are marked with asterisks &#x2018;*&#x2019;, and the floor &#x2014; with spaces. The floor of different levels, except the lowest
    one, can have holes marked with &#x2018;o&#x2019;. The holes allow you to move to a lower level (if it is on the floor of
    the current level), to move to a higher level (if it is on the floor of the higher level), or to move over the hole
    on the current level.
</p>
<p>
    Below is the example of a labyrinth scheme for N=5:
</p>
<pre>Level 1:

\*\*\*\*\*
\*   \*
\* \*\*\*
\*   \*
\*\* \*\*



Level 2:

\*\*\*\*\*
\*  o\*
\*o\* \*
\* \* \*
\*\*\*\*\*



Level 3:

\*\*\*\*\*
\*   \*
\* \* \*
\*o\* \*
\*\*\*\*\*



Level 4:

\*\*\*\*\*
\* o \*
\*\*\* \*
\*   \*
\*\*\*\*\*



Level 5:

\*\* \*\*
\*o  \*
\*\*\*o\*
\*o  \*
\*\*\*\*\*
</pre>

<p>
    Find the number of steps in the shortest way from the entrance on the first floor to the exit on the last floor,
    including entrance and exit. Moving between levels is one step.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains test cases, one test case per line. Each test case contains N number
    (the length of the cube edge) and scheme of the labyrinth, separated by semicolon. The scheme of the
    labyrinth is serialized: all elements are listed sequentially, starting from the top left corner of the first level.
</p>
<p>
    For example (the first test case represent the example provided above in challenge description):
</p>

<pre class="description-input-output">5;******   ** ****   *** ********  o**o* ** * ************   ** * **o* ************ o **** **   ******** ***o  ****o**o  ******
5;****** * ** * **   *** ********o*o** *o**   ************   **o* ** *o************   **** **   ******** *** o ****o**  o******
7;********     ** *** ** * * ** * * **     **** *********** *   ** *** **   *o**o***o**oo   ****************  oo ** * * ** * * ** * * ** *o o****************     ** * ****o* * ** *** **o    ****************     ** *** **     ****** ** o  o**************** *oo ** *** **o  * ** *** **o    *********** ****   * ** * * ** * *o** ***o**     ********</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the minimum number of steps for each test case to get through the labyrinth. If it is impossible
    to pass the labyrinth&#xA0;&#x2014; print&#xA0;0.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">15
0
39</pre>

<h3>Constraints:</h3>
<ol>
<li>Number of test cases is 20.</li>
<li>The length of the cube edge is from 5 to 11.</li>
<li>Moving between levels is 1 step.</li>
<li>There can more than one shortest way.</li>
</ol>
