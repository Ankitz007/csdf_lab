#### To find Live hosts on a network
This scan is known as a Simple List that can help determine what is live on a particular network.  
**nmap -sL <network>**


#### To find and ping all Live hosts on a network
Nmap tries to ping all the addresses in the given network. Here -sn disbales nmap’s default behavior of attempting to port scan a host and simply has nmap try to ping the host.  
**nmap -sn <network>**

  
#### To find open ports on host
Nmap port scans specific hosts. These ports indicate listening services on a particular machine.  
**nmap <ip_address>**


#### To find services listening on ports on hosts
This is a service scan and used to determine the service that may be listening on a particular port on a machine. Nmap will probe all of the open ports and attempt to banner grab information from the services running on each port.  
**nmap -sV <ip_address>**


#### To find Anonymous FTP logins on hosts
Nmap takes a closer look at this particular port and sees what can be determined. By default nmap runs its default script -sC on the FTP port 21 on the host.  
**nmap -sC <ip_address> -p <port_number>**
