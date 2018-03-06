<h2>DNA Alignment</h2>

<h3>Challenge Description:</h3>

<p>
    In this challenge, you have to deal with biological code: DNA sequences. DNA sequences are made up
    of four bases: A, C, T, and G. New DNA sequences are formed by copying the existing ones.
    However, sometimes, this process is accompanied by errors: one base may be replaced with another;
    fragments may be deleted or inserted.
</p>

<p>
    Your task is to compare two related sequences that parted from one another million years ago and
    changed during this time.
</p>
<p>
    To do this, bioinformaticians use sequence alignment: they present them in the form of a matrix,
    indicating gaps with a minus sign (-), so that the maximum number of identical bases (symbols) are
    under each other.
</p>
<p>
    For example, for <code>GAAAAAAT</code> and <code>GAAT</code> sequences, one of the possible alignments
    will be the following:
</p><pre>GAAAAAAT
G--A&#x2013;A&#x2013;T
</pre>

<p>
    Scoring systems are used to assess the alignment. These are rules, according to which the alignment receives:
</p>
<ul>
<li>positive points&#xA0;&#x2014; for each match (when the symbols in two lines match)</li>
<li>negative points&#xA0;&#x2014; for mismatch (different symbols in two lines)</li>
<li>negative points&#xA0;&#x2014; for indel (an insertion or deletion, i.e. a gap in one of the lines)</li>
</ul>

<p>
    In some scoring systems, indel start  &#x201C;costs&#x201C; more than indel extension, because one big gap is biologically
    more likely to appear than two or more smaller gaps.
</p>
<p>
    In this challenge, we use the following scoring system:
</p>
<pre>Match: +3
Mismatch: -3
Indel start: -8
Indel extension: -1
</pre>

<p>
    Thus, the score for the above sequence is calculated as follows:
</p>
<pre>  G  A  A  A  A  A  A  T
  G  -  -  A  &#x2013;  A  &#x2013;  T
 +3 -8 -1 +3 -8 +3 -8 +3 = -13
</pre>

<p>
    Another version of the same sequences alignment:
</p>

<pre>  G  A  A  A  A  A  A  T
  G  A  A  -  -  -  -  T
 +3 +3 +3 -8 -1 -1 -1 +3 = 1
</pre>
<p>
    For most pairs of sequences, there is more than one optimal alignment. Your task is to find the highest
    possible score of such alignments.
</p>

<h3>Input sample:</h3>

<p>
    Your program should accept a path to a file as its first argument. Each line of the file is a pair of DNA
    sequences separated by vertical bar (|).
</p>

<pre class="description-input-output">GAAAAAAT | GAAT
GCATGCT | GATTACA</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the score of the best possible alignment taking into account the above scoring system.
</p>

<pre class="description-input-output">1
-3</pre>

<h3>Constraints:</h3>
<ol>
<li>The length of each sequence does not exceed 400 symbols.</li>
</ol>