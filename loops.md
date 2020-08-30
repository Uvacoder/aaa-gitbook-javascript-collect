# Loops

|  |  |
| :--- | :--- |
| [Should You Stop Using .forEach\(\) in Your JavaScript Code?](https://medium.com/better-programming/should-you-stop-using-foreach-in-your-javascript-code-efe1e86c78e5) | 8/30 |

|  |  |
| :--- | :--- |
| [.filter\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) | The **`filter()`** method **creates a new array** with all elements that pass the test implemented by the provided function. |
| [.forEach\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) | The **`forEach()`** method executes a provided function once for each array element. |
| [.map\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) | The **`map()`** method **creates a new array** populated with the results of calling a provided function on every element in the calling array. |
| [.reduce\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) | The **`reduce()`** method executes a **reducer** function \(that you provide\) on each element of the array, resulting in a single output value. |
|  |  |

### Loops

```javascript
const numbers = [2, 34, 3, 23, 42, 3, 1, 65, 364, 5, 645, 6];
const name = 'John Doe 🙋‍♂️';
const john = {
  name: 'John',
  age: 100,
  cool: true,
}
```

{% code title="for - loop" %}
```javascript
for (let i = 0; i < numbers.length; i++) {
console.log(numbers[i]);
}
```
{% endcode %}

{% code title="for of - promises/await" %}
```javascript
for(const letter of name) {
console.log(letter);
}
```
{% endcode %}

{% code title="for in - used for looping over keys of an object" %}
```javascript
for(const prop in john) {
console.log(prop);
}
```
{% endcode %}

{% code title="while loop - runs until condition is false" %}
```javascript
let cool = true;
let i = 1;
while(cool === true) {
  console.log('You are cool');
  i++;
  if(i > 100) {
    cool = false;
  }
}
```
{% endcode %}

{% code title="do while loop - will always run first do condition" %}
```javascript
do {

} while () {

}
```
{% endcode %}

