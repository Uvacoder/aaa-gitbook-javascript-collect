# Flow Control

|  |  |
| :--- | :--- |
| [The delay on setTimeout\(\) and setInterval\(\) is just a suggestion](https://gomakethings.com/the-delay-on-settimeout-and-setinterval-is-just-a-suggestion/?mc_cid=a64b101c23&mc_eid=[UNIQID]) | 4/15 |
| [What the heck is the event loop anyway? \| Philip Roberts \| JSConf EU](https://www.youtube.com/watch?v=8aGhZQkoFbQ) | 2/21 |

|  |  |
| :--- | :--- |
| Control Flow | is in computer science the order that the instructions or statements or functions are executed. |
| Event Loop | Continuously checks if the call stack is empty before adding callback queue functions |

```javascript
//ternary
// 1. Condition
// 2. what to do if true
// 3. what to do if false
const word = count === 1 ? 'item' : 'items';

//if else statement
let word;
if (count === 1) {
  word = 'item';
} else {
  word = 'items';
}
```

```javascript
//switch
      switch (event.key) {
        case 'ArrowUp':
          y = y - 1;
          rotate = -90;
          break;
        case 'ArrowDown':
          y = y + 1;
          rotate = 90;
          break;
        case 'ArrowLeft':
          x = x - 1;
          rotate = 0;
          flipped = true;
          break;
        case 'ArrowRight':
          x = x + 1;
          rotate = 0;
          flipped = false;
          break;
        default:
          console.log('That is not a valid move');
          break;
```

|  |  |
| :--- | :--- |
| .clearInterval\(\) |  |
| .clearTimeout\(\) |  |
| .setInterval\(\) |  |
| [.setTimeout\(\)](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setTimeout) |  |
|  |  |

{% code title="promise" %}
```javascript
    function makePizza(toppings = []) {
      return new Promise(function (resolve, reject) {
        // reject if people try with pineapple
        if (toppings.includes('pineapple')) {
          reject('Seriously? Get out 🍍');
        }
        const amountOfTimeToBake = 500 + (toppings.length * 200);
        // wait 1 second for the pizza to cook:
        setTimeout(function () {
          // when you are ready, you can resolve this promise
          resolve(`Here is your pizza 🍕 with the toppings ${toppings.join(' ')}`);
        }, amountOfTimeToBake);
        // if something went wrong, we can reject this promise;
      });
    }
    
        makePizza(['pepperoni'])
      .then(function (pizza) {
        console.log(pizza);
        return makePizza(['ham', 'cheese']);
      })
      .then(function (pizza) {
        console.log(pizza);
        return makePizza(['hot peppers', 'onion', 'feta']);
      })
      .then(function (pizza) {
        console.log(pizza);
        return makePizza(['pineapple']);
      })
      .then(function (pizza) {
        console.log(pizza);
        return makePizza(['one', 'two', 'three', 'four', 'one', 'two', 'three', 'four', 'one', 'two', 'three', 'four']);
      }).then(pizza => {
        console.log('All done! here is your last pizza');
        console.log(pizza);
      })
      .catch(handleError)
      
      //catch handle error
      function handleError(err) {
      console.log('Ohh noooo!!');
      console.log(err);
    }

    makePizza(['cheese', 'pineapple'])
      .then(pizza => {
        console.log(pizza);
      }).catch(handleError)
```
{% endcode %}

{% code title="async/await" %}
```javascript
    function wait(ms = 0) {
      return new Promise((resolve) => {
        setTimeout(resolve, ms);
      })
    }

    async function go() {
      console.log('Starting');
      await wait(2000);
      console.log('running');
      await wait(200);
      console.log('ending');
    }
```
{% endcode %}

### [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

|  |  |
| :--- | :--- |
| [async](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function) | The **`async function`** declaration defines an **asynchronous function** — a function that returns an [`AsyncFunction`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/AsyncFunction) object. Asynchronous functions operate in a separate order than the rest of the code via the [event loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop), returning an implicit [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) as its result. But the syntax and structure of code using async functions looks like standard synchronous functions. |
| [await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await) | The `await` operator is used to wait for a [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise). It can only be used inside an [`async function`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function). |
| [.all\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all) | The **`Promise.all()`** method returns a single [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) that fulfills when all of the promises passed as an iterable have been fulfilled or when the iterable contains no promises or when the iterable contains promises that have been fulfilled and non-promises that have been returned. It rejects with the reason of the first promise that rejects, or with the error caught by the first argument if that argument has caught an error inside it using try/catch/throw blocks. |
| [.allSettled\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/allSettled) | The **`Promise.allSettled()`** method returns a promise that resolves after all of the given promises have either resolved or rejected, with an array of objects that each describes the outcome of each promise. |
| [.catch\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/catch) | The **`catch()`** method returns a [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) and deals with rejected cases only. It behaves the same as calling [`Promise.prototype.then(undefined, onRejected)`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/then) \(in fact, calling `obj.catch(onRejected)` internally calls `obj.then(undefined, onRejected)`\). This means that you have to provide an `onRejected` function even if you want to fall back to an `undefined` result value - for example `obj.catch(() => {})`. |
| [.race\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/race) | The **`Promise.race()`** method returns a promise that fulfills or rejects as soon as one of the promises in an iterable fulfills or rejects, with the value or reason from that promise. |
| [.then\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/then) | The **`then()`** method returns a [`Promise`](https://developer.mozilla.org/en-US/docs/Web/API/Promise). It takes up to two arguments: callback functions for the success and failure cases of the `Promise`. |
| [try...catch](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch) | The **`try...catch`** statement marks a block of statements to try and specifies a response should an exception be thrown. |

