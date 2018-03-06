<h2>Discount Offers</h2>

<h3>Challenge Description:</h3>

<p>
    Our marketing department has just negotiated a deal with several
    local merchants that will allow us to offer exclusive discounts on
    various products to our top customers every day. The catch is that we
    can only offer each product to one customer and we may only offer
    one product to each customer.
</p>
<p>
    Each day we will get the list of products that are eligible for these
    special discounts. We then have to decide which products to offer to
    which of our customers. Fortunately, our team of highly skilled
    statisticians has developed an amazing mathematical model for determining
    how likely a given customer is to buy an offered product by calculating
    what we call the &quot;suitability score&quot; (SS).
    The top-secret algorithm to calculate the SS between a customer and
    a product is this:
<br>
<br>
    1. If the number of letters in the product&apos;s name is even then
    the SS is the number of vowels (a, e, i, o, u, y) in the customer&apos;s
    name multiplied by 1.5.
<br>
    2. If the number of letters in the product&apos;s name is odd then the SS
    is the number of consonants in the customer&apos;s name.
<br>
    3. If the number of letters in the product&apos;s name shares any common
    factors (besides 1) with the number of letters in the customer&apos;s name
    then the SS is multiplied by 1.5.
<br>
<br>
    Your task is to implement a program that assigns each customer a product
    to be offered in a way that maximizes the combined total SS across all
    of the chosen offers. Note that there may be a different number of
    products and customers. You may include code from external libraries
    as long as you cite the source.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its only argument a path to a file.
    Each line in this file is one test case. Each test case will be a comma
    delimited set of customer names followed by a semicolon and then a comma
    delimited set of product names. Assume the input file is ASCII encoded.
    For example (NOTE: The example below has 3 test cases):
<br>
<br>
</p>
<pre>Jack Abraham,John Evans,Ted Dziuba;iPad 2 - 4-pack,Girl Scouts Thin Mints,Nerf Crossbow</pre>
<pre>Jeffery Lebowski,Walter Sobchak,Theodore Donald Kerabatsos,Peter Gibbons,Michael Bolton,Samir Nagheenanajar;Half &amp; Half,Colt M1911A1,16lb bowling ball,Red Swingline Stapler,Printer paper,Vibe Magazine Subscriptions - 40 pack</pre>
<pre>Jareau Wade,Rob Eroh,Mahmoud Abdelkader,Wenyi Cai,Justin Van Winkle,Gabriel Sinkin,Aaron Adelson;Batman No. 1,Football - Official Size,Bass Amplifying Headphones,Elephant food - 1024 lbs,Three Wolf One Moon T-shirt,Dom Perignon 2000 Vintage</pre>

<h3>Output sample:</h3>

<p>
    For each line of input, print out the maximum total score to two
    decimal places. For the example input above,
    the output should look like this:
</p>
<pre>21.00
83.50
71.25</pre>