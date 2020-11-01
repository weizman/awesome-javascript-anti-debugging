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
    if ('#test1test2test3test4' !== getCallStack()) alert('flow of execution was tampered!')
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

### About

The idea here is to test the integrity of the flow of execution "on the fly" and to pick the next behaviour based on it.
Normally, if calling `getCallStack()` outputs something different than expected, it probably means someone has been playing around with the code.

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x07-implicit-control-of-flow-integrity) [[J. M. Fernández](https://x-c3ll.github.io)]
