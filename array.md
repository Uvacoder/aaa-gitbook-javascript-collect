# Array

|  |  |
| :--- | :--- |
| [Removing duplicates from an array with the vanilla JS Set\(\) object](https://gomakethings.com/removing-duplicates-from-an-array-with-the-vanilla-js-set-object/?mc_cid=11d34946a2&mc_eid=[UNIQID]) | 8/1 |
| [How to reorder an item in an array with vanilla JS](https://gomakethings.com/how-to-reorder-an-item-in-an-array-with-vanilla-js/?mc_cid=c0083d96b8&mc_eid=[UNIQID]) | 7/16 |
| [JavaScript: How to Remove Duplicate Values from Arrays](https://dev.to/will_devs/javascript-how-to-remove-duplicate-values-from-arrays-lf0?utm_source=digest_mailer&utm_medium=email&utm_campaign=digest_email) | 7/5 |
| [How I work with arrays](https://zellwk.com/blog/how-i-work-with-arrays/?ck_subscriber_id=420572458) | 6/17 |
| [Revisiting Array.reduce\(\)](https://gomakethings.com/revisiting-array.reduce/?mc_cid=349c39a779&mc_eid=[UNIQID]) | 6/9 |
| [When to use which array method in vanilla JS](https://gomakethings.com/when-to-use-which-array-method-in-vanilla-js/?mc_cid=c513a900d9&mc_eid=[UNIQID]) | 6/3 |
| [Getting the last matching item in an array with vanilla JS](https://gomakethings.com/getting-the-last-matching-item-in-an-array-with-vanilla-js/?mc_cid=fbcd1aac35&mc_eid=[UNIQID]) | 4/20 |
| [How to flatten an array with vanilla JS](https://gomakethings.com/how-to-flatten-an-array-with-vanilla-js/?mc_cid=cad6df7f69&mc_eid=[UNIQID]) | 4/7 |
| [Five interesting ways \(and one boring way\) to use Array.reduce\(\)](https://gomakethings.com/five-interesting-ways-and-one-boring-way-to-use-array.reduce) | 12/19/2019 |
| [13 useful Array tips and tricks](https://dev.to/duomly/13-useful-javascript-array-tips-and-tricks-you-should-know-2jfo) |  |
| [MDN Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) |  |

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
| [.every\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every) | The **`every()`** method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value. |
| [.flat\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/flat) | The **`flat()`** method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth. |
| [.find\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find) | The **`find()`** method returns the **value** of the **first element** in the provided array that satisfies the provided testing function. |
| [.findIndex\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex) | The **`findIndex()`** method returns the **index** of the first element in the array **that satisfies the provided testing function**. Otherwise, it returns -1, indicating that no element passed the test. |
| [.fill\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/fill) | The **`fill()`** method changes all elements in an array to a static value, from a start index \(default `0`\) to an end index \(default `array.length`\). It returns the modified array. |
| [.filter\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) | The **`filter()`** method **creates a new array** with all elements that pass the test implemented by the provided function. |
| [.forEach\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) | The **`forEach()`** method executes a provided function once for each array element. |
| [.from\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from) | The **`Array.from()`** method creates a new, shallow-copied `Array` instance from an array-like or iterable object.  |
| [.includes\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/includes) | The **`includes()`** method determines whether an array includes a certain value among its entries, returning `true` or `false` as appropriate. |
| [.indexOf\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf) | The **`indexOf()`** method returns the first index at which a given element can be found in the array, or -1 if it is not present. |
| [.join\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join) | The **`join()`** method creates and returns a new string by concatenating all of the elements in an array \(or an [array-like object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections#Working_with_array-like_objects)\), separated by commas or a specified separator string. If the array has only one item, then that item will be returned without using the separator. |
| [.keys\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/keys) | The **`keys()`** method returns a new **`Array Iterator`** object that contains the keys for each index in the array. |
| [.lastIndexOf\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/lastIndexOf) | The **`lastIndexOf()`** method returns the index within the calling [`String`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) object of the last occurrence of the specified value, searching backwards from `fromIndex`. Returns -1 if the value is not found. |
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
| [.sort\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort) | The **`sort()`** method sorts the elements of an array [_in place_](https://en.wikipedia.org/wiki/In-place_algorithm) and returns the sorted array. The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values. |
| [.splice\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice) | The **`splice()`** method changes the contents of an array by removing or replacing existing elements and/or adding new elements [in place](https://en.wikipedia.org/wiki/In-place_algorithm). |
| [.split\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split) | The **`split()`** method turns a [`String`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) into an array of strings, by separating the string at each instance of a specified separator string. |
| [.unshift\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift) | The **`unshift()`** method adds one or more elements to the beginning of an array and returns the new length of the array. |

### Objects

|  |  |
| :--- | :--- |
| [.entries\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/entries) | The **`Object.entries()`** method returns an array of a given object's own enumerable string-keyed property `[key, value]` pairs, in the same order as that provided by a [`for...in`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in) loop. \(The only important difference is that a `for...in` loop enumerates properties in the prototype chain as well\).  |
| .keys\(\) |  |
| .values\(\) |  |

