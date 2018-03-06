<h2>Racing Chars</h2>

<h3>Challenge Description:</h3>
<p>
    You are given a file where each line is a section of a race track with obstructions, gates, and checkpoints.
    Your task is to find a way to pass this track using the following information:
</p><p>
        1. Each section contains either one single gate or one gate with a checkpoint.
<br>
        2. You should drive only through gates or checkpoints.
<br>
        3. You should drive through a checkpoint rather than a gate.
<br>
        4. An obstruction is represented by a number sign &quot;#&quot;.
<br>
        5. A gate is represented by an underscore &quot;_&quot;.
<br>
        6. A checkpoint is represented by a letter C.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument.
    Each line of the file is a new section of a race track.
</p>

<pre class="description-input-output">#########_##
########C_##
#######_####
######_#C###
#######_C###
#######_####
######C#_###
######C_####
#######_####
#######_####</pre>

<h3>Output sample:</h3>

<p>
    Print out the way of passing this race track starting from the first line in the file.
    Use a pipe &quot;|&quot; for the straight, use a slash &quot;/&quot; for the left turn, and use a backslash &quot;\&quot;
    for the right turn.
</p>

<pre class="description-input-output">#########|##
########/_##
#######/####
######_#\###
#######_|###
#######/####
######/#_###
######|_####
#######\####
#######|####</pre>

<h3>Constraints:</h3>

<ul>
<li>The number of lines in a file is 50.</li>
<li>The width of a section is 12 characters.</li>
</ul>