<h2>Seat your team members</h2>

<h3>Challenge Description:</h3>
<p>
    Your team is moving to a new office.
    In order to make it feel comfortable on a new place you decided to give the possibility to
    pick the places where they want to sit. After the team visited the new office,
    each team member gave you a list of working places that he/she would like to occupy.
    Your goal is to determine a possibility of making all
    of your team members feel comfortable according to those lists.
<br>
<br>
    All working places in the new office are numbered from 1 to N.
    And each team member gave you the list which contained the places in unsorted order.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line of the file contains an integer N of available places in the office as the first digit and the lists of places that have been chosen by each team member.
    These lists are enclosed by square brackets. E.g.
</p>
<pre>4; 1:[1, 3, 2], 2:[1], 3:[4, 3], 4:[4, 3]
3; 1:[1, 3, 2], 2:[1], 3:[1]
</pre>

<h3>Output sample:</h3>

<p>
    For each line of input print out the simple &quot;Yes&quot; or &quot;No&quot; answer for the following question:
    &quot;Is there a possibility to make all of your team members feel comfortable at the new office?&quot;. E.g.
</p>

<pre>Yes
No
</pre>
<p>
    Constraints:
<br>
    N is an integer in range [1, 50].
<br>
    The number of team members is &lt;= N.
<br>
    Each team member can pick 1 to N numbers of working places.
</p>