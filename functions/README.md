# Functions

### Articles

|  |  |
| :--- | :--- |
| [Arrow function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) |  |

### Methods

|  |  |
| :--- | :--- |
| .apply\(\) |  |
| .bind\(\) | returns copy of function where `this` is set to the first argument passed into `.bind()` |
| .call\(\) |  |

|  |  |
| :--- | :--- |
| [Math.floor\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/floor) |  |
| Math.round\(\) |  |
| Math.ceil\(\) |  |
| Math.max\(\) |  |
| parseFloat\(\) |  |

|  |  |
| :--- | :--- |
| Date.now\(\) |  |

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
  }
  //Shorthand method
  yellHi() {
    console.log('HEY WESSSSS');
  }
  //arrow function
  whisperHi: () => {
    console.log('heeyyy wess');
  }
}
```
{% endcode %}

