<h2>Juggle Fest</h2>

<h3>Challenge Description:</h3>

<p>
    Many developers here at Yodle are avid jugglers. To celebrate their prowess we are organizing a Yodle Open JuggleFest,
    but we need your help planning it. There will be thousands of participants split into teams. Each team will attempt
    to complete a juggling circuit consisting of several tricks.
</p>
<p>
    Each circuit emphasizes different aspects of juggling,
    requiring hand to eye coordination (H), endurance (E) and pizzazz (P) in various amounts for successful completion.
    Each juggler has these abilities in various amounts as well. How good a match they are for a circuit is determined
    by the dot product of the juggler&apos;s and the circuit&apos;s H, E, and P values. The higher the result, the better the match.
<br>
<br>
    Each participant will be on exactly one team and there will be a distinct circuit for each team to attempt.
    Each participant will rank in order of preference their top X circuits. Since we would like the audiences to enjoy
    the performances as much as possible, when assigning jugglers to circuits we also want to consider how well their
    skills match up to the circuit. In fact we want to match jugglers to circuits such that no juggler could switch to
    a circuit that they prefer more than the one they are assigned to and be a better fit for that circuit than one of
    the other jugglers assigned to it.
<br>
<br>
    To help us create the juggler/circuit assignments write a program in a language of your choice that takes as input
    a file of circuits and jugglers and outputs a file of circuits and juggler assignments. The number of jugglers
    assigned to a circuit should be the number of jugglers divided by the number of circuits. Assume that the number
    of circuits and jugglers will be such that each circuit will have the same number of jugglers with no remainder.
</p>

<h3>Input sample:</h3>
<p>
    One line per circuit or juggler. All circuits will come before any jugglers. Circuit lines start with a C and
    juggler lines start with a J. Names of circuits and jugglers will never have spaces. A skill and the rating for
    that skill are separated by a colon. Circuit lines have the circuit names followed by skills. Juggler lines have
    the juggler names followed by skills, followed by circuits in order of preference, separated by commas. Example:
</p>
<pre class="description-input-output">C C0 H:7 E:7 P:10
C C1 H:2 E:1 P:1
C C2 H:7 E:6 P:4

J J0 H:3 E:9 P:2 C2,C0,C1
J J1 H:4 E:3 P:7 C0,C2,C1
J J2 H:4 E:0 P:10 C0,C2,C1
J J3 H:10 E:3 P:8 C2,C0,C1
J J4 H:6 E:10 P:1 C0,C2,C1
J J5 H:6 E:7 P:7 C0,C2,C1
J J6 H:8 E:6 P:9 C2,C1,C0
J J7 H:7 E:1 P:5 C2,C1,C0
J J8 H:8 E:2 P:3 C1,C0,C2
J J9 H:10 E:2 P:1 C1,C2,C0
J J10 H:6 E:4 P:5 C0,C2,C1
J J11 H:8 E:4 P:7 C0,C1,C2</pre>

<h3>Output sample:</h3>

<p>
    You should have one line per circuit assignment. Each line should contain the circuit name followed by the juggler
    name, followed by that juggler&apos;s circuits in order of preference and the match score for that circuit. The line
    should include all jugglers matched to the circuit. The example below is a valid assignment for the input file above (has 3 lines).
</p>

<pre class="description-input-output">C2 J6 C2:128 C1:31 C0:188, J3 C2:120 C0:171 C1:31, J10 C0:120 C2:86 C1:21, J0 C2:83 C0:104 C1:17
C1 J9 C1:23 C2:86 C0:94, J8 C1:21 C0:100 C2:80, J7 C2:75 C1:20 C0:106, J1 C0:119 C2:74 C1:18
C0 J5 C0:161 C2:112 C1:26, J11 C0:154 C1:27 C2:108, J2 C0:128 C2:68 C1:18, J4 C0:122 C2:106 C1:23</pre>
<p>
    Run your program on the input which contains 2000 circuits and 12000 jugglers. The correct output is the sum of the
    names of the jugglers (taking off the leading letter J) that are assigned to circuit C1970. So for example if the
    jugglers assigned to circuit C1970 were J1,J2,J3,J4,J5 and J6 the correct answer would be
</p>
<pre class="description-input-output">21 </pre>