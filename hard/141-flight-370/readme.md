<h2>Flight 370</h2>

<h3>Challenge Description:</h3>
<p>
    You have probably heard about the tragedy that happened to one of the Malaysian airplanes. Many countries support
    the search mission with ships, planes, and rescue services. There is also a web app which allows people to help with
    the search. It is called <a href="http://www.tomnod.com/nod/">Tomnod</a>. Thousands of volunteers are browsing the
    satellite images to explore the Earth and solve the real-world problems. They mark the items they have found with
    the special tags. You can also join the search by going to <a href="http://www.tomnod.com/">http://www.tomnod.com/</a>
    and signing in. All the search results regarding the Malaysian flight are in an XML file that you can download
<a href="assets/malaysiaairsar2014_crowdrank.kmz">here</a>. Each item found
    and marked on the map is represented by the following XML section:
</p>
<pre class="description-input-output">    &lt;Placemark id=&apos;4889783&apos;&gt;
        &lt;name&gt;Oil Slick ID 4889783&lt;/name&gt;&lt;Snippet maxLines=&apos;0&apos;&gt;&lt;/Snippet&gt;
        &lt;type&gt;Oil Slick&lt;/type&gt;
        &lt;description&gt;&lt;![CDATA[
            &lt;img src=&apos;https://s3.amazonaws.com/explorationlab/chips/08458a6f42a780af66c05d0ef1385558.jpg&apos; height=400 width=400&gt;&lt;br/&gt;
            &lt;table width=400&gt;&lt;tr&gt;&lt;td width=40%&gt;CrowdRank: &lt;b&gt;100%&lt;/b&gt;&lt;br/&gt;Confirmation: &lt;b&gt;2&lt;/b&gt; people&lt;br/&gt;
            &lt;td align=&apos;right&apos; valign=&apos;bottom&apos;&gt;Image &#xA9; DigitalGlobe 2014&lt;br&gt;&lt;br&gt;&lt;a href=&apos;http://tomnod.com/nod/challenge/mh370_indian_ocean/map/983378&apos;&gt;See this point on &lt;img src=&apos;http://www.tomnod.com/nod/images/logo_small.png&apos; width=100&gt;&lt;/a&gt;
        &lt;/tr&lt;/table&gt;
        ]]&gt;&lt;/description&gt;
        &lt;styleUrl&gt;#tag_type_130&lt;/styleUrl&gt;
        &lt;TimeStamp&gt;&lt;when&gt;2014-03-27 18:14:25.234888&lt;/when&gt;&lt;/TimeStamp&gt;
        &lt;Point&gt;&lt;coordinates&gt;79.834979564799994,6.97011026235&lt;/coordinates&gt;&lt;/Point&gt;
    &lt;/Placemark&gt;</pre>
<p>
    An item is called a placemark. It has a name, a type, a point with coordinates, a timestamp when it was marked, and
    a description section with the confirmation in it.
</p>
<p>
    You are given a point on the Earth surface, represented by a longitude and a latitude, and a radius in kilometers.
    Your task is to print out the name of the placemark that was confirmed by the largest amount of people in the given
    area.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument. The first N lines of the file contain
    the regions, one per line. Other lines contain the XML code itself starting with the following line:
</p>
<pre>&lt;?xml version=&apos;1.0&apos; encoding=&apos;UTF-8&apos;?&gt;</pre>
<p>
    For example:
</p>

<pre class="description-input-output">70; (96.289565663600001, 4.0044008079599998)
873; (92.749414588199997, 11.692508007600001)
98; (105.364957907, 6.6474719752600002)
20; (80.185393420699995, 7.5700396347199996)
&lt;?xml version=&apos;1.0&apos; encoding=&apos;UTF-8&apos;?&gt;
&lt;kml xmlns=&apos;http://www.opengis.net/kml/2.2&apos;&gt;
&lt;Document&gt;

... Document body ...

&lt;/Document&gt;
&lt;/kml&gt;</pre>

<h3>Output sample:</h3>
<p>
    For each test case print out the name of the placemark that was confirmed by the largest amount of people. If there
    is more than one placemark with the same maximum amount of confirmations, print out the names ordered by timestamp
    starting from the most recent ones, separated by comma and a single space. In case the timestamps are the same,
    print out placemarks ordered by Id. Print out &apos;None&apos; in case there is no placemark in a given area.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">Other ID 4398192, Other ID 4402502, Other ID 4437554, Other ID 4437645, Oil Slick ID 4519894
Wreckage ID 6757595
Other ID 3835555
None</pre>

<h3>Constraints:</h3>
<ol>
<li>R is in a range from 20 to 3000.</li>
<li>N is in a range from 10 to 15</li>
</ol>
