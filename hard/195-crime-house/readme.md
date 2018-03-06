<h2>Crime House</h2>

<h3>Challenge Description:</h3>

<p>
<small>This challenge appeared in Google Code Jam competition, licensed under
<a href="http://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution License</a></small>
</p>

<p>
    While working for the police, you&apos;ve identified a house where people go to commit crimes, called Crime House.
    One day, you set up a camera over the door of the house and record a video.
</p>

<p>
    You don&apos;t know how many people were in Crime House at the start of the day, but you can see people enter and leave
    through the front door. Unfortunately, because the people entering and leaving Crime House are criminals, sometimes
    they wear masks; and you aren&apos;t quite sure if the front door is the only way in or out.
</p>

<p>
    Sometimes you can guess who was wearing a mask. If criminal #5 entered the house, then someone wearing a mask left,
    then criminal #5 entered the house again, then either the person wearing the mask was criminal #5, or there is
    another way out of Crime House.
</p>

<p>
    At the end of the day, when Crime House has closed its doors for the night, you watch your video. Because you&apos;re
    an optimist, you want to figure out if it&apos;s possible that there are no other entrances or exits from crime house;
    and if so, you want to figure out the minimum number of people who could be in Crime House at the end of the day.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line of the input file contains one test case.
    Each test case starts with a single integer N, the number of times people pass through the front door of Crime House
    in the day. Next, after the semicolon, follows N events, separated by a pipe.
    Each event contains information about one person entering or leaving Crime House through the front door.
</p>

<p>
    That information consists of a single character, E or L, followed by a space and then an integer id.
    If the first character is E, that indicates someone entered Crime House through the front door;
    if it&apos;s L, someone left through the front door. If id is greater than zero, the person with that identifier entered
    or left Crime House. If id is zero, then the person who entered or left Crime House was wearing a mask,
    and we don&apos;t know who he or she was.
</p>

<pre class="description-input-output">3; E 5|L 0|E 5
2; L 1|L 1
4; L 1|E 0|E 0|L 1
7; L 2|E 0|E 1|E 2|E 0|E 3|L 4
13; L 4|L 1|L 2|E 0|L 1|E 0|L 2|E 0|L 2|E 0|E 0|L 1|L 4</pre>

<h3>Output sample:</h3>

<p>
    For each test case, output one line containing the answer. If it&apos;s possible that there are no other entrances or
    exits from Crime House, then the answer should be the minimum number of people who could be in Crime House at the
    end of the day. If that&apos;s impossible, it should be &quot;CRIME TIME&quot;.
</p>

<pre class="description-input-output">1
CRIME TIME
1
4
0</pre>

<h3>Constraints:</h3>
<ol>
<li>The number of test cases is 20.</li>
<li>Ids of criminals are in range from 0 to 2000 inclusive.</li>
<li>The number of events is in range from 1 to 15 inclusive.</li>
</ol>