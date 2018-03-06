<h2>Simple or trump</h2>

<h3>Challenge Description:</h3>

<p>
    First playing cards were invented in Eastern Asia and then spread all over the world taking different forms and
    appearance. In India, playing cards were round, and they were called Ganjifa. In medieval Japan, there was a
    popular Uta-garuta game, in which shell mussels were used instead of playing cards. <br>
    In our game, we use playing cards that are more familiar nowadays. The rules are also simple: an ace
    beats a deuce (2) unless it is a trump deuce.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case which contains two playing cards and a
    trump suit. Cards and a trump suite are separated by a pipeline (|). The card deck includes thirteen ranks
    (from a deuce to an ace) of each of the four suits: clubs (&#x2663;), diamonds (&#x2666;), hearts (&#x2665;), and spades (&#x2660;). There
    are no Jokers.
</p>

<pre class="description-input-output">AD 2H | H
KD KH | C
JH 10S | C</pre>

<h3>Output sample:</h3>

<p>
    Your task is to print a card that wins. If there is no trump card, then the higher card wins. If the cards are
    equal, then print both cards.
</p>

<pre class="description-input-output">2H
KD KH
JH</pre>

<h3>Constraints:</h3>
<ol>
<li>The card deck includes ranks from a deuce (2) to an ace, no Jokers.</li>
<li>If the cards are equal, then print both cards.</li>
<li>The number of test cases is 40.</li>
</ol>