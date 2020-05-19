# Promises

|  |  |
| :--- | :--- |
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

global memory &gt; execution context &gt; call stack &gt; microtask queue \(promises .then\(\)\) &gt; callback queue

