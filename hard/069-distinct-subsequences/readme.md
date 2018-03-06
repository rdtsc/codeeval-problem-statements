<h2>Distinct Subsequences</h2>

<h3>Challenge Description:</h3>
<p>
    A subsequence of a given sequence S consists of S with zero or more elements deleted.
    Formally, a sequence Z = z1z2..zk is a subsequence of X = x1x2...xm, if there exists a strictly increasing
    sequence <i1,i2...ik> of indicies of X such that for all j=1,2,...k we have Xij = Zj. E.g. Z=bcdb is a
    subsequence of X=abcbdab with corresponding index sequence &lt;2,3,5,7&gt;
</i1,i2...ik></p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line in this file contains two
    comma separated strings. The first is the sequence X and the second is the subsequence Z. E.g.
</p>
<pre class="description-input-output">babgbag,bag
rabbbit,rabbit</pre>

<h3>Output sample:</h3>

<p>
    Print out the number of distinct occurrences of Z in X as a subsequence E.g.
</p>

<pre class="description-input-output">5
3</pre>