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
### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x0a-proxy-objects) [[J. M. Fernández](https://x-c3ll.github.io)]
