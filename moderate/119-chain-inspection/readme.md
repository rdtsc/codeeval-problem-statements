<h2>Chain Inspection</h2>

<h3>Challenge Description:</h3>

<p>
    We use special generator to produce chains of elements. Don&apos;t ask why we need them,
    we&apos;re not sure that somebody knows the answer for this question.
    A chain is represented by a string of name-address pairs.
    So the first element is the name of a pair and the second one (address) is pointing to the name of a next pair. E.g.
</p>
<pre>BEGIN-3;4-2;3-4;2-END # GOOD
77-END;BEGIN-8;8-11;11-77 # GOOD
</pre>
<p>
    In examples above we can pass trough the chains from the &apos;BEGIN&apos; to the &apos;END&apos; without missing any single pair.
    In the first case we moved from &apos;BEGIN&apos; to 3, from 3 to 4, from 4 to 2, from 2 to &apos;END&apos;.
    In the second case we moved from &apos;BEGIN&apos; to 8, from 8 to 11, from 11 to 77, from 77 to &apos;END&apos;.
<br>
<br>
    Our generator was producing only good chains, but something went wrong and now it
    generates random chains and we are not sure if it&apos;s a good chain or a bad one. E.g.
</p>
<pre>BEGIN-3;4-3;3-4;2-END # BAD
77-END;BEGIN-8;8-77;11-11 # BAD
</pre>
<p>
    In the first case the &apos;END&apos; is unreachable because we have a loop between 3 and 4.
<br>
    In the second case we can reach the &apos;END&apos; but we missed one pair (11-11).
<br>
    We know that for a BAD chain the generator first produces a GOOD chain but after that
    it may replace existing address in some pairs with an address from another pair.
    It never replaces an address in a pair to an addresses which isn&apos;t present in original chain.
<br>
    You can help us by writing a program that investigates the input and finds GOOD and BAD chains.
</p>
<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each string in this file is a chain. The pairs are separating by semicolon,
    the names and the address are separating by dash. E.g.
</p>
<pre class="description-input-output">4-2;BEGIN-3;3-4;2-END
4-2;BEGIN-3;3-4;2-3</pre>

<h3>Output sample:</h3>

<p>
    For each line of input print out the chain status. E.g.
</p>
<pre class="description-input-output">GOOD
BAD</pre>
<p>
    Constraints:
<br>
    The number of pairs in a chain is in range [1, 500]
<br>
    The addresses are integers in range [2, 10000]

</p>