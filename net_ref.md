# Networking Reference

#### Get machine's MAC addresses
*Linux*

```ip link``` or ```ip address```

- lo: points to own host
- eth: ethernet link
- wifi: WIFI link

#### Get machine's MAC and IP addresses
*Linux*

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
