# frida
## Android

## iOS
- get an array of all object instances of class NSString
```
a = ObjC.chooseSync(ObjC.classes.NSString)
```

- call a static method
```
ObjC.classes.Class['- method']()
```

## Useful JavaScript
- test if object is an array-type
```
Array.isArray(obj)
```
