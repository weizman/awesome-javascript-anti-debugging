# Chromium Shadow Root Abuse

### POC

```html
<a href="?disable">disable poc</a>
<br>
<a href="?enable">enable poc</a>
<script>
const enabled = location.href.includes('disable');

(function() {
    const ifr = document.body.appendChild(document.createElement('iframe'));
    const template = ifr.contentWindow.document.createElement('html');
    !enabled && ifr.remove();
    template.innerHTML = `<my-element><template shadowroot="open"></template></my-element>`;
    const shadow = template.children[1].children[0].children[0];
    console.log(shadow);
})();
</script>
```
### Resources

- [Live DEMO!](https://weizmangal.com/awesome-javascript-anti-debugging/NewGenTechniques/ChromiumShadowRootAbuse/poc.html)
- [Bug report](https://bugs.chromium.org/p/chromium/issues/detail?id=1465129)
