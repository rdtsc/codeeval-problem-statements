<h2>Commuting Engineer</h2>

<div id="map-canvas"></div>

<br>
<h3>Challenge Description:</h3>
<p>
    Commuters in the bay area who commute to and from South Bay spend
    on average 2-3 hours of valuable time getting to and from work every day.
    That&apos;s why startups like Mashery, Flurry, New Relic and Glassdoor
    have called the San Francisco Peninsula their home.
</p>

<p>
    Today, we&apos;re visiting some of area&apos;s fastest growing startups
    and would like to find the shortest possible distance to visit
    each company once starting from the CodeEval offices at 1355 Market Street.
</p>

<p>
    Solving the following challenge means finding the shortest possible route which visits each coordinate once starting from the point 1.
    You may read more about the <a href="http://en.wikipedia.org/wiki/Travelling_salesman_problem">Travelling salesman problem</a>
</p>

<p>
    On the map you can see the best route for 6 coordinates.
    But we&apos;ve added 4 more for the offices of Mashery, Flurry, New Relic
    and Glassdoor. So you need to find the best route for 10 coordinates.
</p>

<h3>Input sample:</h3>
<p>
    Your program should accept as its first argument a path to a filename. Input example is the following
</p>
<pre class="description-input-output">1 | CodeEval 1355 Market St, SF (37.7768016, -122.4169151)
2 | Yelp 706 Mission St, SF (37.7860105, -122.4025377)
3 | Square 110 5th St, SF (37.7821494, -122.4058960)
4 | Airbnb 99 Rhode Island St, SF (37.7689269, -122.4029053)
5 | Dropbox 185 Berry St, SF (37.7768800, -122.3911496)
6 | Zynga 699 8th St, SF (37.7706628, -122.4040139)</pre>

<p>
    The following locations will also be present in the input file:
<br>
<b>
        7 | Mashery 717 Market St, SF (37.7870361, -122.4039444)
<br>
        8 | Flurry 3060 3rd St, SF (37.7507903, -122.3877184)
<br>
        9 | New Relic 188 Spear St, SF (37.7914417, -122.3927229)
<br>
        10 | Glassdoor 1 Harbor Drive, Sausalito (37.8672841, -122.5010216)
</b>
</p>

<h3>Output sample:</h3>
<p>
    It must start from position 1
</p>

<pre class="description-input-output">1
3
2
5
6
4</pre>

<p>
    (Check points on the map)
</p>

<p>
    If you&apos;re able to solve this challenge and interested in Mashey, Flurry,
    New Relic or Glassdoor, you&apos;ll be able to apply directly after submitting
    your solution. Let&apos;s see if it cuts down your work commute!
</p>

<script type="text/javascript" src="https://maps.googleapis.com/maps/api/js?key=AIzaSyATY9ALwgMNKu3ggL8aJlHy09qiNZaNcIA&amp;sensor=false"></script>
<script type="text/javascript" src="https://google-maps-utility-library-v3.googlecode.com/svn/tags/markerwithlabel/1.1.8/src/markerwithlabel.js"></script>
<script type="text/javascript">
var google_map;
var google_map_center = new google.maps.LatLng(37.780145, -122.402544);
function initialize() {
    var mapDiv = document.getElementById('map-canvas');
    google_map = new google.maps.Map(mapDiv, {
        center: google_map_center,
        zoom: 14,
        mapTypeId: google.maps.MapTypeId.ROADMAP
    });
}

$(function() {
    initialize();

    var sf_coords_str = "1 | CodeEval 1355 Market St, SF (37.7768016, -122.4169151)\n\
2 | Yelp 706 Mission St, SF (37.7860105, -122.4025377)\n\
3 | Square 110 5th St, SF (37.7821494, -122.4058960)\n\
4 | Airbnb 99 Rhode Island St, SF (37.7689269, -122.4029053)\n\
5 | Dropbox 185 Berry St, SF (37.7768800, -122.3911496)\n\
6 | Zynga 699 8th St, SF (37.7706628, -122.4040139)\n\
7 | Mashery 717 Market St, SF (37.7870361, -122.4039444)\n\
8 | Flurry 3060 3rd St, SF (37.7507903, -122.3877184)\n\
9 | New Relic 188 Spear St, SF (37.7914417, -122.3927229)\n\
10 | Glassdoor 1 Harbor Drive, Sausalito (37.8672841, -122.5010216)";

    var sf_coords = [];
    var markers = {};
    var lines = [];

    sf_coords_str_lines = sf_coords_str.split("\n");
    for (i = 0; i < sf_coords_str_lines.length; i++){
        var matches = sf_coords_str_lines[i].match(/(\d+) .*?\((\-*\d+\.*\d*),\s*(\-*\d+\.*\d*)\)/);
        sf_coords.push([parseInt(matches[1]), parseFloat(matches[2]), parseFloat(matches[3])]);
    }
    for (i = 0; i < sf_coords.length; i++){
        var point_name = "" + sf_coords[i][0];
        markers[point_name] = new MarkerWithLabel({
            position: new google.maps.LatLng(sf_coords[i][1], sf_coords[i][2]),
            map: google_map,
            labelContent: point_name
//            labelClass: "labels", // the CSS class for the label
//            labelStyle: {opacity: 0.75}
        });
    }
    var right_order = ["1", "3", "2", "5", "6", "4"];
    for (i = 0; i < right_order.length - 1; i++){
        var line = new google.maps.Polyline({
            path: new Array(markers[right_order[i]].getPosition(),markers[right_order[i+1]].getPosition()),
            strokeColor: '#ff0000',
            strokeOpacity: 1.0,
            strokeWeight: 2
        });
        line.setMap(google_map);
    }

});

</script>