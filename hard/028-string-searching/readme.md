<h2>String Searching</h2>

<h3>Challenge Description:</h3>
<p>
    You are given two strings. Determine if the second string is a substring of the first
    (Do NOT use any substr type library function). The second string may contain an asterisk(*)
    which should be treated as a regular expression i.e. matches zero or more characters. The asterisk can be escaped
    by a \ char in which case it should be interpreted as a regular &apos;*&apos; character. To summarize: the strings can contain
    alphabets, numbers, * and \ characters.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    The input file contains two comma delimited strings per line. E.g.
</p>
<pre>Hello,ell
This is good, is
CodeEval,C*Eval
Old,Young
</pre>

<h3>Output sample:</h3>

<p>
   If the second string is indeed a substring of the first, print out a &apos;true&apos;(lowercase), else print out a
   &apos;false&apos;(lowercase), one per line. E.g.
</p>
<pre>true
true
true
false
</pre>