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
