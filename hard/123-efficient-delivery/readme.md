<h2>Efficient Delivery</h2>

<h3>Challenge Description:</h3>
<p>
    A shipping company is providing oil delivery between two continents using tankers. They&#x2019;re trying to increase their
    efficiency by keeping their ships in port to wait for additional oil to prevent setting to sea only partially loaded.
<br>
    As a logistician, the challenge for you will be to determine all variations of efficient delivery based on the
    available tankers and the total amount of oil in barrels needed to achieve maximum efficiency.
<br>
    A tanker&apos;s carrying capacity is expressed in barrels of oil that it can take on board.
<br>
    E.g. the company has only two kind of tankers with the capacity of 2 and 5 barrels and the amount of oil to be transferred is 12 barrels.
    In this case there are two options of efficient delivery:
<br>
    1. load 6 tankers with the capacity of 2. [6,0]
<br>
    2. load 1 tanker with the capacity of 2 and 2 tankers with the capacity of 5. [1,2]
<br>
    In case the company had three kind of tankers with the capacity of 6, 7, 8 barrels and 10 barrels of oil to be transferred
    then there would be no option for efficient delivery and the minimum amount of oil needed would be 12 [2,0,0] so the answer in this case is 2.
<br>
    So you see that if there is no option to load the tankers effectively, you need to find out the minimum amount of oil
    which needs to be added to the given quantity to make the efficient delivery possible.

</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename
    containing rows with available tankers in brackets in sorted order, and the amount
    of oil after a comma. E.g.
</p>
<pre class="description-input-output">(2,5), 12
(6,9,20), 44
(197,8170), 155862
(2,4,8), 8</pre>

<h3>Output sample:</h3>

<p>
    Print out all possible variations of efficient delivery in sorted order if the efficient delivery exists.
    In another case print out the amount of oil to be added. E.g.
</p>
<pre class="description-input-output">[1,2][6,0]
[1,2,1][4,0,1]
3
[0,0,1][0,2,0][2,1,0][4,0,0]</pre>
<p>
    Constrains:
    Number of test cases is in range [20, 40]
<br>
    The number of tankers is in range [2, 5]
<br>
    A tanker&apos;s capacity is in range of [2, 10000] barrels
<br>
    Oil amount is in range of [1, 200000] barrels
</p>