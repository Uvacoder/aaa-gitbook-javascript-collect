# Modules

|  |  |
| :--- | :--- |
| [How to bundle ES modules with rollup.js](https://gomakethings.com/how-to-bundle-es-modules-with-rollup.js/) | 12/3 |
| [Scoping with vanilla JS ES modules](https://gomakethings.com/scoping-with-vanilla-js-es-modules/) | 12/2 |
| [How to define a default export with vanilla JS ES modules](https://gomakethings.com/how-to-define-a-default-export-with-vanilla-js-es-modules/) | 12/1 |
| [An intro to import and export with ES modules](https://gomakethings.com/an-intro-to-import-and-export-with-es-modules/) | 11/30 |

|  |  |
| :--- | :--- |
| export |  |
| [import](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import) | The static **`import`** statement is used to import bindings which are exported by another module. Imported modules are in [`strict mode`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode) whether you declare them as such or not. The `import` statement cannot be used in embedded scripts unless such script has a `type="module"`. |

{% code title="html" %}
```javascript
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Currency Converter</title>
  <link rel="stylesheet" href="../../base.css">
  <link rel="stylesheet" href="./money.css">
</head>

<body>
  <div class="app">
    <form>
      <input type="number" name="from_amount">
      <select name="from_currency">
        <option>Select a Currency</option>
      </select>
      <p>in</p>
      <select name="to_currency">
        <option>Select a Currency</option>
      </select>
      <p>is</p>
      <p class="to_amount">$0</p>
    </form>
  </div>
  <script src="./money.js" type="module"></script>
</body>

</html>

```
{% endcode %}

```javascript
const last = 'bos';
const middle = 'slam dunk';

export function returnHi(name) {
  return `hi ${name} ${last}`;
}
const first = 'wes';
// NAMED exports - we can have as many as we want
export { last, middle };
export default first;

```

```javascript
import first, { returnHi as sayHi, last, middle } from './utils.js';
import * as everything from './wes.js';
import { handleButtonClick } from './handlers.js';

const button = document.querySelector('button');

button.addEventListener('click', handleButtonClick);

```

