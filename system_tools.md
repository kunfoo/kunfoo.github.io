# System configuration
## Filesystem
- lsof

### ACLs
- getfacl/setfacl

### Capabilities
- ???

## Namespaces
- lsns
- nsenter

## Processes
List all processes, including the complete cmdline:
```
ps auxwww
```

Show processes as a tree:
```
ps faux
ps axjf
pstree
```

## misc
List alternatives for `editor`:
```
update-alternatives --list editor
```

Set `/usr/bin/vim.basic` as alternative for `editor`:
```
update-alternatives --set editor /usr/bin/vim.basic
```

## systemd
- schedule reboot at certain point in time
```
systemd-run --on-calendar="2023-01-01 01:00:00 UTC" systemctl reboot
```

## mdadm
- `mdadm --auto-detect`
- `mdadm --assemble --scan`
- `mdadm --detail /dev/md0`
