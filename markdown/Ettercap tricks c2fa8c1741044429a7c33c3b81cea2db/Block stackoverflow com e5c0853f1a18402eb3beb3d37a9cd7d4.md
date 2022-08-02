# Block stackoverflow.com

- If installed using homebrew:

Open `/opt/homebrew/etc/ettercap/etter.dns` file

- If installed using other tools:

Open `/etc/ettercap/etter.dns` file

Add the following contents

```
stackoverflow.com A 172.217.24.228
*.stackoverflow.com A 172.217.24.228
```

172.217.24.228 is the IP of google, google will automatically detect dns spoofing and block the access

Run the following command

`sudo ettercap -T -q -i en0 -P dns_spoof -P autoadd -M arp:remote /192.168.1.1// ///`

192.168.1.1 is the router IP address