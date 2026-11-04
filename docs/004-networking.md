# Networking

The server is configured and tested using standard Linux networking tools.

Topics covered:
- Network interfaces
- IPv4 addressing
- Routing
- Default gateway
- DNS resolution
- TCP/UDP ports
- Network connectivity
- Network troubleshooting

### Tools:

```

ip
ss
ping
traceroute
dig
nslookup
curl

```

### Example troubleshooting workflow:

```

Application unavailable
        │
        ▼
Check network interface
        │
        ▼
Check IP configuration
        │
        ▼
Check routing
        │
        ▼
Check DNS
        │
        ▼
Check destination port
        │
        ▼
Check application/service

```

step 1: check ip

```
ip addr show

admin01@linux-server01:~$ ip addr show
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether xx:xx:xx:xx:xx:xx brd ff:ff:ff:ff:ff:ff
    altname enxXXXXXXXXXXXX
    inet 192.168.1.99/24 brd 192.168.1.255 scope global dynamic noprefixroute enp0s3
       valid_lft 1767sec preferred_lft 1767sec
    inet6 2001:db8::xxxx:xxxx:xxxx:xxxx/64 scope global temporary dynamic 
       valid_lft 86376sec preferred_lft 43176sec
    inet6 2001:db8::xxxx:xxxx:xxxx:xxxx/64 scope global dynamic mngtmpaddr noprefixroute 
       valid_lft 86376sec preferred_lft 43176sec
    inet6 fe80::xxxx:xxxx:xxxx:xxxx/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever

```

step 2: check routes

```
ip routes

default via 192.XXX.X.X dev enp0s3 proto dhcp src 192.XXX.X.XX metric 100 
XXX.XXX.X.0/XX dev enp0s3 proto kernel scope link src XXX.XXX.X.XX metric 100 

```

step 3: DNS test

```
dig google.com

nslookup google.com

ping -c 4 google.com

curl https://example.com

```
