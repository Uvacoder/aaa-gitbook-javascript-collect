# Loops

|  |  |
| :--- | :--- |
| [.filter\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) | The **`filter()`** method **creates a new array** with all elements that pass the test implemented by the provided function. |
| [.forEach\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) | The **`forEach()`** method executes a provided function once for each array element. |
| [.map\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) | The **`map()`** method **creates a new array** populated with the results of calling a provided function on every element in the calling array. |
| [.reduce\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) | The **`reduce()`** method executes a **reducer** function \(that you provide\) on each element of the array, resulting in a single output value. |
|  |  |

```javascript
const numbers = [2, 34, 3, 23, 42, 3, 1, 65, 364, 5, 645, 6];
const name = 'John Doe 🙋‍♂️';
const john = {
  name: 'John',
  age: 100,
  cool: true,
}

//for - loop
for (let i = 0; i < numbers.length; i++) {
console.log(numbers[i]);
}

//for of - promises/await
for(const letter of name) {
console.log(letter);
}

//for in - used for looping over keys of an object
for(const prop in john) {
console.log(prop);
}

//while loop - runs until condition is false
let cool = true;
let i = 1;
while(cool === true) {
  console.log('You are cool');
  i++;
  if(i > 100) {
    cool = false;
  }
}

//do while loop - will always run first do condition
do {

} while () {

}
```

>

