<h2>Running for president</h2>

<h3>Challenge Description:</h3>

<p>
<span class="p-like">
        You&apos;re planning your party&apos;s campaign strategy to win the Presidency of the United States.
</span>
<span class="p-like">
        To win, your candidate has to navigate many controversial issues, which influence voters, such as healthcare,
        immigration, education, energy, independence, jobs, taxes, environment, and so on. Each of these is important,
        but also expensive to address.
</span>
</p>
<p>
    Because the United States presidential election is determined by states casting votes in the Electoral College, you
    need minimum 270 of the total 538 Electoral College votes to win.
</p>
<p>
    While not completely accurate, for this challenge we use the following criteria:
</p>
<ul>
<li>States may or may not value an issue.</li>
<li>States value each issue differently.</li>
<li>
        Winning 51% of any state gives you all of that state&apos;s votes. If you have less than 51 %, you won&apos;t receive
        any votes.
</li>
</ul>
<p>
    Your task is to put together a winning strategy by identifying the fewest issues you must address to win 270 votes.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a file as its first argument. The file content is the following:
</p>
<pre class="description-input-output">Social issues: 9

Healthcare: 33995797
Immigration: 2089699
Education: 37182280
Energy independence: 1344134
...
Wealth inequality: 99237127
Increase military spending: 44066575

Mississippi
Votes: 6
Creating jobs: 1
Jobs: 0
...
Increase military spending: 0
Education: 1
Energy independence: 0

Oklahoma
Votes: 7
Creating jobs: 1
Jobs: 2
...
Increase military spending: 0
Education: 1
Energy independence: 2

...

Maine
Votes: 4
Creating jobs: 0
Jobs: 0
...
Increase military spending: 0
Education: 1
Energy independence: 3
</pre>
<p>
    The first line identifies the total number of potential issues, the second&#x2014;information about costs for each program,
    and the third &#x2014; information about each state, separated by spacing. Each state has a name, number of votes, and a
    list of issues that you can choose in each state. Each of these issues is valued based on the number of votes it
    can get in each state. Remember, you must get the majority of votes in each state to win.
</p>

<h3>Output sample:</h3>

<p>
    Print out the list of issues you want to cover in you electoral program in alphabetical order.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">Energy independence
Healthcare
Immigration
Increase military spending
</pre>
<br>
<p>
    Remember, that your task is to create a program with the fewest number of issues. If there are several variants
    of program with the fewest number of issues, then you need to choose the program with minimum costs.
</p>
<br>