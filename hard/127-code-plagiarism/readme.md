<h2>Code Plagiarism</h2>

<h3>Challenge Description:</h3>
<p>
    We propose you to solve an exciting challenge: find plagiarism in one piece of source code against another. This
    challenge is similar to revealing plagiarism in two texts; but, in case of source code, we know the syntax of a
    language and we can be more accurate in finding renamed data structures and other cheating.
</p>
<p>
    We do not provide any ranking points for this task. However, those developers who send a good working solution
    to us will receive a special badge.
</p>
<p>
    To make the challenge more interesting, we have chosen two programming
    languages: Python and Go. You will have two pairs of source code to compare.
    The first one is written in Python, and the second one – in Go. You will need
    to find duplicates in Python code chunks, and then in Go code chunks. Thus,
    you will not need to compare Python code and Go code.
</p>
<p>
    Our test cases for both languages are the following:
</p>
<ol>
    <li>The same code</li>
    <li>Changed names of variables</li>
    <li>One is a half of another</li>
    <li>Removed documentation strings and comments</li>
    <li>Shuffled functions</li>
    <li>Small part of code is inside of another code</li>
    <li>Two approaches to the same problem</li>
    <li>Different code</li>
    <li>"Hello World"</li>
</ol>
<p>
    Please feel free to  contact the support at codeeval.com if you can add more test cases suitable for this task.
    Also, if for successful challenge completion you need to install some library for the language used, contact
    the support.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a filename as its first argument. The input file contains 18 sets of test cases
    (9 for Python and 9 for Go). You can check the input file on
    <a href="input.txt">GitHub</a>.
    Each test case is separated by five asterisks. The first line of each test case is the title, for example "&lt;&lt;&lt;
    Python The same code." Two code samples inside of each test case are separated by five equal signs.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">&lt;&lt;&lt; Python The same code   # first test case

def quickSort(alist):
    ... new code

&#61;&#61;&#61;&#61;&#61;

def quickSort(alist):
    ... existing code

&#42;&#42;&#42;&#42;&#42;
&lt;&lt;&lt; Go The same code  # second test case

package main
    ... new code

&#61;&#61;&#61;&#61;&#61;

package main
    ... existing code

&#42;&#42;&#42;&#42;&#42;
&lt;&lt;&lt; Python Changed names of variables  # Third test case
            etc.</pre>

<h3>Output sample:</h3>

<p>
    For each test case, produce a single line of output containing the percentage of plagiarism comparing <em>new</em>
    code with the <em>existing</em> one.
</p>
<pre class="description-input-output">100
95
0</pre>
