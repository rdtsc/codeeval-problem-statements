<h2>Mars Networks</h2>

<h3>Challenge Description:</h3>

<p>
    For the mission to Mars some areas are chosen, where soil, climate, and seismology investigations will be made.
    These areas are of size 10 000&#xA0;&#xD7;&#xA0;10 000 meters. The probes are sent to all these areas. For the effective work,
    the probes in each area must be connected to high-speed data network.
</p>
<p>
    Since delivery to Mars is very expensive, you have to determine the minimum length of the optical fiber cable
    which connects probes to a network.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains the space-separated coordinates of the site&#x2019;s probes, one line per site. X and Y coordinates are separated by comma.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">500,8000 1000,9500 2000,8500 1000,7500 4500,7000 5500,6500 7000,7000 2500,4000 1000,4000 1000,3000 3000,2500 2500,1000 3500,500 9000,6000 8500,4500 7500,4000 9000,3500 10000,3000
8028,5930 1835,5145 8537,9824 7623,7936 8031,1207
9349,3367 395,3342 3588,3655 9235,2503 1075,6413 2394,8353
9013,3937 7791,872 2417,3183
3416,472 8093,7510 1709,4893 9999,6958 6761,2692 2530,6753</pre>

<h3>Output sample:</h3>

<p>Print to stdout the minimum length of optical fiber cable for every site:</p>

<pre class="description-input-output">26602
15110
15335
9150
17770</pre>

<p>
    If the length is not integer (for example, 9063. 114), you should round it upward (9064).
</p>

<h3>Constraints:</h3>
<ol>
<li>Number of sites is 20.</li>
<li>Number of probes within one site can be from 3 to 250.</li>
<li>There can be 2 or more probes with the same coordinates &#x2014; in such case they do not need any cable
        to interconnect.</li>
</ol>