# Networking Reference
*Linux Debian / Raspbian, otherwise noted

#### Get machine's MAC addresses

```ip link``` or ```ip address```

- lo: points to own host
- eth: ethernet link
- wifi: WIFI link

#### Get machine's MAC and IP addresses

```ip address```

- lo: points to own host
- eth: ethernet link
- wifi: WIFI link

#### Get radio devices

```
rfkill list all
rfkill block 0
rfkill unblock 0
```

#### Get wireless connection info

```iwlist wlan0 scan |less```

#### Get WAPs nearby into file

```sudo iwlist wlan0 scanning | egrep 'Cell|Encryption|Quality|Last beacon|ESSID' >> waps```

#### Put up/down a link

```
ip link
sudo ip link set wlan0 up
```
