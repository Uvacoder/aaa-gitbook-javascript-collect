# Modules

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

