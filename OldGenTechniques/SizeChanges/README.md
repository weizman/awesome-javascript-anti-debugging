# SizeChanges

### POC

```javascript
const widthThreshold = window.outerWidth - window.innerWidth > threshold;
const heightThreshold = window.outerHeight - window.innerHeight > threshold;
const orientation = widthThreshold ? 'vertical' : 'horizontal';
```
### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x05-devtools-detection-ii-size-changes) [[J. M. Fernández](https://x-c3ll.github.io)]
