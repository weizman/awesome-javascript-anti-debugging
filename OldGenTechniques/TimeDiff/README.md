# TimeDiff

### POC

```javascript
var startTime = performance.now();
startMaliciousCode();
var stopTime = performance.now();
if ((stopTime - startTime) > 1000) {
    alert("Debugger detected!")
}
```

### About

The idea here is to measure time between two points in the code, preferably right before and right after the code that needs the anti debugging protection, and then based on the difference between the two tell whether the code is being debugged or not. 
If the difference was small enough, it means the code was executed with no interruptions.
But if the difference was unrealistically big, it probably means it was interrupted, most likely by a debugger.

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x03-differences-of-time) [[J. M. Fernández](https://x-c3ll.github.io)]
