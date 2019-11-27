# ssh
- make remote port 1337 accessible on port 8080 on local side and go to
  background (do not present a remote shell)
```
ssh -NfL 8080:localhost:1337 user@host.tld
```

- run tcpdump on remote host and pipe traffic to local wireshark instance
```
ssh user@host sudo tcpdump -i wlan0 -w - | wireshark -k -i -
```
