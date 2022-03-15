### Steps

1. sudo eth0 down
2. Try the following commands:  
  -  macchanger -m <new_MAC_address> eth0 (Specified Address)
  -  macchanger -r eth0 (Random address)
  -  macchanger -e eth0 (Change only serial number, keep vendor bytes intact)
  -  macchanger -p eth0 (Change to original address)  
3.  ifconfig eth0 up
