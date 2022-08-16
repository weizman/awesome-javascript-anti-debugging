# Obfuscation

### About

Obfuscation is just another anti debugging technique, that has so much into to it that it can be considered as a field of its own rather than "just" a technique.

The idea is to take some javascript source code and mess it up as much as possible without changing its original logic whatsoever, so it would serve the same purpose as before but would be much harder to read and understand.

What's usually done on the basic level is changing variables names, minifying the code, scrambling strings and so on, but javascript obfuscation can be much more than that.

### Relation to Anti Debugging

Making the code as not readable as possible is a method of anti debugging of itself. 
Also, common obfuscators usually implement some of the old-gen anti debugging techniques that are listed in this **awesome** repo.

### Obfuscators

There are many tools out there that do code obfuscation. Here are some:

#### Free

```javascript
// Sample javascript to obfuscate
function hi() {
  console.log("Hello World!");
}
hi();
```

- [obfuscator.io](https://obfuscator.io/)

```javascript
var _0x22e1=['log','Hello\x20World!'];(function(_0x54a82c,_0x22e133){var _0x52d59f=function(_0x37d3b5){while(--_0x37d3b5){_0x54a82c['push'](_0x54a82c['shift']());}};_0x52d59f(++_0x22e133);}(_0x22e1,0x78));var _0x52d5=function(_0x54a82c,_0x22e133){_0x54a82c=_0x54a82c-0x0;var _0x52d59f=_0x22e1[_0x54a82c];return _0x52d59f;};function hi(){var _0xf2ec74=_0x52d5;console[_0xf2ec74('0x0')](_0xf2ec74('0x1'));}hi();
```

- [jsfuck](http://www.jsfuck.com/)

```javascript
[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]][([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+([][[]]+[])[+!+[]]+(![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[+!+[]]+([][[]]+[])[+[]]+([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+(!![]+[])[+!+[]]]((!![]+[])[+!+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+([][[]]+[])[+[]]+(!![]+[])[+!+[]]+([][[]]+[])[+!+[]]+(+[![]]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+!+[]]]+(!![]+[])[!+[]+!+[]+!+[]]+(+(!+[]+!+[]+!+[]+[+!+[]]))[(!![]+[])[+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+([]+[])[([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+([][[]]+[])[+!+[]]+(![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[+!+[]]+([][[]]+[])[+[]]+([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+(!![]+[])[+!+[]]][([][[]]+[])[+!+[]]+(![]+[])[+!+[]]+((+[])[([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+([][[]]+[])[+!+[]]+(![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[])[+!+[]]+([][[]]+[])[+[]]+([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+[]]+(!![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[+!+[]+[+[]]]+(!![]+[])[+!+[]]]+[])[+!+[]+[+!+[]]]+(!![]+[])[!+[]+!+[]+!+[]]]](!+[]+!+[]+!+[]+[!+[]+!+[]])+(![]+[])[+!+[]]+(![]+[])[!+[]+!+[]])()((![]+[])[+!+[]]+(![]+[])[!+[]+!+[]]+(!![]+[])[!+[]+!+[]+!+[]]+(!![]+[])[+!+[]]+(!![]+[])[+[]]+([][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]]+[])[+!+[]+[!+[]+!+[]+!+[]]]+[+!+[]]+([+[]]+![]+[][(![]+[])[+[]]+(![]+[])[!+[]+!+[]]+(![]+[])[+!+[]]+(!![]+[])[+[]]])[!+[]+!+[]+[+[]]])
```

- [javascriptobfuscator](https://javascriptobfuscator.com/Javascript-Obfuscator.aspx)

```javascript
var _0xb3cd=["\x48\x65\x6C\x6C\x6F\x20\x57\x6F\x72\x6C\x64\x21","\x6C\x6F\x67"];function hi(){console[_0xb3cd[1]](_0xb3cd[0])}hi()
```

#### Paid

- [jscrambler](https://jscrambler.com/)

### References

- [javascript obfuscators introduction](https://www.youtube.com/watch?v=4dxPizOvM8g) [by JSScrambler CTO [Pedro Fortuna](https://twitter.com/pedrofortuna)]
