<h2>Balanced Smileys</h2>

<h3>Challenge Description:</h3>
<p>
    Credits: This problem appeared in the Facebook Hacker Cup 2013 Hackathon.
<br>
<br>
    Your friend John uses a lot of emoticons when you talk to him on Messenger.
    In addition to being a person who likes to express himself through
    emoticons, he hates unbalanced parenthesis so much that it makes him go :(.
<br>
<br>
    Sometimes he puts emoticons within parentheses, and you find it hard to
    tell if a parenthesis really is a parenthesis or part of an emoticon.
    A message has balanced parentheses if it consists of one of the following:
<br>
<br>
    - An empty string &quot;&quot;
<br>
    - One or more of the following characters: &apos;a&apos; to &apos;z&apos;, &apos; &apos; (a space) or &apos;:&apos; (a colon)
<br>
    - An open parenthesis &apos;(&apos;, followed by a message with balanced parentheses,
    followed by a close parenthesis &apos;)&apos;.
<br>
    - A message with balanced parentheses followed by another message with
    balanced parentheses.
<br>
    - A smiley face &quot;:)&quot; or a frowny face &quot;:(&quot;
<br>
<br>
    Write a program that determines if there is a way to interpret his
    message while leaving the parentheses balanced.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Each line in this file contains a message that you got from John. E.g.
</p>
<pre class="description-input-output">:((
i am sick today (:()
(:)
hacker cup: started :):)
)(</pre>

<h3>Output sample:</h3>

<p>
    Print out the string &quot;YES&quot;/&quot;NO&quot; (all quotes for clarity only) stating
    whether or not it is possible that the message had balanced parentheses.
    E.g.
</p>

<pre class="description-input-output">NO
YES
YES
YES
NO</pre>