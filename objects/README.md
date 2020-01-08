# Objects

```javascript
//object literaly syntax
const person = {
age: 100,
name: 'John',
sayHello: function (greeting = 'Hey') {
 return `${greeting} ${this.name}`;
}
}

//longer notation, not used because literal is cleaner
const person = new Object ({
age: 100,
name: 'John',
});

//to access properties use dot notation or square bracket
console.log(person.age);
console.log(person['age']); //can reference property using a variable by removing ''

//method shorthand
sayHello (greeting = 'Hey') {
 return `${greeting} ${this.name}`;
}
```

```javascript
const person1 = {
      first: 'John',
      last: 'Doe',
    };

//spread operator, copies the object instead of reference it
const person3 = { ...person1 };

Object.assign({}, person1); //old way to copy object
```

|  |  |
| :--- | :--- |
| [constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/constructor) | The constructor property returns a reference to the Object constructor function that created the instance object. Note that the value of this property is a reference to the function itself, not a string containing the function's name. The value is only read-only for primitive values such as 1, true and "test". |
| [enumerable](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Enumerability_and_ownership_of_properties) | **Enumerable** Properties in **JavaScript**. **Enumerable** properties are properties whose internal **enumerable** flag set to true. **Enumerable** simply means "countable", and with **JavaScript** objects, **enumerable** properties are those we are typically interested in when iterating over properties. |
| [polymorphism](https://developer.mozilla.org/en-US/docs/Glossary/Polymorphism) | Polymorphism is the presentation of one interface for multiple data types. |
| [properties](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#Properties_of_the_Object_constructor) | **JavaScript Properties**. **Properties** are the values associated with a **JavaScript** object. A **JavaScript** object is a collection of unordered **properties**. **Properties** can usually be changed, added, and deleted, but some are read only. |

|  |  |
| :--- | :--- |
| [.freeze\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/freeze) | method **freezes** an object. A frozen object can no longer be changed |
| .keys |  |
| [.preventExtensions\(\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/preventExtensions) | The **`Object.preventExtensions()`** method prevents new properties from ever being added to an object \(i.e. prevents future extensions to the object\). |
| .seal\(\) |  |

### Window object

|  |  |
| :--- | :--- |
| onclick |  |
| .scrollTo\(\) |  |
| .setInterval\(\) |  |
| .setTimeout\(\) |  |

