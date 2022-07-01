# Networking
- ip
- ncat
- socat

## IPv6
- Link-local scope multicast all nodes address
  - ff02::1
  - `ping -6 ff02::1%eth0`

## curl
- resolve ccc.de to localhost address and don't check certificate
```
# curl --resolve ccc.de:443:127.0.0.1 -k https://ccc.de
```

## iptables

- list all chains
```
# iptables -L | grep Chain
```

- list all rules of the INPUT chain
```
# iptables -n -L INPUT
or
# iptables -S INPUT
```

- list rules of the FORWARD chain with line numbers and packet counters
```
# iptables -n -v --line-numbers -L FORWARD
# iptables -vnL FORWARD --line-numbers
```

- delete rule 23 in FORWARD chain
```
# iptables -D FORWARD 23
```

- reset packet counter for rule 42 in INPUT chain
```
# iptables -Z INPUT 42
```

- delete all rules in the OUTPUT chain (flush)
```
# iptables -F OUTPUT
```

## nft

- list all rules
```
# nft list ruleset
```

## ssh
- make remote port 1337 accessible on port 8080 on local side and go to
  background (do not present a remote shell)
```
ssh -NfL 8080:localhost:1337 user@host.tld
```

- run tcpdump on remote host and pipe traffic to local wireshark instance
```
ssh user@host sudo tcpdump -i wlan0 -w - | wireshark -k -i -
```
