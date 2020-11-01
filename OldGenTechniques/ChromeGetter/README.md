# ChromeGetter

### POC

```javascript
let div = document.createElement('div');
console.log(div);
Object.defineProperty(div, "id", {get: () => { alert("Dev Tools detected!"); }});
```

### About

The idea here is to manipulate the way Chrome devtools work to tell whether it is activated or not.
When Chrome Devtools want to present info about a certain element, they usually call the element's different getters in order to obtain that info.
So for example, in order to get the element's id, its getter is called by the devtools. 
The trick here is to console log an element that was never passed globaly under window in any way and that can only be accessed by the code that created it, meaning the only entity that can call its id getter would be the devtools itself when the element is being logged to the console.
So by hooking the getter, we can write some javascript code that will only be executed when that id getter is called. 
And that way we'd know for certain when the devtools were activated.

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x04-devtools-detection-i-chrome-getter) [[J. M. Fernández](https://x-c3ll.github.io)]
