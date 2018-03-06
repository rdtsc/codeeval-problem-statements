<h2>The Major Element</h2>

<h3>Challenge Description:</h3>
<p>
   The major element in a sequence with the length of L is the element which appears in a sequence more than L/2 times.
   The challenge is to find that element in a sequence.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line of the file contains a sequence of integers N separated by comma. E.g.
</p>

<pre class="description-input-output">92,19,19,76,19,21,19,85,19,19,19,94,19,19,22,67,83,19,19,54,59,1,19,19
92,11,30,92,1,11,92,38,92,92,43,92,92,51,92,36,97,92,92,92,43,22,84,92,92
4,79,89,98,48,42,39,79,55,70,21,39,98,16,96,2,10,24,14,47,0,50,95,20,95,48,50,12,42</pre>

<h3>Output sample:</h3>
<p>
     For each sequence print out the major element or print &quot;None&quot; in case there is no such element. E.g.
</p>

<pre class="description-input-output">19
92
None</pre>
<p>
    Constraints:
<br>
    N is in range [0, 100]
<br>
    L is in range [10000, 30000]
<br>
    The number of test cases &lt;= 40
</p>