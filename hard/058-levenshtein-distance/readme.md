<h2>Levenshtein Distance</h2>

<h3>Challenge Description:</h3>

<p>
    Two words are friends if they have a Levenshtein distance of 1
    (For details see <a href=" http://en.wikipedia.org/wiki/Levenshtein_distance">Levenshtein distance</a>).
    That is, you can add, remove, or substitute exactly one letter in word X to create word Y. A word&#x2019;s social network
    consists of all of its friends, plus all of their friends, and all of their friends&#x2019; friends, and so on. Write a
    program to tell us how big the social network for the given word is, using our word list.
</p>

<h3>Input sample:</h3>
<p>
    The first argument will be a path to a filename, containing words, and the word list to search in. The first N
    lines of the file will contain test cases, they will be terminated by string &apos;END OF INPUT&apos;. After that there will
    be a list of words one per line. E.g

</p>
<pre class="description-input-output">recursiveness
elastic
macrographies
END OF INPUT
aa
aahed
aahs
aalii
...
...
zymoses
zymosimeters</pre>

<h3>Output sample:</h3>

<p>
    For each test case print out how big the social network for the word is. In sample the social network for the word
    &apos;elastic&apos; is 3 and for the word &apos;recursiveness&apos; is 1. E.g.
</p>
<pre class="description-input-output">1
3
1</pre>
Constraints:
<br>
Number of test cases N in range(15, 30)
<br>
The word list always will be the same and it&apos;s length will be around 10000 words
<br>
<br>