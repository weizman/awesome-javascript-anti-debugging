# SizeChanges

### POC

```javascript
function getCallStack() {
    var stack = "#", total = 0, fn = arguments.callee;
    while ( (fn = fn.caller) ) {
        stack = stack + "" +fn.name;
        total++
    }
    return stack
}
function test1() {
    console.log(getCallStack());
}
function test2() {
    test1();
}
function test3() {
    test2();
}
function test4() {
    test3();
}
test4();
```

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x07-implicit-control-of-flow-integrity) [[J. M. Fernández](https://x-c3ll.github.io)]
