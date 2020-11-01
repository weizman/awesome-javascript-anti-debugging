# CodeIntegrity

### POC

```javascript
function hashCode (s) {
    var hash = 0;
    if (s.length == 0) {
        return hash;
    }
    for (var i = 0; i < s.length; i++) {
        var char = s.charCodeAt(i);
        hash = ((hash<<5)-hash)+char;
        hash = hash & hash; // Convert to 32bit integer
    }
    return hash;
}

function start() {
    alert('steal cookies!');
}

function main() {
    if (hashCode(start.toString()) !== -1968638942) return;
    start();
}

main()
```

### About

The idea here is to test the integrity of the code "on the fly" and expect the protected function's hash to not change.
If it changed it means the code has changed as well, probably for research purposes, and that means the protection of the code has been compromised.

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x08-implicit-control-of-code-integrity) [[J. M. Fernández](https://x-c3ll.github.io)]
