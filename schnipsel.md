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
- `gpg -c --cipher-algo AES256 $FILE`

## xrandr
- `cvt 1920 1080 60`
- `xrandr --newmode 1920x1080 173.00 1920 2048 2248 2576 1080 1083 1088 1120 -hsync +vsync`
- `xrandr --addmode Virtual1 1920x1080`
- `xrandr --output Virtual1 --mode 1920x1080`
