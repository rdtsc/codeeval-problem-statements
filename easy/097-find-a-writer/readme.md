<h2>Find a Writer</h2>

<h3>Challenge Description:</h3>

<p>
    You have a set of rows with names of famous writers encoded inside.
    Each row is divided into 2 parts by pipe char (|).
    The first part has a writer&apos;s name. The second part is a &quot;key&quot; to generate
    a name.
</p>
<p>
    Your goal is to go through each number in the key (numbers are separated by space)
    left-to-right.
    Each number represents a position in the 1st part of a row.
    This way you collect a writer&apos;s name which you have to output.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Input example is the following
</p>
<pre>osSE5Gu0Vi8WRq93UvkYZCjaOKeNJfTyH6tzDQbxFm4M1ndXIPh27wBA rLclpg| 3 35 27 62 51 27 46 57 26 10 46 63 57 45 15 43 53

3Kucdq9bfCEgZGF2nwx8UpzQJyHiOm0hoaYP6ST1WM7Nks5XjrR4IltBeDLV vA| 2 26 33 55 34 50 33 61 44 28 46 32 28 30 3 50 34 61 40 7 1 31</pre>
<p>
    This input had 2 rows.
</p>

<h3>Output sample:</h3>

<p>
    Print results in the following way.
</p>

<pre>Stephen King 1947
Kyotaro Nishimura 1930</pre>