### Steps

1. Install Tor 
  sudo apt-get install tor  

2. Check status and start if need be 
  sudo service tor status/start

3. Locate proxychains4.conf file
  locate proxychains4.conf
  
4. Change the configuration:
  - Enable dynamic mode
  - uncomment proxy_dns
  - add sock5 ip at last

5. Test it
  - proxychain firefox google.com
  - go to iplocation.com and check your location


### Extras

Can also be tried with nmap to enhance anonymity.  
Eg. proxychains nmap 192.168.1.120



