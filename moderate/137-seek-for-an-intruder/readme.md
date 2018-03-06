<h2>Seek for an Intruder</h2>

<h3>Challenge Description:</h3>
<p>
    A company&apos;s server has been down for a couple of hours due to an unauthorized intrusion. After bringing it back
    live, a security department started to investigate the log files in order to find any trails of a hacker. Luck was
    on their side: they found a broken network log file containing pieces of useful data that could possibly help them
    identify an intruder. Among the garbage of ASCII uppercase and lowercase letters, punctuation marks, and digits,
    they found IP addresses in various formats.
</p>
<p>
    For example:
</p>
<pre>Dotted decimal	192.0.2.235 with no leading zero.
Dotted hexadecimal 0xc0.0x0.0x02.0xeb Each octet is individually converted to hexadecimal form.
Dotted octal 0300.0000.0002.0353 Each octet is individually converted into octal.
Dotted binary 11000000.00000000.00000010.11101011 Each octet is individually converted into binary.
Binary 11000000000000000000001011101011
Octal 030000001353
Hexadecimal	0xC00002EB	Concatenation of the octets from the dotted hexadecimal.
Decimal	3221226219	The 32-bit number expressed in decimal.</pre>
<p>
    To help them finish their investigation and find the hacker, you need to find the most frequently occurring
    IP address in that file. You must search only for a valid IPv4 address in a range from 1.0.0.0 to 255.255.255.254.
</p>
<p>
    The input sample below contains:
</p>
<pre>Valid IP addresses:
    1000000111011100010000001100101
    01000000.11101110.00100000.01100101
    034062405073
    023244514100
    033642264316
    222.137.104.206
    10110010011001001101100010111010
<u>0131.0345.0202.0341</u>
<u>0x59.0xe5.0x82.0xe1</u>
<u>89.229.130.225</u>
<u>1011001111001011000001011100001</u>
<u>89.229.130.225</u>

Not valid IP addresses:
    1101100000.1001010111.101010101.1110010101
    864.599.341.917
    01540.01127.0525.01625
    0x360.0x257.0x155.0x395
    864.599.341.917
    864.599.341.917</pre>
<p>
     The IP address 89.229.130.225 appears five times so it&apos;s the one we&apos;ve been searching for.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. The file contains the N number of lines with
    the length of M symbols.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">m*M}Qz`\fz/We}e[`md;Puuat-;UP|Yi64iXh%{Hnul8&amp;onq0p*mY+4x\/{ZTw[gXeJV2&amp;.P*Ywe
VA,8Z%z-AYzp6o{qeX3Q|\`Zw7{78:Y80qP-,b0BDVvZh60x59.0xe5.0x82.0xe1uptW8eF8C]nKJ9c(AtXa9&gt;Dy}nF&apos;Jr
Cq2ox2Mmr7PuaPO023244514100.@({-mER/yhWg)wsf&quot;`Fu_tp.C]6$!?(^+wzLBxi,PJ41Hdu`m&gt;Bz=v*^~N|h
jfZ&amp;y9w&apos;XkrrO6JDoZOyZ864.599.341.917JBJ5u(^i%BjecAd&quot;$4UKtPnbtvx^01540.01127.0525.01625tU$HY/,Uw(/CJP]L+/XohV2hD&amp;]
9Pl.1011001111001011000001011100001,Y,HNAiSzL;?BU_UQlCvyzRU^&quot;R]{kVJ&quot;[+3%PK`]\&quot;V?;Y&apos;8CjJ&lt;&amp;QGmESP6W7&amp;P,@$tFtL
`z6DR}/&gt;gLfLX[1&amp;]Vr8&quot;EG-_+wy?sw4beHIp^oTtZzvWBwY{[89.229.130.225R,?B;&quot;?[ix4^9D$fVaJ_V\)N`B
=ddalCNOM)FnA=/r,?}#idpo1E#eeMq.wyfu/2viz;c_[kHppMh,K|\`Q1_R(`jRNvCZW2Niz7Q#
w:b21f[rsnj^Rgg[t!(&lt;5v`Iup^&amp;]o@489.229.130.225gw4\SwBEbN222.137.104.206[Jo&lt;)lj36bB.034062405073xx37d;~wKi/D&quot;I&apos;AeVfeBO
|7$mi3k]f}9N*Vjq5aMy[Xd+3a$n$paB?5p9^01000000.11101110.00100000.01100101u@0:7&amp;J;8FDZ&lt;LuN-ecftQ%XU2urHk=N&quot;y}1Zt+
|lLN|l8ZlMi()kN29/B!uj~l8#1o?Kcp/1{FfL]1/NsK$&lt;@`)0P+LVgv4ziP&gt;t840131.0345.0202.0341`}Z*Xz[8IH?&apos;
^~H5]JqL#?&gt;d8V5JPP1101100000.1001010111.101010101.11100101011Funfr=3*E\pEa&quot;3YV^?J+;dLA#t)$3Lvi5J&lt;MSF]LB&amp;yOXgO&apos;t/E864.599.341.917Ze033642264316z~7
W7+1&amp;dt2#Ek&amp;&lt;am6G|!!18P&gt;?|?qQyV(0k?&gt;KPB:t{IRUm&gt;cuN0^[YSOsixxF&quot;zzl5LALPIaXFM.
jMfgpfH+w&gt;M8\`r{;`XdEYm0Rc7o&gt;Aqq4k?gP&gt;,O^2I^]OF#zN\cLSUQ(x!(oxA0l&lt;xjM=-qcIXE
_L)a,&lt;}f4u9dc]&apos;440h0y7Yu=&amp;NOfz-k%hk/FLpVZBsX|+P5YjaNBH]TCG~{,k]Dc\7p$)s&amp;4D+Y
xI~0JkBd]}c#]!4eGec7oz&gt;d:yYl*K_AK^Hd_&lt;c+hjD4w:-[90?}lBZ]^@iT2A&amp;i9=9tsjg3muNC
,6ze^#eqtjrd`P&amp;?WY,J-]L)_gVR*NJ~]Q(#l&quot;Yu~Jpl*ui&quot;9JtZ=&amp;2B{!6&quot;iP@Y@3I%Zft&gt;cpd`
OwEK!d?y\M(_L~|=lm1++BLA&lt;&amp;PnOnBAfga&gt;t},x{T$*&amp;/}+wX{j/pm&apos;|N~Cq1000000111011100010000001100101x~[*Scc=lb82`K~
HydTS#@@864.599.341.917Q&amp;.DVb\ails}C101100100110010011011000101110100&amp;@KyFK&quot;7}u3\63?u][~zz&gt;-r$_OqUbE*uv,\ccCnUmP\&lt;p,o4E6[7c]
v&lt;md%aG2z8n&apos;}&quot;9}qwZYnHdo&gt;`4/Ht!3puL.A\&apos;].BA&gt;reos{U0x360.0x257.0x155.0x395y^UGXh^&apos;`|I.CV}R&gt;a}RAhO%Vw
uQ#27/z^B8q:x(I|$k9dmF{\&lt;ofV5sg[F&gt;P(t!ui5[&lt;mpXTzO%0wF|E2Sh6bl5[YZ:Tm%JsE*5pUO</pre>

<h3>Output sample:</h3>
<p>
    Print out the most frequently occurring IP address in a dotted decimal representation without leading zeros.
    In case there is more than one most frequently occuring IP address, then print them both out in ascending order
    separated by a white space.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">89.229.130.225</pre>

<h3>Constraints:</h3>
<ol>
<li>M is in range [100, 300]</li>
<li>N is in range [800, 1200]</li>
</ol>

<br>