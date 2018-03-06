<h2>Visit to the Headquarters</h2>

<h3>Challenge Description:</h3>
<p>
    The Department of Security has a new headquarters. The building has several floors, and on each floor there are
    rooms numbered XXYY, where XX stands for the floor number, YY for the room number, and XX&#xA0;&gt;&#xA0;0;
    YY&#xA0;&lt;=&#xA0;10. The building has paternoster &#x2013; a passenger elevator, which consists of several cabins that move
    slowly up and down without stopping. From time to time, the agents visit the headquarters. During the visit they go
    to see several rooms and stay in each room for some time. Due to the security reasons, only one agent can be in the
    room at the same time. The same rule applies to the elevators, only one agent can be in the elevator at the same
    time. The visits are planned to be completed within one day. Each agent visits the headquarters once a day.
</p>
<p>
    The agent enters the building on the 1st floor, passes the reception, and visits the rooms according to his/her
    list. Agents always visit the rooms in the increasing room number. The agents form a linear hierarchy according to
    the personal codes that were assigned to them. Agents with higher seniority have smaller codes in lexicographical
    order. The two agents cannot have the same code.
</p>
<p>
    If there are more than one agent who wants to enter a room, or an elevator, they have to form a queue. The queue is
    formed according to the codes. The higher the seniority of the agent, the closer to the top of the queue he stands.
    Agents can enter the elevator every 5 seconds. There is a queue for up and down directions of the elevator on each
    floor. After visiting the last room in the headquarters, the agent uses elevator to the first floor (if necessary)
    and exits the building.
</p>

<p>The time necessary to move from one point in the headquarters to another is set as follows:</p>

<ol>
<li>Entering the building (passing the reception and reaching the elevator or a room on the first floor) takes
        10&#xA0;seconds.</li>
<li>Exiting the building (stepping out of the elevator or a room on the first floor and passing the reception)
        takes 10&#xA0;seconds.</li>
<li>On the same floor, the way from the elevator to the room (or to the queue in front of the room), or from
        the room to the elevator (or to the queue in front of the elevator), or from one room to another (or to
        the queue in front of the room) takes 10&#xA0;seconds.</li>
<li>The way up or down from one floor to another using an elevator takes 10&#xA0;seconds.</li>
</ol>
<p>Write a program that determines time when the agent leaves the headquarters.</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a filename as its first argument. Each line of the file contains the description of
    the agent visit. The description of each visit consists of agent&apos;s one character code (C), time (T) when the agent
    enters the headquarters, and the room numbers (XXYY) followed by the time in seconds (S) that agent may spend in
    the room. E.g.
</p>
<pre>C T XXYY S XXYY S XXYY S ...</pre>
<p>
    The time when the agent enters the headquarters is in the HH:MM:SS format. E.g.
</p>

<pre class="description-input-output">A 09:00:00 0203 5 0210 10 0305 5 0604 10 0605 10 0901 10 0908 10
B 09:00:25 0205 10 0404 5 0501 5 0602 5 0703 5 0807 5
C 09:00:45 0109 10 0110 5 0207 5 0208 10 0401 10 0510 5
D 09:01:15 0310 5 0404 5 0503 10 0603 5 0604 5 0704 10 0708 5 0910 5 1005 10</pre>

<h3>Output sample:</h3>

<p>
    For each test case print out the time when agent entered the headquarters and the time when agent left
    the headquarters in the HH:MM:SS format separated by a single space. E.g.
</p>

<pre class="description-input-output">09:00:00 09:05:50
09:00:25 09:05:40
09:00:45 09:04:40
09:01:15 09:08:15</pre>
<h3>Constraints:</h3>
<ul>
<li>S is in range [5, 100]</li>
<li>C is in range [A, Z]</li>
</ul>