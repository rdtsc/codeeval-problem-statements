<h2>JSON menu IDs</h2>

<h3>Challenge Description:</h3>
<p>
    You have JSON string which describes a menu.
    Calculate the SUM of IDs of all &quot;items&quot; in the case a &quot;label&quot; exists for an item.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Input example is the following
</p>
<pre>{&quot;menu&quot;: {&quot;header&quot;: &quot;menu&quot;, &quot;items&quot;: [{&quot;id&quot;: 27}, {&quot;id&quot;: 0, &quot;label&quot;: &quot;Label 0&quot;}, null, {&quot;id&quot;: 93}, {&quot;id&quot;: 85}, {&quot;id&quot;: 54}, null, {&quot;id&quot;: 46, &quot;label&quot;: &quot;Label 46&quot;}]}}

{&quot;menu&quot;: {&quot;header&quot;: &quot;menu&quot;, &quot;items&quot;: [{&quot;id&quot;: 81}]}}

{&quot;menu&quot;: {&quot;header&quot;: &quot;menu&quot;, &quot;items&quot;: [{&quot;id&quot;: 70, &quot;label&quot;: &quot;Label 70&quot;}, {&quot;id&quot;: 85, &quot;label&quot;: &quot;Label 85&quot;}, {&quot;id&quot;: 93, &quot;label&quot;: &quot;Label 93&quot;}, {&quot;id&quot;: 2}]}}</pre>
<p>
    All IDs are integers between <b>0</b> and <b>100</b>. It can be 10 items maximum for a menu.
</p>

<h3>Output sample:</h3>

<p>
    Print results in the following way.
</p>

<pre>46
0
248</pre>