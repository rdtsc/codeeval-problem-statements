<h2>Everything or nothing</h2>

<h3>Challenge Description:</h3>

<p>
    Today, you have a top-secret assignment. You will have access to a super confidential information about documents
    with the highest security rate. There are only three such documents in the world which include extremely important
    information. If any of these files fall into the wrong hands, there is a risk that the global balance of power can
    be destroyed. <br>
    Only 6 people have access to these files, each with the different access rights&#x2014;from a total ban to a full access.
    Several lines of code from these files leaked into the Internet recently. Your task will be to check the code that
    we provide. But, be careful: if you agree to take this task, you automatically sign an agreement on non-disclosure
    of confidential information; otherwise, we will have to &#x2026; you. <br> <br>
    The following is a transcript of all rights to the files: <br>
    0 - total ban;<br>
    1 - grant;<br>
    2 - write;<br>
    3 - write, grant;<br>
    4 - read;<br>
    5 - read, grant;<br>
    6 - read, write;<br>
    7 - full access (read, write, grant); <br>
<br>
    The following table shows what access to a particular file each of these 6 users had.
</p><pre class="description-input-output">         file_1   file_2   file_3
user_1     7        3        0
user_2     6        2        4
user_3     5        1        5
user_4     3        7        1
user_5     6        0        2
user_6     4        2        6</pre>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with several lines of code separated by a
    space. In each line, first comes the user name, then the file name, and finally what the user done with this
    file. <br>
    If it is granting an access to someone, then the code contains the action that is granted followed by a name of a
    user who has been granted access. For each test case, a table above will be a starting point. That is, if the
    action is user_3=&gt;file_3=&gt;grant=&gt;read=&gt;user_1, the number in the table for user_1 will change from 0 to 4. However,
    for the next test cases, it will again be 0.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">user_1=&gt;file_1=&gt;read user_2=&gt;file_2=&gt;write
user_1=&gt;file_1=&gt;grant=&gt;read=&gt;user_4 user_4=&gt;file_1=&gt;read
user_4=&gt;file_1=&gt;read</pre>

<h3>Output sample:</h3>

<p>
    You must go through all the lines of code, and if at least one is not correct, print False; otherwise, bring True.
</p>

<pre class="description-input-output">True
True
False</pre>

<h3>Constraints:</h3>
<ol>
<li>
        The table with users is the same for each test case, but it can change within a test case depending on the code.
</li>
<li>The number of lines of code in a test case can be from 1 to 8.</li>
<li>User with grant permissions can provide rights on read and write to himself.</li>
<li>The number of test cases is 40.</li>
</ol>