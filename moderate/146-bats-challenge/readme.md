<h2>Bats Challenge</h2>

<h3>Challenge Description:</h3>

<p>
    There is a wire between two buildings outside of your window. Bats love to hang there, but they never hang closer
    than &quot;d&quot; centimeters from each other. They also don&apos;t hang closer than 6 centimeters from any of the buildings.
</p>
<p>
    Your task is to determine the maximum number of additional bats that can fit on the wire assuming they have a zero width.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a file as its first argument. Each line of input contains three space separated integers:
    the length of the wire &quot;l&quot;, distance &quot;d&quot;, and number of bats &quot;n&quot; that are already hanging on the wire.
</p>
<p>
    The &quot;n&quot; number of bats is located in any order. All numbers are integers. You can assume that the bats that are
    already hanging on the wire are at least 6 cm from the buildings and at least &quot;d&quot; centimeters apart from each other.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">22 2 2 9 11
33 5 0
16 3 2 6 10
835 125 1 113
47 5 0</pre>

<h3>Output sample:</h3>
<p>
    For each line of input, print out one integer to determine the maximum number of additional bats that can possibly
    hang on the wire.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">3
5
0
5
8</pre>