# debugger;

### POC

```javascript
setInterval(() => {debugger;}, 100);
```

### About

The idea here is to create a state in which the code runs smoothly, but the devtools will get stuck when is activated. 
This can be achieved by running the POC above. 
`debugger;` statement is normally ignored by the browser when is interpreted, but when the devtools is activated, `debugger;` makes the devtools source code debugger to pause.
Calling `debugger;` in an infinite async interval will force the devtools to pause non-stop, which would make it a bit harder for researchers to debug other pieces of code in the website using the devtools.

### Resources
