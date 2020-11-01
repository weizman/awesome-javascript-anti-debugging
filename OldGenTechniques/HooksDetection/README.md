# HooksDetection

### POC

```javascript
if (document.createElement.toString() !== 'function createElement() { [native code] }') {
    console.log("hook detected!");
}
else {
    alert('steal cookies!');
}
```

### About

The idea here is to tell when someone tried to place a hook on the protected code in order to investigate it, and if so to give up on running.

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x0a-proxy-objects) [[J. M. Fernández](https://x-c3ll.github.io)]
