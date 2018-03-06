<h2>Skyscrapers</h2>

<h3>Challenge Description:</h3>
<p>
    You are to design a program which helps you in drawing the skyline of a city.
    You are given the locations of the buildings represented by triples (L, H, R) where L and R are left and
    right coordinates of the building and H is the height of the building.
    All buildings are rectangular in shape and they are standing on a very flat surface. E.g.
<br>

<br>

<br>
    On the first diagram the buildings are represented by the following triples:
</p>
<pre>(1,2,3); (2,4,6); (4,5,5); (7,3,11); (9,2,14); (13,7,15); (14,3,17)</pre>
<p>
    The drawing line as shown on the second diagram is described by the following sequence:
</p>
<pre>1 2 2 4 4 5 5 4 6 0 7 3 11 2 13 7 15 3 17 0</pre>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file is one test case. Each test case will contain the list of triples semicolon separated. E.g.
</p>
<pre class="description-input-output">(1,2,3);(2,4,6);(4,5,5);(7,3,11);(9,2,14);(13,7,15);(14,3,17)
(2,22,3);(6,12,10);(15,6,21)
(1,2,6);(9,23,22);(22,6,24);(8,14,19);(23,12,30)</pre>

<h3>Output sample:</h3>
<p>
    The output must describe the drawing line as a vector (X1,H1,X2,H2,X3,H3,X3,Xn-1,Hn-1,Xn) where X is a x-coordinate
    of a point where the line is changing its direction from horizontal to vertical, and H is a height of the vertical line.
    You&apos;re drawing continuously by starting at the bottom of the first left building and finishing at
    the bottom of the right building. So for each test case print out the drawing line in a way as it is shown below.
</p>
<pre class="description-input-output">1 2 2 4 4 5 5 4 6 0 7 3 11 2 13 7 15 3 17 0
2 22 3 0 6 12 10 0 15 6 21 0
1 2 6 0 8 14 9 23 22 6 23 12 30 0</pre>
<p>
    Notice that the elimination of hidden lines is one of the problems that appear in CAD (computer-aided design).
<br>
<br>
    Constraints:
<br>
    H in range (1, 100),  max(x-coordinate) &lt;= 10000, number of buildings &lt;= 1000
</p>