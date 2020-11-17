# Promises

|  |  |
| :--- | :--- |
| [Best of Modern JavaScript — Async and Promises](https://medium.com/javascript-in-plain-english/best-of-modern-javascript-async-and-promises-38711c834d02) | 11/17 |
| [JavaScript \| Promises](https://www.geeksforgeeks.org/javascript-promises/) |  |

```javascript
return new Promise((resolve, reject) => {
  functionWithCallback((err, result) => {
   return err ? reject(err) : resolve(result);
  });
});
```

|  |  |
| :--- | :--- |
| try |  |
| catch |  |
|  |  |

global memory &gt; execution context &gt; event loop

event loop = callstack &gt; microtask queue \(promises .then\(\)\) &gt; callback queue \(setTimeout\(f, 0\)\)

