# Chromium Devtools Scope Pane

### POC

```javascript
function malicious() {
    const detect = (function(){
        const dummy = /./;
        dummy.toString = () => {
            alert('someone is debugging the malicious function!');
            return 'SOME_NAME';
        };
        return dummy;
    }());

    // do a malicious action
    if (window.stealUserCookies) window.stealUserCookies();
}

function legit() {
    // do a legit action
    return 1 + 1;
}

function main() {
    legit();
    malicious();
}

debugger;
main();
```
### Resources

- [Original research and fully detailed explanation](https://weizman.github.io/website/?javascript-anti-debugging-some-next-level-shit-part-2) [[Gal Weizman](https://weizman.github.io/website)]
- [Demo site](https://debug-tracker.ue.r.appspot.com/) [[Gal Weizman](https://weizman.github.io/website)]
