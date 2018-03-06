<h2>Which way is faster?</h2>

<h3>Challenge Description:</h3>

<p>
    You must have heard about the famous Macedonian king, commander, and strategist of the Argead dynasty. This story
    is about Alexander of Macedon or Alexander the Great. We can talk about his deeds and victories for a long time
    and you have already heard most of them. <br>
    There is an event in the codeeval.com archive that no historian can tell you. It is about a small battle near
    Persia. Once, Alexander the Great sent the part of his army, led by Hephaistion&#x2014;the commander and his best
    friend&#x2014;to patrol the area. After a while, the herald brought bad news: the detachment was ambushed; they could
    hold out some time, but they needed urgent help. Alexander with the army was about to depart, but the question
    was &#x2013; which way would be faster: by sea or by land? <br>
    He decided to go by sea, and that was the right decision. This way was the fastest and Alexander saved the
    life of his warriors and his best friend.
</p>

<p>
    The following figures show a map that Alexander of Macedon had and two alternative ways. The first way is by sea,
    it took 4 hours (2 steps by land) to get to the port, followed by 1 hour of getting the army on board. Then,
    in 3 hours they passed 3 cells on the map, and, finally, landed in another port in 1 hour, plus 2 hours by
    land (1 cell up). <br>
    Total - 4 + 1 + 3 + 1 + 2 = 11 hours. <br>
    If they decided to go by land, it would have taken them 12 hours (3 cells left and 3 cells up) and most likely
    they would not have come in time to help.
<br> We want that you rely not only on a good luck, but also on your programming skills. Your task is to write
    a program that will calculate the fastest way from several alternatives.
</p>

<p>
    So, write a program that will determine the shortest time for the army to come and help, knowing that you
    have a map, where &apos;S&apos; - Start, &apos;F&apos; - Finish, &apos;P&apos; - 2 ports for a trip by sea.
    Why do you need it? Tripping by sea is the faster way. On the land, you should bypass mountains
    &apos;^&apos; if there are any.<br>
    Each step in the new cell takes 2 hours by land or 1 hour by sea, getting on the ship and landing the army
    also take 1 hour each. You need to calculate and print out the shortest time that the trip can take.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with map, where the following
    items are shown: <br>
    S - Start (This is your initial position) <br>
    F - Finish (This is the point where you need to lead the army to) <br>
    P - Port (The place where the army gets on board or lands) <br>
    ^ - Mountains (Which you should bypass) <br>
    * - Empty cells (Where you can safely move by ship and by land)
</p>

<p>
    For example:
</p>

<pre class="description-input-output">**^F | P**P | **** | S***
**^F | P*^P | **** | S***</pre>

<h3>Output sample:</h3>

<p>
    Calculate and print out the shortest time that the trip will take.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">11
12</pre>

<h3>Constraints:</h3>
<ol>
<li>The map is always square and can consist of 4 to 12 cells.</li>
<li>Every map is passable.</li>
<li>Mountains need to be bypassed.</li>
<li>One cell by land &#x2013; 2 hours, by sea &#x2013; 1 hour.</li>
<li>The number of test cases is 40.</li>
<li>This story is fictional. :)</li>
</ol>