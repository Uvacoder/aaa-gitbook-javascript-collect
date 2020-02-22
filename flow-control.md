# Flow Control

|  |  |
| :--- | :--- |
| Control Flow | is in computer science the order that the instructions or statements or functions are executed. |

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

|  |  |
| :--- | :--- |
| [What the heck is the event loop anyway? \| Philip Roberts \| JSConf EU](https://www.youtube.com/watch?v=8aGhZQkoFbQ) | 2/21 |

