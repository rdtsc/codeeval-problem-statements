<h2>Alphabet blocks</h2>

<h3>Challenge Description:</h3>

<p>
    We all remember those childhood times when we learned how to use alphabet blocks to form different words, such as MOM, DAD, TRAIN, and others.
    We propose you to remind this time for a while and imagine yourself being a child.<br>
    So, you have a set of alphabet blocks. There is a letter on each of the six faces of every block. Also, you have a
    word associated with your childhood that you want to form.<br>
    Write a program that will verify if it is possible to form the necessary word out of the set. If yes, then
    print &quot;True&quot; to stdout; otherwise, print &quot;False&quot;.<br>
    You can choose only one letter from an alphabet block and place blocks in any order.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a path to a file. Each line contains test cases that have three arguments separated by the pipe symbol &quot;|&quot;.
<br>1. The first argument in the line is a number that shows how many blocks are in the set.
<br>2. The second one is a word that you want to form.
<br>3. The third one is a list of arrays of letters. One face of the alphabet block includes one letter from array.
<br>For example:
<br>There is an array of letters <strong>&quot;ABCDEF&quot;</strong>. It refers to one toy block with the following faces: <br> <strong>&quot;A&quot;, &quot;B&quot;, &quot;C&quot;, &quot;D&quot;, &quot;E&quot;, &quot;F&quot;.</strong>
</p>

<pre class="description-input-output">4 | DOG | UPZRHR INOYLC KXDHNQ BAGMZI
6 | HAPPY | PKMFQP KTXGCV OSDMAJ SDSIMY OEPGLE JZCDHI
5 | PLAIN | BFUBZD XMQBNM IDXVCN JCOIAM OZYAYH</pre>

<h3>Output sample:</h3>

<p>
    Print &quot;True&quot; to stdout if you can form the necessary word, or &quot;False&quot; if you cannot do this.
</p>

<pre class="description-input-output">True
True
False</pre>

<h3>Constraints:</h3>
<ol>
<li>The word length is from 4 to 18 characters.</li>
<li>Number of blocks in the set is always equal to or greater than the word length.</li>
<li>You can take only one block from the set to form one letter in the word.</li>
<li>The letters in the word and letters on the faces of one block may repeat: the word might be &quot;MOM&quot; or there might be a block with &quot;AAAAAA&quot; faces. </li>
<li>The number of test cases is 40.</li>
</ol>