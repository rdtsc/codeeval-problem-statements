<h2>URI Comparison</h2>

<h3>Challenge Description:</h3>
<p>
    Determine if two URIs match. For the purpose of this challenge, you should
    use a case-sensitive octet-by-octet comparison of the entire URIs,
    with these exceptions:
<br>
<br>
    1. A port that is empty or not given is equivalent to the default port of 80
<br>
    2. Comparisons of host names MUST be case-insensitive
<br>
    3. Comparisons of scheme names MUST be case-insensitive
<br>
    4. Characters are equivalent to their % HEX HEX encodings. (Other than typical reserved characters in urls like , / ? : @ &amp; = + $ #)
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains two urls delimited by a semicolon. E.g.
</p>
<pre>http://abc.com:80/~smith/home.html;http://ABC.com/%7Esmith/home.html</pre>

<h3>Output sample:</h3>

<p>
    Print out True/False if the URIs match. E.g.
</p>

<pre>True</pre>