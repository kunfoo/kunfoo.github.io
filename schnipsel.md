# Schnipsel

## openssl
- `openssl x509 -in /tmp/cert.der -inform der -text -noout`
- `openssl x509 -in /tmp/cert.der -inform der -outform pem -out /tmp/cert.pem`
- `openssl rsa -in /tmp/key.der -inform der -check -noout -text`

## adb
- `adb shell am stack list`
- `adb shell 'su -c /data/local/tmp/frida-server -D'`

## misc
- `iconv -f utf-16 -t utf-8 $FILE`
  - convert utf-16 encoded file to utf-8
- `podman run -it ubuntu`
- `mount.cifs //$HOST/$SHARE /$MNT/$POINT -o user=$USER,uid=1000`
- `mount -t nfs $HOST:/$SHARE /$MNT/$POINT
- `gpg -c --cipher-algo AES256 $FILE`
- `echo 100 | sudo tee /sys/class/backlight/amdgpu_bl0/brightness`
- `pandoc -t slidy -o presentation.html -s presentation.md`

## xrandr
- `cvt 1920 1080 60`
- `xrandr --newmode 1920x1080 173.00 1920 2048 2248 2576 1080 1083 1088 1120 -hsync +vsync`
- `xrandr --addmode Virtual1 1920x1080`
- `xrandr --output Virtual1 --mode 1920x1080`

## jq
- `jq -r '.[].ip' foo.json`
  - get field "ip" from json-formatted data

## grep
- `grep -v -f file1 file2`
  - find lines in file2 that are not in file1

## awk
- `awk -F ',' '{ print $1 "\t" $NF}'`
  - print the first and the last column, separated by tab, use field separator ","

## find
- `find . -perm -a+w -type d,f -ls`
  - find and list world-writable files and directories in cwd and subdirectories

- `find /usr -type f \( -perm -04000 -o -perm -02000 \)`
  - find suid/sgid executables in /usr and subdirectories

## tmux
- `tmus -S $SESSION ls`
  - list tmux sessions on socket $SOCKET as defined by byobu -S $SESSION
- `tmus -S $SESSION attach -t $NUM`
  - attach to tmux session $NUM on socket $SOCKET
