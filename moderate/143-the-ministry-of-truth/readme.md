<h2>The Ministry of Truth</h2>

<h3>Challenge Description:</h3>
<p>
    It&apos;s 1984, and you are working as an official at the Ministry of Truth. You have intersected a message subjected to Big Brother&apos;s doctrine.
</p>
<p>
    Your task is to delete letters from certain &quot;utterances&quot; in order to replace them with an &quot;utterance&quot; approved by the Ministry.
</p>
<p>
    A &quot;word&quot; is a single sequence of Latin letters, and an &quot;utterance&quot; is a sequence of multiple words and spaces.
</p>
<p>
    To compare two &quot;utterances,&quot; you have to replace all blocks of spaces with one space. Utterances are considered to be identical when resulting expressions match.
</p>
<p>
    One line contains two different expressions separated by semicolon &apos;;&apos;. The first expression is the original utterance, and the second one is the utterance you want to get.
</p>
<p>
    If you cannot fulfill the order, print a single line &#xAB;I cannot fix history&#xBB;. Otherwise, output the original utterance by replacing the letters that must be erased with underscore and by replacing all blocks of white spaces with a single white space.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. E.g.:
</p>
<pre class="description-input-output">Higher meaning;Hi mean
this is impossible;im possible
twenty   two minutes;two minutes
Higher meaning;e</pre>

<h3>Output sample:</h3>

<p>
    Print the results, or &quot;I cannot fix history&quot; in case there is no match. E.g.:
</p>

<pre class="description-input-output">Hi____ mean___
I cannot fix history
______ two minutes
____e_ _______</pre>

<h3>Constraints:</h3>
<p>
    The length of each utterance does not exceed 100,000 characters
</p>