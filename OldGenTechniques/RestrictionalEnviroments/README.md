# RestrictionalEnviroments

### POC

```javascript
if (location.hostname === "localhost" || location.hostname === "127.0.0.1" || location.hostname === "") {
    console.log("Don't run me here!")
}
try { 
   console.log(window); 
} catch(e){ 
   console.log("NodeJS detected!!!!"); 
}
 
```

### About

The idea here is to prevent execution of code on local/non-browser environments (this is less about anti debugging and more about environmental restrictions)

### Resources

- [Original explanation](https://x-c3ll.github.io/posts/javascript-antidebugging/#0x0b-restrictional-enviroments) [[J. M. Fernández](https://x-c3ll.github.io)]
