<h2>A bus network</h2>

<h3>Challenge Description:</h3>
<p>
    You have just moved to a new city where the main transport facility is a bus. You have noticed that for each bus route,
    it takes a bus 7 minutes to ride between the adjacent stops, and it takes 12 minutes for you to change a bus.
    To use your time more efficiently, write a program that determines how to get from point A to point B in the least amount
    of time using a following list of bus routes.
<br>
<br>
    The bus route R1 a list of bus stops ID represented in the same order as
    they appear on the route. You can change a bus only at the stop with the same ID.
</p>

<p>
    For example:
</p>

<pre>R1=[1,2,3,4]; R2=[5,6,4]; R3=[9,6,7]; R4=[12,1,2,3,11,16,15,14,10,7]</pre>
<p>
    To get from point 1 to point 7, you can start from the bus route R1, and ride to the stop with ID=4,
    change the route R1 to the route R2 to reach the stop with ID=6, then change R2 to R3 to arrive at the stop with ID=7,
    or you can simply take the bus route R4, occupy a seat, relax, and ride straight to a stop with ID=7.
    Your task is to determine the fastest possible route.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument.
    Each line in the file is one test case. Each test case contains the points A and B in brackets
    and a list of routes separated by a semicolon.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">(2,4); R1=[1,2,3,11,12,4]; R2=[5,6,4]; R3=[1,6,7]; R4=[5,6,4]; R5=[8,6,3]
(1,7); R1=[1,2,3,4]; R2=[5,6,4]; R3=[9,6,7]; R4=[12,1,2,3,11,16,15,14,10,13,7]
(3,299); R1=[1,2,3,4]; R2=[6,7,19,12,4]; R3=[11,14,16,6]; R4=[24,299,42,6]
(3,4); R1=[1,2,3]; R2=[6,7,19,12,4]; R3=[11,14,16,6]</pre>

<h3>Output sample:</h3>
<p>
    For each test case print out the minimum time in minutes needed to get from point A to point B using the given bus routes or
    print out &quot;None&quot; if there is no connection between these two points.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">28
59
73
None</pre>
<p>
<br>
    Constraints:
<br>
    The number of routes is in a range from 3 to 150.
<br>
    The IDs are in a range from 0 to 300.
<br>
    The length of a route is in a range from 10 to 35 stops.
</p>