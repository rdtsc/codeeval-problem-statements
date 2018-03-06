<h2>Bay Bridges</h2>

<div id="map-canvas"></div>

<br>
<h3>Challenge Description:</h3>

<p>
    A new technological breakthrough has enabled us to build bridges that can
    withstand a 9.5 magnitude earthquake for a fraction of the cost. Instead of
    retrofitting existing bridges which would take decades and cost at least
    3x the price we&apos;re drafting up a proposal rebuild all of the bay area&apos;s
    bridges more efficiently between strategic coordinates outlined below. 
</p>

<p>
    You want to build the bridges as efficiently as possible and connect as many
    pairs of points as possible with bridges such that no two bridges cross.
    When connecting points, you can only connect point 1 with another point 1,
    point 2 with another point 2. 
</p>

<p>
    At example given on the map we should connect all the points except points
    with number 4.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename.
    Input example is the following
</p>
<pre class="description-input-output">1: ([37.788353, -122.387695], [37.829853, -122.294312])
2: ([37.429615, -122.087631], [37.487391, -122.018967])
3: ([37.474858, -122.131577], [37.529332, -122.056046])
4: ([37.532599,-122.218094], [37.615863,-122.097244])
5: ([37.516262,-122.198181], [37.653383,-122.151489])
6: ([37.504824,-122.181702], [37.633266,-122.121964])</pre>
<p>
    Each input line represents a pair of coordinates for each possible bridge.
</p>

<h3>Output sample:</h3>
<p>
    You should output bridges in ascending order.
</p>

<pre class="description-input-output">1
2
3
5
6</pre>
<p>
    (Check lines on the map)
</p>

<script type="text/javascript" src="https://maps.googleapis.com/maps/api/js?key=AIzaSyATY9ALwgMNKu3ggL8aJlHy09qiNZaNcIA&amp;sensor=false"></script>
<script type="text/javascript" src="https://google-maps-utility-library-v3.googlecode.com/svn/tags/markerwithlabel/1.1.8/src/markerwithlabel.js"></script>
<script type="text/javascript">
var google_map;
var google_map_center = new google.maps.LatLng(37.640879, -122.25174);
function initialize() {
    var mapDiv = document.getElementById('map-canvas');
    google_map = new google.maps.Map(mapDiv, {
        center: google_map_center,
        zoom: 10,
        mapTypeId: google.maps.MapTypeId.ROADMAP
    });
}

$(function() {
    initialize();

    var sf_coords_str = "1: ([37.788353, -122.387695], [37.829853, -122.294312])\n\
2: ([37.429615, -122.087631], [37.487391, -122.018967])\n\
3: ([37.474858, -122.131577], [37.529332, -122.056046])\n\
4: ([37.532599,-122.218094], [37.615863,-122.097244])\n\
5: ([37.516262,-122.198181], [37.653383,-122.151489])\n\
6: ([37.504824,-122.181702], [37.633266,-122.121964])";

    var sf_coords = [];
    var markers = {};
    var lines = [];

    sf_coords_str_lines = sf_coords_str.split("\n");
    for (i = 0; i < sf_coords_str_lines.length; i++){
        var matches = sf_coords_str_lines[i].match(/(\d+)\:\s*\(\[(\-*\d+\.*\d*),\s*(\-*\d+\.*\d*)\],\s*\[(\-*\d+\.*\d*),\s*(\-*\d+\.*\d*)\]\)/);
        sf_coords.push([parseInt(matches[1]), parseFloat(matches[2]), parseFloat(matches[3]), parseFloat(matches[4]), parseFloat(matches[5])]);
    }
    for (i = 0; i < sf_coords.length; i++){
        var point_name = "" + sf_coords[i][0];
        markers[point_name + "1"] = new MarkerWithLabel({
            position: new google.maps.LatLng(sf_coords[i][1], sf_coords[i][2]),
            map: google_map,
            labelContent: point_name
        });
        markers[point_name + "2"] = new MarkerWithLabel({
            position: new google.maps.LatLng(sf_coords[i][3], sf_coords[i][4]),
            map: google_map,
            labelContent: point_name
        });
    }
    //var right_order = ["1", "5", "2", "3", "4"];
    for (i = 0; i < sf_coords.length; i++){
        var line = new google.maps.Polyline({
            path: new Array(markers[sf_coords[i][0] + "1"].getPosition(),markers[sf_coords[i][0] + "2"].getPosition()),
            strokeColor: (i != 3)?'#ff0000':'#0000ff',
            strokeOpacity: 1.0,
            strokeWeight: 2
        });
        line.setMap(google_map);
    }

});

</script>