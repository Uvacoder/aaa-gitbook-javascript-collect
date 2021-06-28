# Flow Control

### 2021

|  |  |
| :--- | :--- |
| [Automatically provided arguments in JavaScript callback functions](https://gomakethings.com/automatically-provided-arguments-in-javascript-callback-functions/) | 6/28 |
| [Learn callbacks, promises, Async/Await by Making Ice Cream 🍧🍨🍦](https://dev.to/joyshaheb/learn-callbacks-promises-async-await-by-making-ice-cream-4n76) | 6/24 |
| [How to structure asynchronous JavaScript with async and await](https://gomakethings.com/how-to-structure-asynchronous-javascript-with-async-and-await/) | 2/16 |
| [How to use async and await in vanilla JS](https://gomakethings.com/how-to-use-async-and-await-in-vanilla-js/) | 2/15 |
| [What is Zone.js in 5 Minutes](https://medium.com/javascript-in-plain-english/what-is-zone-why-zone-8534350480dd) | 1/29 |
| [The for...of loop in vanilla JS](https://gomakethings.com/the-for...of-loop-in-vanilla-js/) | 1/22 |

### 2020

|  |  |
| :--- | :--- |
| [5 ways to refactor if/else statements in JS functions](https://dev.to/sylwiavargas/5-ways-to-refactor-if-else-statements-in-js-functions-208e?utm_source=digest_mailer&utm_medium=email&utm_campaign=digest_email) | 11/19 |
| [Conditional JavaScript for Experts](https://medium.com/hackernoon/conditional-javascript-for-experts-d2aa456ef67c) | 10/3 |
| [Run a function after a specified amount of time using vanilla JS](https://gomakethings.com/run-a-function-after-a-specified-amount-of-time-using-vanilla-js/?mc_cid=42651963cd&mc_eid=[UNIQID]) | 7/26 |
| [How to run a function repeatedly at a desired interval using vanilla JS](https://gomakethings.com/how-to-run-a-function-repeatedly-at-a-desired-interval-using-vanilla-js/?mc_cid=91a5e0a1b8&mc_eid=[UNIQID]) | 7/12 |
| [The nullish coalescing operator in vanilla JS \(sorry, the what now?\)](https://gomakethings.com/the-nullish-coalescing-operator-in-vanilla-js-sorry-the-what-now/?mc_cid=847da65dd5&mc_eid=[UNIQID]) | 6/30 |
| [Optional chaining in vanilla JS](https://gomakethings.com/optional-chaining-in-vanilla-js/?mc_cid=d4f6bcc5d0&mc_eid=[UNIQID]) | 6/29 |
| [Cache API in JavaScript](https://medium.com/javascript-dots/cache-api-in-javascript-644380391681) | 6/4 |
| [Stop Putting So Many If Statements in Your JavaScript](https://medium.com/better-programming/stop-putting-so-many-if-statements-in-your-javascript-3b65aaa4b86b) | 5/24 |
| [JavaScript setTimeout Tutorial](https://www.freecodecamp.org/news/javascript-sleep-wait-delay/) | 5/6 |
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

//optional chaining
let house = wizards.harry?.house.toLowerCase() ?? 'hufflepuff';
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

