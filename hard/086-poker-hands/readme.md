<h2>Poker hands</h2>

<h3>Challenge Description:</h3>
<p>
In the card game poker, a hand consists of five cards and are ranked, from lowest to highest, in the following way:
</p>
<pre>High Card: Highest value card.
One Pair: Two cards of the same value.
Two Pairs: Two different pairs.
Three of a Kind: Three cards of the same value.
Straight: All cards are consecutive values.
Flush: All cards of the same suit.
Full House: Three of a kind and a pair.
Four of a Kind: Four cards of the same value.
Straight Flush: All cards are consecutive values of same suit.
Royal Flush: Ten, Jack, Queen, King, Ace, in same suit.
The cards are valued in the order:
2, 3, 4, 5, 6, 7, 8, 9, Ten, Jack, Queen, King, Ace.
</pre>
<p>
If two players have the same ranked hands then the rank made up of the highest value wins; for example, a pair of
    eights beats a pair of fives. But if two ranks tie, for example, both players have a pair of queens, then highest
    cards in each hand are compared; if the highest cards tie then the next highest cards are compared, and so on.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line in this file contains 2 hands
    (left and right). Cards and hands are separated by space. E.g.
</p>

<pre>6D 7H AH 7S QC 6H 2D TD JD AS
JH 5D 7H TC JS JD JC TS 5S 7S
2H 8C AD TH 6H QD KD 9H 6S 6C
JS JH 4H 2C 9H QH KC 9D 4D 3S
TC 7H KH 4H JC 7D 9S 3H QS 7S</pre>

<h3>Output sample:</h3>

<p>
    Print out the name of the winning hand or &quot;none&quot; in case the hands are equal. E.g.
</p>

<pre>left
none
right
left
right</pre>