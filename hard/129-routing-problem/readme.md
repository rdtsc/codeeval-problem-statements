<h2>Routing Problem</h2>

<h3>Challenge Description:</h3>
<p>
    A company has a network with H number of hosts. The network is customized according to the following rules:
</p>

<ol>
<li>Each host has 0 &lt;= K &lt;= 6 number of network interfaces (if there is no network interface, it means that a host is turned off).</li>
<li>
        Each interface is identified by an IP address and a subnet mask represented by CIDR notation (for example,
        192.168.0.1 is an IP address, 255.255.255.0 is a NetMask, 192.168.0.1/24 is an IP address in CIDR).
</li>
<li>
        Two hosts are on the same subnet if (IP_1 AND NetMask_1) = (IP_2 AND NetMask_2), where IP_i and NetMask_i
        are IP address and NetMask of the i-th computer, AND is a bitwise multiplication.
</li>
<li>A package between two hosts in the same subnet is transmitted directly.</li>
<li>
        A package between two hosts that are located in different subnets can be transmitted through the third host in
        case their interfaces are connected to both source and destination subnets (for example, Host 1 has interfaces
        in the subnets &quot;A&quot; and &quot;B&quot;, Host 2 has interfaces in the subnets &quot;B and C&quot;, Host 3 has an interface in the subnet
        &quot;C&quot;, Host 4 has an interface in the subnet &quot;A&quot;, so the package path from 1 to 3 is [1, 2, 3], from 1 to 4 is
        [1, 4], and from 3 to 4 is [3, 2, 1, 4]).
</li>
</ol>

<p>Your task is to find all the shortest paths for the package between two specified hosts.</p>

<h3>Input sample:</h3>
<p>
    Your program should accept a path to a filename as its first argument. The first line of the file contains IDs of hosts
    and IP addresses that belong to each host (for example,
    {ID_0: [&apos;IP address_1&apos;, &apos;IP address_K&apos;], ID_1: [], ID_H: [&apos;IP address_1&apos;, &apos;IP address_K&apos;]}),
    the other N lines are test cases. Each test case is a pair of host IDs (start_ID and end_ID) separated by a single space.
</p>

<pre class="description-input-output">{0: [&apos;179.177.220.225/23&apos;, &apos;77.119.202.216/26&apos;, &apos;171.251.60.138/25&apos;], 1: [&apos;147.105.101.114/22&apos;, &apos;67.239.38.194/23&apos;, &apos;50.202.182.215/21&apos;], 2: [&apos;14.125.37.194/23&apos;, &apos;128.3.0.158/23&apos;], 3: [&apos;77.119.202.193/26&apos;, &apos;164.119.164.209/30&apos;], 4: [&apos;178.102.37.7/25&apos;, &apos;117.184.65.161/21&apos;, &apos;246.255.201.77/20&apos;, &apos;128.160.69.237/30&apos;], 5: [&apos;67.239.38.85/23&apos;, &apos;128.3.1.67/23&apos;, &apos;19.136.96.193/20&apos;, &apos;108.243.129.176/24&apos;], 6: [&apos;103.131.199.252/25&apos;, &apos;222.15.10.40/20&apos;], 7: [&apos;194.214.45.144/20&apos;, &apos;22.53.223.185/26&apos;], 8: [&apos;147.105.102.57/22&apos;, &apos;122.119.95.62/22&apos;, &apos;0.111.125.205/30&apos;], 9: [&apos;0.111.125.206/30&apos;], 10: [&apos;117.184.70.222/21&apos;], 11: [&apos;178.102.37.31/25&apos;, &apos;19.136.100.54/20&apos;, &apos;96.43.12.49/28&apos;, &apos;214.240.75.20/23&apos;], 12: [&apos;171.251.60.130/25&apos;, &apos;198.240.92.134/22&apos;, &apos;242.183.157.69/27&apos;, &apos;235.172.192.119/23&apos;], 13: [&apos;122.119.93.84/22&apos;], 14: [&apos;128.160.69.238/30&apos;, &apos;22.53.223.131/26&apos;, &apos;89.111.130.102/30&apos;], 15: [&apos;50.202.182.148/21&apos;, &apos;235.172.192.12/23&apos;], 16: [&apos;179.177.220.149/23&apos;, &apos;103.131.199.146/25&apos;, &apos;198.240.92.1/22&apos;], 17: [&apos;96.43.12.52/28&apos;], 18: [&apos;164.119.164.210/30&apos;, &apos;108.243.129.104/24&apos;, &apos;222.15.4.215/20&apos;, &apos;89.111.130.101/30&apos;, &apos;63.113.177.19/28&apos;], 19: [&apos;14.125.36.203/23&apos;, &apos;246.255.204.239/20&apos;, &apos;194.214.34.254/20&apos;, &apos;214.240.74.123/23&apos;, &apos;242.183.157.93/27&apos;, &apos;63.113.177.27/28&apos;]}
5 8
1 7
2 14
11 20
10 14</pre>

<h3>Output sample:</h3>

<p>
    For each test case, print out the shortest path represented by a list of host IDs in the order from start_ID to end_ID.
    If there is no path, print out &quot;No connection&quot;.
</p>

<pre class="description-input-output">[5, 1, 8]
[1, 5, 2, 19, 7], [1, 5, 11, 19, 7], [1, 5, 18, 14, 7], [1, 5, 18, 19, 7], [1, 15, 12, 19, 7]
[2, 5, 18, 14], [2, 19, 4, 14], [2, 19, 7, 14], [2, 19, 18, 14]
No connection
[10, 4, 14]</pre>

<h3>Constraints:</h3>
<ol>
<li>H is in a range from 150 to 300.</li>
<li>ID is in a range from 0 to H &#x2013; 1.</li>
<li>K is in a range from 0 to 6.</li>
<li>N is in a range from 30 to 40.</li>
<li>IP address is in a range from 1.0.0.0 to 254.254.254.254.</li>
<li>NetMask is in a range from 20 to 30.</li>
</ol>

<p>
<b>Sorting example:</b>
<br>
    Please use the natural sorting in case there is more than one path. E.g.
    for the lists [1,1,2,3], [0,2,1,2], [1,1,2,2], [0,1,1,2] the output is [0,1,1,2], [0,2,1,2], [1,1,2,2], [1,1,2,3]
</p>