<h2>Suggest Groups</h2>

<h3>Challenge Description:</h3>
<p>
    You may have noticed that a new feature was added to our web site &#x2013; <a href="/groups/">user groups</a>. So, this challenge is about joining
    groups.
</p>
<p>
    You are given a list of users of a social network, friends of each user, and groups the user participates in.
</p>
<p>
    To help users find the most interesting groups, we suggest them joining the groups where &#x2265;50% of their friends
    participate.
</p>
<p>
    Your task is to write a program which finds a list of suggested groups for each user.
</p>

<h3>Input sample:</h3>
<p>
    The first argument is a file that contains the information about each user, one user per line. The line is delimited
    by colon &#x2018;:&#x2019; into three parts: user name, list of friends, and list of groups. The items in each part are delimited
    by comma &#x2018;,&#x2019;.
</p>
<p>For example:</p>

<pre class="description-input-output">Amira:Isaura,Lizzie,Madalyn,Margarito,Shakira,Un:Driving,Mineral collecting
Elliot:Isaura,Madalyn,Margarito,Shakira:Juggling,Mineral collecting
Isaura:Amira,Elliot,Lizzie,Margarito,Verla,Wilford:Juggling
Lizzie:Amira,Isaura,Verla:Driving,Mineral collecting,Rugby
Madalyn:Amira,Elliot,Margarito,Verla:Driving,Mineral collecting,Rugby
Margarito:Amira,Elliot,Isaura,Madalyn,Un,Verla:Mineral collecting
Shakira:Amira,Elliot,Verla,Wilford:Mineral collecting
Un:Amira,Margarito,Wilford:
Verla:Isaura,Lizzie,Madalyn,Margarito,Shakira:Driving,Juggling,Mineral collecting
Wilford:Isaura,Shakira,Un:Driving</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the list of suggested groups for each user. The list of users and the list of groups for each user
    must be sorted alphabetically.
</p>

<p>For example:</p>

<pre class="description-input-output">Isaura:Driving,Mineral collecting
Lizzie:Juggling
Madalyn:Juggling
Margarito:Driving,Juggling
Shakira:Driving,Juggling
Un:Driving,Mineral collecting</pre>

<h3>Constraints:</h3>
<ul>
<li>Number of users in input data is 200.</li>
<li>Number of different groups in input data is 15.</li>
<li>There can be users that do not participate in any group.</li>
<li>Friendship is mutual (if user A is a friend with user B, then user B is a friend with user A).</li>
</ul>