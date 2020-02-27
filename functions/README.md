# Functions

### Articles

|  |  |  |
| :--- | :--- | :--- |
| [What is hoisting in vanilla JavaScript?](https://gomakethings.com/what-is-hoisting-in-vanilla-javascript/?mc_cid=1303dffebc&mc_eid=e9174ba77f) | 1/22/2020 | 1/22/2020 |
| [Callbacks in JavaScript](https://zellwk.com/blog/callbacks/?ck_subscriber_id=420572458) | 1/8/2020 | 1/8/2020 |
| [Arrow function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) |  |  |

### Methods

|  |  |
| :--- | :--- |
| .apply\(\) |  |
| .bind\(\) | returns copy of function where `this` is set to the first argument passed into `.bind()` |
| .call\(\) |  |

### `Hoisting` 

variable declarations  && function declaration, `hoisted` or moved to the top of the file

### `Closure`

A **closure** is the combination of a function bundled together \(enclosed\) with references to its surrounding state \(the **lexical environment**\). In other words, a closure gives you access to an outer function’s scope from an inner function. In JavaScript, closures are created every time a function is created, at function creation time.

![](../.gitbook/assets/screen-shot-2019-12-16-at-11.20.52-am.png)

{% code title="Function definition" %}
```javascript
function functionName(parameter = 'default value') { //scope start
  const functionBody = 'do something';
  return functionBody; //return statement
} //end scope

const capturedVal = functionName(0, arguments);
```
{% endcode %}

{% code title="Function types" %}
```javascript
/* ==============================
Regular function declaration
============================== */
function doctorize(firstName) {
  return `Dr. ${firstName}`;
}

/* ==============================
Anon function
============================== */
function (firstName) {
  return `Dr. ${firstName}`;
}

/* ==============================
Function expression
============================== */
const doctorize = function (firstName) {
  return `Dr. ${firstName}`;
}

/* ==============================
Arrow function
============================== */
const inchesToCM = inches => inches *2.54;

//function inchToCM() {
// const cm = inches * 2.54;
// return cm;
//}

/* ==============================
IIFE
immediately invoked function expression
============================== */
(function() {
  console.log('Running the Anon function');
return;
})();

/* ==============================
Methods!!!
============================== */
const wes = {
  name: 'Wes Bos',
  //Method!
  sayHi: function() {
    console.log('Hey Wes');
    return 'Hey Wes';
  },
  //Shorthand method
  yellHi() {
    console.log('HEY WESSSSS');
  },
  //arrow function
  whisperHi: () => {
    console.log('heeyyy wess');
  }
}

/* ==============================
Callback Functions
============================== */
//Click Callback
const button = document.querySelector('.clickMe');

function handleClick() {
  console.log('Great Clicking!!!');
}

button.addEventListener('click', handleClick);

//Timer Callback
setTimeout(function() {
  console.log('DONE! Time to eat!!');
}, 1000);

```
{% endcode %}

