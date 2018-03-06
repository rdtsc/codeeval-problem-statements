<h2>Minesweeper</h2>

<h3>Challenge Description:</h3>
<p>
    You will be given an M*N matrix. Each item in this matrix is either a &apos;*&apos; or a &apos;.&apos;. A &apos;*&apos;
    indicates a mine whereas a &apos;.&apos; does not. The objective of the challenge is to output a M*N matrix
    where each element contains a number (except the positions which actually contain a mine which will remain as &apos;*&apos;)
    which indicates the number of mines adjacent to it. Notice that each position has at most 8 adjacent positions e.g.
    left, top left, top, top right, right, ...
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Each line in this file contains M,N,
    a semicolon and the M*N matrix in row major form. E.g.
</p>
<pre>3,5;**.........*...
4,4;*........*......</pre>

<h3>Output sample:</h3>

<p>
    Print out the new M*N matrix (in row major form) with each position(except the ones with the mines)
    indicating how many adjacent mines are there. E.g.
</p>

<pre>**100332001*100
*10022101*101110</pre>