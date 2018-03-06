<h2>Trick or Treat</h2>

<h3>Challenge Description:</h3>

<p>
    Everyone knows what Halloween is and how children love it. Children in costumes travel from house to house asking
    for treats with a phrase &quot;Trick or treat&quot;. After that, they divide the treats equally among all. This year, they
    collected tons of candies, and need your help to share everything equally. <br>
    You know that children receive different number of candies depending on their costume: vampire gets 3 candies
    from one house, zombie &#x2013; 4 candies, and witch &#x2013; 5 candies. <br>
    That is, three children in three different costumes get 3+4+5=12 candies from one house.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case with number of vampires, zombies, witches,
    and houses that they visited.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">Vampires: 1, Zombies: 1, Witches: 1, Houses: 1
Vampires: 3, Zombies: 2, Witches: 1, Houses: 10</pre>

<h3>Output sample:</h3>

<p>
    You need to print number of candies that each child will get. If the number is not integer, round it to
    the lower: for example, if the resulting number is 13.666, round it to 13.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">4
36</pre>

<h3>Constraints:</h3>
<ol>
<li>Number of vampires, zombies, witches, and houses can be from 0 to 100.</li>
<li>If the final number of candies is not integer, round it to the lower.</li>
<li>The number of test cases is 40.</li>
</ol>