<h2>Glue Shredded Pieces</h2>

<h3>Challenge Description:</h3>

<p>
    Imagine that you are taking part in the investigation of a criminal organization. Having determined its location,
    you came there and found out that the criminals had recently left that place. But it is not a dead end, because
    there are lots of shredded documents in the room. On investigating these documents, you came to conclusion that the
    criminals had not been very careful. Firstly, the papers are shredded horizontally, and you can read some pieces of
    text. Secondly, there are many copies of the same documents, and the pieces of text overlap each other.
</p>
<p>
    For example, you can put pieces together and get the original text:
</p>
<pre class="description-input-output">evil pl
 vil pla
  il plan</pre>
<p>
    The answer is &#x2018;evil plan&#x2019;.
</p>
<p>
    Your task is to print out the original text. Due to repetitions in the text, you will sometimes get identical
    pieces.
</p>

<h3>Input sample:</h3>

<p>
    Your program should accept a path to a file as its first argument. Each line in the file is one test case with the
    pieces of shredded text separated by a pipe. Each test case starts and finishes with symbol &apos;|&apos;.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">|deEva|lan t|to ha|evil |ankin|il-ev|o hac| to h|vil p|an to|The e|CodeE| evil|plan |hack |Eval |ack C|l ran|king.|l-evi|evil-|-evil|l pla|il pl| hack|al ra|vil-e|odeEv|he ev|n to |ck Co|eEval|nking| rank| Code|e evi|ranki|k Cod| plan|val r|</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the original text for each test case.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">The evil-evil plan to hack CodeEval ranking.</pre>

<h3>Constraints:</h3>
<ol>
<li>
        For the text with the length t shredded into pieces with the length n, there are t&#xA0;-&#xA0;(n&#xA0;-&#xA0;1)
        pieces of text in the input file. Each piece of text is shifted by one character. For example, the word
        &#x2018;secret&#x2019; and n&#xA0;=&#xA0;4:

<pre class="description-input-output">secr
 ecre
  cret</pre>
</li>
<li>There is only one correct answer for each test case.</li>
<li>The minimum number of pieces is 125, the maximum number is 975.</li>
<li>The minimum length of a piece of text is 8, the maximum length is 28.</li>
<li>The number of test cases is 20.</li>
</ol>