# SizeChanges

### POC

```javascript
const threshold = 160;
const widthThreshold = window.outerWidth - window.innerWidth > threshold;
const heightThreshold = window.outerHeight - window.innerHeight > threshold;
const orientation = widthThreshold ? 'vertical' : 'horizontal';
if (widthThreshold || heightThreshold) alert('devtools activated!');
```

### About

The idea here is to tell whether the devtools are active or not by the difference between the outer width/height of the window and the inner width/height.
If it is bigger than a certain threshold, it probably means that some of the window's space is taken by the devtools, meaning their open.

### Resources

- [Original explanation](https://github.com/sindresorhus/devtools-detect) [[sindresorhus](https://twitter.com/sindresorhus)]
- [Demo Site](https://sindresorhus.com/devtools-detect/) [[sindresorhus](https://twitter.com/sindresorhus)]
