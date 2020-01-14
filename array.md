# Array

|  |  |  |
| :--- | :--- | :--- |
| [Five interesting ways \(and one boring way\) to use Array.reduce\(\)](https://gomakethings.com/five-interesting-ways-and-one-boring-way-to-use-array.reduce) | 12/19/2019 | 12/19/2019 |
| [13 useful Array tips and tricks](https://dev.to/duomly/13-useful-javascript-array-tips-and-tricks-you-should-know-2jfo) |  |  |
| [MDN Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) |  |  |

```javascript
//array literal
const names = [];

const names = new Array(); //longer way to create an array

//first items in arrays start at 0


```

|  |  |
| :--- | :--- |
| [.from\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from) | The **`Array.from()`** method creates a new, shallow-copied `Array` instance from an array-like or iterable object. |
| .isArray\(\) |  |
| [.of\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/of) | The Array.of\(\) method creates a new Array instance from a variable number of arguments, regardless of number or type of the arguments. |

### Methods

|  |  |
| :--- | :--- |
| .every\(\) |  |
| .flat\(\) |  |
| [.find\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find) | The **`find()`** method returns the **value** of the **first element** in the provided array that satisfies the provided testing function. |
| .findIndex\(\) |  |
| .fill\(\) |  |
| [.filter\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) | The **`filter()`** method **creates a new array** with all elements that pass the test implemented by the provided function. |
| [.forEach\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) | The **`forEach()`** method executes a provided function once for each array element. |
| [.includes\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/includes) | The **`includes()`** method determines whether an array includes a certain value among its entries, returning `true` or `false` as appropriate. |
| [.indexOf\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf) | The **`indexOf()`** method returns the first index at which a given element can be found in the array, or -1 if it is not present. |
| [.join\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join) | The **`join()`** method creates and returns a new string by concatenating all of the elements in an array \(or an [array-like object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections#Working_with_array-like_objects)\), separated by commas or a specified separator string. If the array has only one item, then that item will be returned without using the separator. |
| .keys\(\) |  |
| [.length](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/length) | The length property of an object which is an instance of type Array sets or returns the number of elements in that array. The value is an unsigned, 32-bit integer that is always numerically greater than the highest index in the array. |
| [.map\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) | The **`map()`** method creates a new array with the results of calling a provided function on every element in the calling array. |
| [.pop\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop) | The **`pop()`** method removes the **last** element from an array and returns that element. This method changes the length of the array. |
| [.push\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push) | The **`push()`** method adds one or more elements to the end of an array and returns the new length of the array. |
| [.reduce\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) | The **`reduce()`** method executes a **reducer** function \(that you provide\) on each element of the array, resulting in a single output value. |
| [.reverse\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse) | The **`reverse()`** method reverses an array [_in place_](https://en.wikipedia.org/wiki/In-place_algorithm). The first array element becomes the last, and the last array element becomes the first. |
| [.shift\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift) | The **`shift()`** method removes the **first** element from an array and returns that removed element. This method changes the length of the array. |
| [.slice\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice) | The **`slice()`** method returns a shallow copy of a portion of an array into a new array object selected from `begin` to `end` \(`end` not included\) where `begin` and `end` represent the index of items in that array. The original array will not be modified. |
| [.slice.call\(\)](https://stackoverflow.com/questions/7056925/how-does-array-prototype-slice-call-work) |  |
| [.some\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some) | The **`some()`** method tests whether at least one element in the array passes the test implemented by the provided function. It returns a Boolean value.  |
| [.splice\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice) | The **`splice()`** method changes the contents of an array by removing or replacing existing elements and/or adding new elements [in place](https://en.wikipedia.org/wiki/In-place_algorithm). |
| [.split\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split) | The **`split()`** method turns a [`String`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) into an array of strings, by separating the string at each instance of a specified separator string. |
| .unshift\(\) |  |

### Objects

|  |  |
| :--- | :--- |
| [.entries\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/entries) | The **`Object.entries()`** method returns an array of a given object's own enumerable string-keyed property `[key, value]` pairs, in the same order as that provided by a [`for...in`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in) loop. \(The only important difference is that a `for...in` loop enumerates properties in the prototype chain as well\).  |
| .keys\(\) |  |
| .values\(\) |  |

