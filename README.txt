OVERVIEW

The 'show fabric' command shows you statistics and the status of the uplinks and BGP peerings. 
It is programmed to be consumend by IP fabrics that are based on eBGP (between Spine/Leaf as IGP) and iBGP EVPN. 
Therefore it requires some inputs to discover your uplinks and BGP peerings. 

HOW TO GET AND SET SHOW FABRIC CLI PLUGIN INTO YOUR SR LINUX

1) Get the CLI Plugin with the get/set/delete scripts.This will run the get and set scripts consequently.
   (DNS server-list configuration is needed in SR Linux)

   bash <(curl -sL https://raw.githubusercontent.com/aaakpinar/show-fabric/refs/heads/main/get-show-fabric.sh)

2) Add the uplink subinterfaces (or a pattern that is common in uplink SUBINTERFACE description) and eBGP/iBGP(RR) peer group names after running above command or separately with set-show-fabric.sh script. The script will get you the SR Linux CLI.

3) Try 'show fabric' commands.

Enjoy!

-Alperen
