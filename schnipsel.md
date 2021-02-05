# Schnipsel

## openssl
```openssl x509 -in /tmp/cert.der -inform der -text -noout```
```openssl x509 -in /tmp/cert.der -inform der -outform pem -out /tmp/cert.pem```
```openssl rsa -in /tmp/key.der -inform der -check -noout -text```

## adb
```adb shell am stack list```
```adb shell 'su -c /data/local/tmp/frida-server -D'```

