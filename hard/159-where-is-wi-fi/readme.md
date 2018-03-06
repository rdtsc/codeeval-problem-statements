<h2>Where is Wi-Fi</h2>

<h3>Challenge Description:</h3>

<p>The car with the Wi-Fi radar is driving along the streets. It collects information about the accessible Wi-Fi hotspots in some definite places by determining MAC-address and azimuth angle to the hotspot. Also, the city map is available. It provides the list of buildings and coordinates of polygons vertices that form their outlines.</p>
<p>Your task is to determine in which buildings hotspots are located.</p>

<h3>Input sample:</h3>

<p>The first argument is a path to a file that contains the city map and the Wi-Fi radar log. The city map is separated from the Wi-Fi radar log by an empty line.</p>
<p>The city map is represented as a list of buildings, one building per line. Each line of city map data starts with a building name and is followed by coordinates of vertices that form its outline. Coordinates are pairs X and Y separated by semicolon &#x2018;;&#x2019;. Coordinates are separated by space.</p>
<p>Each line of the Wi-Fi radar log starts with coordinates X and Y separated by semicolon &#x2018;;&#x2019; of radar&#x2019;s current position. If any hotspot was detected radar coordinates are followed by its MAC-address and azimuth angle (in degrees) separated by semicolon &#x2018;;&#x2019;.</p>

<pre>B001 14.88;8.94 14.88;33.23 25.29;33.23 25.29;15.88 32.23;15.88 32.23;8.94 14.88;8.94
B002 14.88;33.23 14.88;43.64 49.58;43.64 49.58;26.29 39.17;26.29 39.17;33.23 14.88;33.23
<span>... some lines skipped ...</span>
B010 63.45;50.58 70.39;50.58 70.39;43.64 63.45;43.64 63.45;50.58

56.51;5.47 56-4c-18-eb-13-8b;59.3493 88-fe-14-a4-aa-2a;303.0239
42.64;5.47 88-fe-14-a4-aa-2a;0.0000
28.76;5.47 88-fe-14-a4-aa-2a;56.9761
14.88;5.47 88-fe-14-a4-aa-2a;71.9958
11.41;15.88
11.41;29.76
<span>... some lines skipped ...</span>
56.51;64.45 f9-aa-de-15-28-46;277.5946 de-c2-8e-34-08-17;214.6952</pre>

<h3>Output sample:</h3>

<p>Print to stdout names of buildings which have Wi-Fi hotspots. The order should be alphabetical.</p>

<pre>B003
B005
B007
</pre>

<h3>Constraints:</h3>
<ol>
<li>0&#xB0; azimuth direction is the same as +Y axis direction</li>
<li>Hotspots can be located both inside and outside of the building</li>
<li>There can be more than one hotspot in the building</li>
<li>Hotspots are immovable during all measurements</li>
</ol>