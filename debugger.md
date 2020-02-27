# Debugger

|  |  |
| :--- | :--- |
| [CORS](https://developer.mozilla.org/en-US/docs/Glossary/CORS-safelisted_response_header) | A _CORS-safelisted response header_ is an [HTTP header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers) which has been safelisted so that it will not be filtered when responses are processed by CORS, since they're considered _safe_ \(as the headers listed in [`Access-Control-Expose-Headers`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Expose-Headers)\). By default, the safelist includes the following response headers: |
| CORS Proxy | [https://cors-anywhere.herokuapp.com/](https://cors-anywhere.herokuapp.com/) |
| [regeneratorRuntime](https://stackoverflow.com/questions/33527653/babel-6-regeneratorruntime-is-not-defined) | [https://github.com/browserslist/browserslist](https://github.com/browserslist/browserslist) |

{% code title="package.json" %}
```javascript
{
  "name": "dogrecipes",
  "version": "1.0.0",
  "description": "",
  "main": "scripts.js",
  "scripts": {
    "start": "parcel index.html"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "parcel-bundler": "^1.12.4"
  },
  "browserslist": [
    "last 1 chrome versions"
  ]
}

```
{% endcode %}

