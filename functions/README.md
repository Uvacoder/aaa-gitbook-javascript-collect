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

```javascript
//normal function
function doctorize(firstName) {
  return `Dr. ${firstName}`;
}

//anon function
function (firstName) {
  return `Dr. ${firstName}`;
}

//function expression
const doctorize = function (firstName) {
  return `Dr. ${firstName}`;
}

```

> >

