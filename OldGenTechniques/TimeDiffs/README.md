# TimeDiffs

### POC

```javascript
var startTime = performance.now();
startMaliciousCode();
var stopTime = performance.now();
if ((stopTime - startTime) > 1000) {
    alert("Debugger detected!")
}
```
### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x03-differences-of-time) [[J. M. Fernández](https://x-c3ll.github.io)]
