<h2>Play with DNA</h2>

<h3>Challenge Description:</h3>
<p>
    This challenge is related to bioinformatics. To help in a DNA research, you have to write an algorithm that finds
    all the occurrences of a DNA segment in a given DNA string. But, it would be too easy for you. So, write an
    algorithm with the maximum N number of allowed mismatches. By mismatch we mean the minimum of the total number
    of substitutions, deletions, and insertions that must be performed on a DNA slice to completely match a given
    segment. You need to compare the DNA slices with the same length as a given pattern (for example, the segments
    &apos;AGTTATC&apos; -&gt; &apos;AGTATGC&apos; have only 2 mismatches).
</p>

<p>
    For the DNA string &apos;CGCCCGAATCCAG&apos; and the segment &apos;CCC&apos;, the first match with the maximum 1 allowed mismatch
    is &apos;CGC&apos;, the second one is &apos;GCC&apos;, the third one is &apos;CCC&apos;, and so on.
</p>

<pre>CCC -&gt; CGC # One mismatch
CCC -&gt; GCC # One mismatch
CCC -&gt; CCC # 0 mismatch</pre>

<p>
    For the given segment &apos;CCC&apos;, the DNA string &apos;CGCCCGAATCCAG&apos;, and the maximum allowed mismatch &apos;1&apos;, the list of the
    matches is &apos;CGC GCC CCC CCG TCC CCA&apos;.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument. Each line in the file contains a segment
    of DNA, the maximum number of allowed mismatches N, and a DNA string separated by a single space.
</p>

<pre class="description-input-output">CCC 1 CGCCCGAATCCAG
GCGAG 2 CCACGGCCTATGTATTTGCAAGGATCTGGGCCAGCTAAATCAGCACCCCTGGAACGGCAAGGTTCATTTTGTTGCGCGCATAG
CGGCGCC 1 ACCCCCGCAGCCATATGTCCCCAGCTATTTAATGAGGGCCCCGAACACGGGGAGTCTTACACGATCTGCCCTGGAATCGC</pre>

<h3>Output sample:</h3>

<p>
    Print out all the occurrences of a segment S in a DNA string in the order from the best match (separated by a
    single space) taking into account the number of allowed mismatches. In case of several segments with the equal
    number of matches, print them in alphabetical order. If there is no such a case, print out &apos;No match&apos;.
</p>

<pre class="description-input-output">CCC CCA CCG CGC GCC TCC
GCAAG GCAAG GCCAG GCGCG GCGCA GCTAA
No match</pre>

<h3>Constraints:</h3>

<ol>
<li>The length of a DNA string is in a range from 100 to 300.</li>
<li>N is in a range from 0 to 40.</li>
<li>The length of a segment S is in a range from 3 to 50.</li>
</ol>