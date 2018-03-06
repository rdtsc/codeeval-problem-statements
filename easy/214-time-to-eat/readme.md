<h2>Time to eat</h2>

<h3>Challenge Description:</h3>

<p>
    It&apos;s amazing how fast time flies by and we don&#x2019;t even realize it. As we are getting older, time seems to move
    so much faster than it did in the past. <br>
    Perception of time is relative to how fast our heart rate is. An unborn baby&#x2019;s heart rate is incredibly fast and
    as we age, it slows. Metabolic rate of an organism determines its perception of time. Organisms like cats and dogs
    have a very high metabolic rate; thus, the breaks between their meals seem to be shorter than humans have.  <br>
    At codeeval.com, we have a cat called Kitty. She loves eating, and it seems like she can eat anything any time. We
    want to keep Kitty fit, so we feed her according to a schedule. <br>
    Planning her daily meals, we need to see when Kitty will eat starting with the latest meal in the evening to the
    earliest morning snack. So, your task is to sort timestamps in the schedule in a reverse chronological order.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line includes a test case: a schedule containing unsorted timestamps
    in HH:MM:SS format.
</p>

<p>
    For example:
</p>

<pre class="description-input-output">02:26:31 14:44:45 09:53:27
05:33:44 21:25:41</pre>

<h3>Output sample:</h3>

<p>
    Sort timestamps in each schedule from the biggest to the smallest one.
</p>

<pre class="description-input-output">14:44:45 09:53:27 02:26:31
21:25:41 05:33:44</pre>

<h3>Constraints:</h3>
<ol>
<li>Each schedule may have from 2 to 20 timestamps.</li>
<li>Timestamp 23:59:59 - biggest and 00:00:01 the smallest one.</li>
<li>The number of test cases is 40.</li>
</ol>