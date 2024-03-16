## Networking

Networking is an essential aspect of Linux system administration. Here are some basic networking commands that are useful for administrators:

### a. `ifconfig`

`ifconfig` is used to view network interfaces.

![ifconfig](/assets/ifconfig.png)

- `Eth0`: Ethernet (wired connection)
- `lo`: Loopback (local)
- `wlan0`: Wireless LAN

### b. `ping`

The `ping` command is a tool for diagnosing connectivity issues, monitoring network performance, and checking server availability.

![ping](/assets/ping.png)

### c. Interface up/down

Here's the process to bring a network interface up or down in Linux:

- To bring an interface down:
`$ sudo ifconfig <ethernet interface> down`

![interface-down](/assets/int-up-down.png)

- To bring an interface up:

`$ sudo ifconfig <ethernet interface> up`


![interface-up](/assets/int-up.png)

### d. `nslookup`

The `nslookup` command is used for querying the Domain Name System (DNS) to obtain name or IP address information. It’s a helpful tool for troubleshooting and diagnosing DNS-related issues.

Basic syntax of nslookup: `$ sudo nslookup <domain or IP address>`


![nslookup](/assets/nslookup.png)

### e. `traceroute`

The `traceroute` command is used to trace the route that packets take from our computer to a destination IP address. It provides information about the network hops between the source and destination.

Basic syntax: `$ sudo traceroute <domain or IP address>`


![traceroute](/assets/traceroute.png)

Here's the basic information of the output:
- `Hop number`: The leftmost column indicates the hop number (30) in the route.
- `Hostname or IP address`: The route starts from my local machine (192.168.123.254) to the final destination (142.250.207.206) which belongs to Google.
- `Latency`: The round-trip times vary at each hop, reflecting the network latency.







