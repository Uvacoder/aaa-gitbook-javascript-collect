# Modules

|  |  |
| :--- | :--- |
| export |  |
| [import](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import) | The static **`import`** statement is used to import bindings which are exported by another module. Imported modules are in [`strict mode`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode) whether you declare them as such or not. The `import` statement cannot be used in embedded scripts unless such script has a `type="module"`. |

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

