<h2>Ray of Light</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a plan of a room with 10&#xD7;10 cells size. The walls in the room are marked with a number sign &#x2018;#&#x2019;.
    They are specular and they reflect light. If a ray hits a corner of the room, its distribution stops:
</p>

<pre><span class="s-gray">-------</span>    <span class="s-gray">-------</span>
<span class="s-gray">-</span>#####<span class="s-gray">-</span>    <span class="s-gray">-</span>#####<span class="s-gray">-</span>
<span class="s-gray">-</span>  /\#<span class="s-gray">-</span>    <span class="s-gray">-</span>   /#<span class="s-gray">-</span>
<span class="s-gray">-</span> / /#<span class="s-gray">-</span>    <span class="s-gray">-</span>  / #<span class="s-gray">-</span>
<span class="s-gray">-</span>/ / #<span class="s-gray">-</span>    <span class="s-gray">-</span> /  #<span class="s-gray">-</span>
<span class="s-dimmed">/</span><span class="s-gray">------</span>    <span class="s-gray">-</span><span class="s-dimmed">/</span><span class="s-gray">-----</span></pre>

<p>
    There can be columns and prisms in the room at a distance at least 1 cell from the walls.
</p>
<p>
    The columns are marked with the &#x2018;o&#x2019; symbol. They absorb light. If a ray hits a column, its distribution stops:
</p>

<pre><span class="s-gray">-------</span>
<span class="s-gray">-</span>     <span class="s-gray">-</span>
<span class="s-gray">-</span>  o  <span class="s-gray">-</span>
<span class="s-gray">-</span> /   <span class="s-gray">-</span>
<span class="s-gray">-</span>/    <span class="s-gray">-</span>
<span class="s-dimmed">/</span><span class="s-gray">------</span></pre>

<p>
    The prisms are marked with an asterisk &#x2018;*&#x2019;. They split a ray into three parts. One of them goes in the same
    direction as the original ray, two others are turned by &#xB1;90&#xB0;:
</p>

<pre><span class="s-gray">------</span>
<span class="s-gray">-</span> \ /<span class="s-gray">-</span>
<span class="s-gray">-</span>  * <span class="s-gray">-</span>
<span class="s-gray">-</span> / \<span class="s-gray">-</span>
<span class="s-gray">-</span>/   <span class="s-gray">-</span>
<span class="s-dimmed">/</span><span class="s-gray">-----</span></pre>

<p>
    There is a hole in one of the walls. A ray of light is let into the room through the hole at an angle aliquot
    to 45&#xB0; to the walls:
</p>
<pre>##########
#        #
#  o  o  #
#    o o #
# o   *o #
# o o    #
# * * *o #
#        #
#        #
###/######</pre>

<p>
    Show the path of light distribution using pseudo-graphics. Use slash &#x2018;/&#x2019; to show the fragment turned to 45&#xB0; or 225&#xB0;,
    backslash &#x2018;\&#x2019; to show the fragment turned to 315&#xB0; or 135&#xB0;, and &#x2018;X&#x2019; symbol to show the fragment where two rays
    are crossed:
</p>

<pre>##########
#\   /\  #
# \o/ o\ #
#  X o o\#
# o \ *o/#
# o o\ / #
# * * *o #
#    / \ #
#   /   \#
###/######</pre>

<p>
    The maximum distance of light distribution is 20 cells, including the first and the last cells, but excluding
    the cells with prisms.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file with test cases. Each line contains serialized plan of a room, starting from the
    upper-left cell.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">###########        ##  o  o  ##    o o ## o   *o ## o o    ## * * *o ##        ##        ####/######
###########        ##    *   ## *      ##    *   ##   *    ##     ** ##     ** ##        ####/######
###########        ##    * o ##  o     #/    o   ## o *    ##        ##        ##        ###########</pre>

<h3>Output sample:</h3>

<p>
    Show the path of light distribution on the plan, using pseudo-graphics. Print the result to stdout in a serialized
    way similarly to the input.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">###########\   /\  ## \o/ o\ ##  X o o\## o \ *o/## o o\ / ## * * *o ##    / \ ##   /   \####/######
###########\ /\/X\ ## X /* \\##/*X/ \ X##\//\* X/##/X *\//\##X \ /**/##\\ X/** ## \X/\/ \####X######
###########  /\ /\ ## /  * o\##/ o/ \ /#/  / o X ## o * / \##/ \ /  /##\  X  / ## \/ \/  ###########</pre>

<h3>Constraints:</h3>
<ol>
<li>A room size is 10&#xD7;10 cells.</li>
<li>The maximum distance of light distribution is 20 cells, including the first and the last cells, but excluding
        the cells with prisms.</li>
<li>There are 40 test cases in the input.</li>
</ol>

<br>