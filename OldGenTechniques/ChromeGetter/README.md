# ChromeGetter

### POC

```javascript
let div = document.createElement('div');
console.log(div);
Object.defineProperty(div, "id", {get: () => { alert("Dev Tools detected!"); }});
```
### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x04-devtools-detection-i-chrome-getter) [[J. M. Fernández](https://x-c3ll.github.io)]
