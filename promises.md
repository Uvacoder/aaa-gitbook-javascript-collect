# Promises

{% embed url="https://www.geeksforgeeks.org/javascript-promises/" %}

```javascript
return new Promise((resolve, reject) => {
  functionWithCallback((err, result) => {
   return err ? reject(err) : resolve(result);
  });
});
```



