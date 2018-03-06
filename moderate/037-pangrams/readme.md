<h2>Pangrams</h2>

<h3>Challenge Description:</h3>

<p>
    The sentence &apos;A quick brown fox jumps over the lazy dog&apos; contains every single letter in the alphabet.
    Such sentences are called pangrams. You are to write a program, which takes a sentence, and returns all the
    letters it is missing (which prevent it from being a pangram). You should ignore the case of the letters in
    sentence, and your return should be all lower case letters, in alphabetical order. You should also ignore all
    non US-ASCII characters.In case the input sentence is already a pangram, print out the string NULL
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. This file will contain several text strings,
    one per line. E.g.
</p>
<pre>A quick brown fox jumps over the lazy dog
A slow yellow fox crawls under the proactive dog</pre>

<h3>Output sample:</h3>

<p>
    Print out all the letters each string is missing in lowercase, alphabetical order . E.g.
</p>

<pre>NULL
bjkmqz</pre>