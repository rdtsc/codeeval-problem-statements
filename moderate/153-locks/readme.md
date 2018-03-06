<h2>Locks</h2>

<h3>Challenge Description:</h3>

<p>
    There are N unlocked rooms located in a row along the corridor.
</p>
<p>
    A security guard, who starts the beat at the beginning of the corridor, passes by and closes the lock of every
    second door (2<sup>nd</sup>, 4<sup>th</sup>, 6<sup>th</sup>&#x2026;). Then he returns to the beginning of the corridor,
    and passes by again changing the state of every third door (3<sup>rd</sup>, 6<sup>th</sup>, 9<sup>th</sup>&#x2026;) to the
    opposite state &#x2014; if the door is closed, security guard opens it; if the door is open, he closes it.
</p>
<p>
    One iteration consists of two beats (when the security guard closes each second door, and changes the state of
    each third door to the opposite state). The iteration repeats M-1 times.
</p>
<p>
    During the last iteration, the security guard just changes the state of the last door in a row (closes it, if the
    door is open or opens it, if the door is closed).
</p>
<p>
    Your task is to determine how many doors have been left unlocked.
</p>

<br>
<h3>Input sample:</h3>
<p>
    Your program accepts a filename as its first argument.
</p>
<p>
    Each line of input contains 2 integers separated by space. The first integer represents number of doors (N),
    the second &#x2014; number of iterations (M).
</p>
<br>

<pre class="description-input-output">3 1
100 100</pre>

<h3>Output sample:</h3>

<p>
    For each line of input print out how many doors are left unlocked:
</p>

<pre class="description-input-output">2
50</pre>