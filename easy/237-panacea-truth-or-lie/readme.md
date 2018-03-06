<h2>Panacea - truth or lie</h2>

<h3>Challenge Description:</h3>

<p>
    There are many computer and human viruses nowadays. Scientists are scratching their heads over antiviruses that
    could stop a particular virus and, in most cases, they find right solutions. <br>
    So, virologists need to know which antiviruses can protect us from viruses, and what they still have to work on
    to secure against the remaining viruses. Let&#x2019;s help them out!
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with virus components in the hexadecimal
    numeral system (HEX) and antivirus components in the binary number system (BIN). Virus and antivirus components
    are separated by a pipeline &apos;|&apos;.
</p>

<pre class="description-input-output">64 6e 78 | 100101100 11110
5e 7d 59 | 1101100 10010101 1100111
93 75 | 1000111 1011010 1100010</pre>

<h3>Output sample:</h3>

<p>
    Your task is to calculate the sum of all virus components and compare it with the sum of antivirus components.
    If the numbers are the same or the sum of antivirus components is greater than the sum of virus components,
    this means that the virus was stopped. So, print True. Otherwise, print False.
</p>

<pre class="description-input-output">True
True
False</pre>

<h3>Constraints:</h3>
<ol>
<li>The sum of components can be from 60 to 1500.</li>
<li>The number of components in virus and antivirus can be from 1 to 8.</li>
<li>The number of test cases is 40.</li>
</ol>