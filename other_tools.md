# Other tools
## awk
- print the first and the last column, separated by tab, use field separator ","
```
awk -F ',' '{ print $1 "\t" $NF}'
```

## find
- find and list world-writable files and directories in cwd and subdirectories
```
find . -perm -a+w -type d,f -ls
```

- find suid/sgid executables in /usr and subdirectories
```
find /usr -type f \( -perm -04000 -o -perm -02000 \)
```

## screen

## not so frequently used
- paste
- shuf
