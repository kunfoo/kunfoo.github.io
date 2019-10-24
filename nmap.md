# nmap
- do a syn scan and version scan of all tcp ports on hosts listed in list.txt
```
nmap -sS -sV -p0-65535 -iL list.txt
```

- run all ms-sql scripts
  - scripts are located in `/usr/share/nmap/scripts/`
```
nmap --script \*ms-sql\* -p 1433 some.host.tld
```

## performance tuning
- decrease retries, if a probe times out (default 10, or if _magic_ applies only 1)
```
--max-retries 2
```
