<h2>Query Board</h2>

<h3>Challenge Description:</h3>

<p>
    There is a board (matrix). Every cell of the board contains one integer,
    which is <b>0</b> initially.
<br>
<br>
    The next operations can be applied to the Query Board:
<br>
<b>SetRow i x</b>: it means that all values in the cells on row &quot;i&quot; have been changed to value &quot;x&quot; after this operation.
<br>
<b>SetCol j x</b>: it means that all values in the cells on column &quot;j&quot; have been changed to value &quot;x&quot; after this operation.
<br>
<b>QueryRow i</b>: it means that you should output the sum of values
    on row &quot;i&quot;.
<br>
<b>QueryCol j</b>: it means that you should output the sum of values on column &quot;j&quot;.
<br>
<br>
    The board&apos;s dimensions are 256x256
<br>
    &quot;i&quot; and &quot;j&quot; are integers from 0 to 255
<br>
    &quot;x&quot; is an integer from 0 to 31
<br>
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains an operation of a query. E.g.
</p>
<pre>SetCol 32 20
SetRow 15 7
SetRow 16 31
QueryCol 32
SetCol 2 14
QueryRow 10
SetCol 14 0
QueryRow 15
SetRow 10 1
QueryCol 2</pre>

<h3>Output sample:</h3>

<p>
    For each <b>query</b>, output the answer of the query. E.g.
</p>

<pre>5118
34
1792
3571</pre>