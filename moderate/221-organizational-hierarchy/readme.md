<h2>Organizational Hierarchy</h2>

<h3>Challenge Description:</h3>

<p>
    Everyone who has ever worked in a large organization understands the organizational hierarchy: you, your boss, boss
    of your boss, and so on. <br>
    Because of changes in all directions of the organization, everything was mixed up. From the existing documentation,
    you can understand only who is a manager and who is a subordinate. We need your help to recreate the whole
    organizational hierarchy using information from all existing documents.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with documents separated by a pipeline &apos;|&apos;.
    There are two letters in each document: 1st one &#x2013; the manager, 2nd one &#x2013; the subordinate.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">ab | ae | bc
ab | bc | cd | ae | cx | xz</pre>

<h3>Output sample:</h3>

<p>
    You should print the hierarchical tree in the following format: if a manager <b>a</b> has two subordinates
<b>e</b> and <b>b</b>, then the tree would be <b>a [b, e]</b>. You should sort all workers alphabetically.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">a [b [c], e]
a [b [c [d, x [z]]], e]</pre>

<h3>Constraints:</h3>
<ol>
<li>Hierarchical tree can be of no more than 4 levels.</li>
<li>Sort all subordinates of one manager in an alphabetical order.</li>
<li>The number of test cases is 15.</li>
</ol>