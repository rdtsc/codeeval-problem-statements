<h2>Car Race</h2>

<h3>Challenge Description:</h3>
<p>Your task is to find out how fast each car goes around a given race track. The race track is represented by a
    sequence of float and integer numbers. Each float number is the length of a straight section in miles, followed
    by an integer number that represents an angle of the turn in degrees. Each car is described by its top speed in
    miles per hour (MPH), the time to reach the top speed from 0 MPH, and the time to brake from its top speed to 0 MPH.
</p>
<p>
    There are the following rules:
</p>
<p>
        1. A car is weightless.
<br>
        2. A car speeds up and brakes with a constant acceleration.
<br>
        3. The speed of a turn is linearly dependent on the turn degree and can be obtained from the following proportion:
        a car can pass through a 0 degree turn with its top speed, but it must brake to 0 MPH if a turn degree is 180.
<br>
        4. A car starts with 0 MPH speed, accelerates to its top speed, goes at the top speed as long as possible,
        then brakes as late as possible to reach the allowed turn speed, and after the turn immediately accelerates from
        the turn speed to the top speed, and so on.
<br>
        5. No time is needed to pass a turn, it is just a point and at that point the speed of a car must be exactly the
        same as the allowed turn speed.
<br>
        6. The length of a track section always allows a car to reach its top speed.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument. The first line of the file contains a track,
    represented by a sequence of numbers separated by a single space, the other N lines contain cars. Each car is a
    line with parameters separated by a single space in the following order: car number, top speed, time to accelerate
    form 0 MPH to a top speed, time to brake from a top speed to 0 MPH.
</p>

<p>For example:</p>

<pre class="description-input-output">1.029 115 1.122 125 1.185 100 0.53 110 0.751 95 1.242 85 0.533 85 1.003 120 0.465 110 0.546 125 0.446 90 0.582 70 0.878 45 0.49 30 1.016 130 1.047 140 1.146 75 0.496 85 0.857 125 0.971 0
1 266 8.1 1.4
2 178 8.7 4.8
3 251 8.0 3.4
4 215 6.8 3.8
5 220 5.9 3.3
6 262 4.5 1.5
7 267 5.4 2.6
8 268 7.8 3.8
9 225 4.7 1.8
10 266 4.0 1.9</pre>

<h3>Output sample:</h3>

<p>
    Print out the car number with its lap time separated by a single space. Each car must be printed out in a new
    line ordered from the fastest to the slowest lap. The lap time must be in seconds rounded to the hundredth of
    a second.
</p>

<pre class="description-input-output">10 241.05
6 244.98
7 247.32
1 254.07
8 258.67
3 273.02
9 283.52
5 298.28
4 309.22
2 375.86</pre>

<h3>Constraints:</h3>
<p>N is in range [20, 40]</p>