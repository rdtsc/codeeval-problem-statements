<h2>Column Names</h2>

<h3>Challenge Description:</h3>

<p>
    Microsoft Excel uses a special convention to name its column headers. The first 26 columns use the letters
    &apos;A&apos; to &apos;Z&apos;. Then, Excel names its column headers using two letters, so that the 27th and 28th column are &apos;AA&apos;
    and &apos;AB&apos;. After &apos;ZZ&apos;, Excel uses three letters.
</p>
<p>
    Write a function that takes as input the number of the column, and returns its header. The input will not ask
    for a column that would be greater than &apos;ZZZ&apos;.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line of the input file contains one test case represented by one
    integer.
</p>

<pre class="description-input-output">52
3702</pre>

<h3>Output sample:</h3>

<p>
    For each test case your program must print one line containing the Excel column heading
    corresponding to the integer in the input.
</p>

<pre class="description-input-output">AZ
ELJ</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of test cases is 40.</li>
<li>The input will not ask for a column that would be greater than &apos;ZZZ&apos;.</li>
</ol>