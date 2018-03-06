<h2>Testing</h2>

<h3>Challenge Description:</h3>

<p>
    In many teams, there is a person who tests a project, finds bugs and errors, and prioritizes them.<br>
    Now, you have the unique opportunity to try yourself as a tester and test a product. Here, you have two strings - the
    first one is provided by developers, and the second one is mentioned in design. You have to find and count the
    number of bugs, and also prioritize them for fixing using the following statuses:  &apos;Low&apos;, &apos;Medium&apos;,
    &apos;High&apos;, &apos;Critical&apos; or &apos;Done&apos;.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with two strings separated by a pipeline
    &apos;|&apos;. The first string is the one the developers provided to you for testing, and the second one is from design.
</p>

<pre class="description-input-output">Heelo Codevval | Hello Codeeval
hELLO cODEEVAL | Hello Codeeval
Hello Codeeval | Hello Codeeval</pre>

<h3>Output sample:</h3>

<p>
    Write a program that counts the number of bugs and prioritizes them for fixing using the following statuses: <br>
    &apos;Low&apos; - 2 or fewer bugs; <br>
    &apos;Medium&apos; - 4 or fewer bugs; <br>
    &apos;High&apos; - 6 or fewer bugs; <br>
    &apos;Critical&apos; - more than 6 bugs; <br>
    &apos;Done&apos; - all is done; <br>
</p>

<pre class="description-input-output">Low
Critical
Done</pre>

<h3>Constraints:</h3>
<ol>
<li>Strings are of the same length from 5 to 40 characters.</li>
<li>Upper and lower case matters.</li>
<li>The number of test cases is 40.</li>
</ol>