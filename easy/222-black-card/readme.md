<h2>Black card</h2>

<h3>Challenge Description:</h3>

<p>
    You must have heard about pirates, their customs, pirates code, and the &#x201C;black spot&#x201D;. If a pirate is presented
    with a &#x201C;black spot&#x201D;, he is officially pronounced guilty, meaning he will soon be expulsed from the pirate
    brotherhood or even be dead. <br>
    We don&#x2019;t have as strict rules as pirates have, and a person who receives a black spot simply leaves the game. <br>
    For example, we have a list of three players: John, Tom, Mary, and a number 5. Starting with the first player
    (in our case, it&#x2019;s John), we start to count all players: John &#x2013; 1, Tom &#x2013; 2, Mary &#x2013; 3, and then again starting
    from the first one John &#x2013; 4, Tom &#x2013; 5. As Tom gets number 5, he should leave. Now, we have John and Mary and start
    counting again. John gets number 5, so he leaves. Thus, the winner is Mary.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with names of players and a number for a
    &#x201C;black spot&#x201D;. Players and a number are separated by a pipeline &apos;|&apos;.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">John Sara Tom Susan | 3
John Tom Mary | 5</pre>

<h3>Output sample:</h3>

<p>
    Print the name of a winner.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">Sara
Mary</pre>

<h3>Constraints:</h3>
<ol>
<li>Always start counting from the first name in a list.</li>
<li>Number of players can be from 3 to 10.</li>
<li>Number of turns can be from 3 to 15.</li>
<li>The number of test cases is 40.</li>
</ol>