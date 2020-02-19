# Operators

|  |  |  |
| :--- | :--- | :--- |
| [MDN Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) | 1/2/2020 | 1/2/2020 |

### Binary Operators

### Compound assignment operators

| Shorthand operator | Meaning |  |
| :--- | :--- | :--- |
| [Assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Assignment) | `x = y` | `x = y` |
| [Addition assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Addition_assignment) | `x += y` | `x = x + y` |
| [Subtraction assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Subtraction_assignment) | `x -= y` | `x = x - y` |
| [Multiplication assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Multiplication_assignment) | `x *= y` | `x = x * y` |
| [Division assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Division_assignment) | `x /= y` | `x = x / y` |
| [Remainder assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Remainder_assignment), \(modulo\) | `x %= y` | `x = x % y` |
| [Exponentiation assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Exponentiation_assignment) | `x **= y` | `x = x ** y` |
| [Left shift assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Left_shift_assignment) | `x <<= y` | `x = x << y` |
| [Right shift assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Right_shift_assignment) | `x >>= y` | `x = x >> y` |
| [Unsigned right shift assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Unsigned_right_shift_assignment) | `x >>>= y` | `x = x >>> y` |
| [Bitwise AND assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Bitwise_AND_assignment) | `x &= y` | `x = x & y` |
| [Bitwise XOR assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Bitwise_XOR_assignment) | `x ^= y` | `x = x ^ y` |
| [Bitwise OR assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators#Bitwise_OR_assignment) | `x |= y` | `x = x | y` |

### Comparison operators

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Operator</td>
      <td style="text-align:left">Description</td>
      <td style="text-align:left">Examples returning true</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Equality">Equal</a> (<code>==</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the operands are equal.</td>
        <td style="text-align:left">
          <p><code>3 == var1</code>
          </p>
          <p><code>&quot;3&quot; == var13 == &apos;3&apos;</code>
          </p>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Inequality">Not equal</a> (<code>!=</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the operands are not equal.</td>
        <td style="text-align:left"><code>var1 != 4<br />var2 != &quot;3&quot;</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Identity">Strict equal</a> (<code>===</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the operands are equal and of the same type.
        See also <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/is"><code>Object.is</code></a> and
        <a
        href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">sameness in JS</a>.</td>
          <td style="text-align:left"><code>3 === var1</code>
          </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Nonidentity">Strict not equal</a> (<code>!==</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the operands are of the same type but not equal,
        or are of different type.</td>
        <td style="text-align:left"><code>var1 !== &quot;3&quot;<br />3 !== &apos;3&apos;</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Greater_than_operator">Greater than</a> (<code>&gt;</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the left operand is greater than the right
        operand.</td>
        <td style="text-align:left"><code>var2 &gt; var1<br />&quot;12&quot; &gt; 2</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Greater_than_or_equal_operator">Greater than or equal</a> (<code>&gt;=</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the left operand is greater than or equal to
        the right operand.</td>
        <td style="text-align:left"><code>var2 &gt;= var1<br />var1 &gt;= 3</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Less_than_operator">Less than</a> (<code>&lt;</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the left operand is less than the right operand.</td>
        <td
        style="text-align:left"><code>var1 &lt; var2<br />&quot;2&quot; &lt; 12</code>
          </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators#Less_than_or_equal_operator">Less than or equal</a> (<code>&lt;=</code>)</td>
      <td
      style="text-align:left">Returns <code>true</code> if the left operand is less than or equal to the
        right operand.</td>
        <td style="text-align:left"><code>var1 &lt;= var2<br />var2 &lt;= 5</code>
        </td>
    </tr>
  </tbody>
</table>### Unary Operators

|  |  |
| :--- | :--- |
| instanceof | The **`instanceof` operator** tests whether the `prototype` property of a constructor appears anywhere in the prototype chain of an object. |
| typeof |  |
| - |  |
| ! |  |

### Ternary Operators

```javascript
console.log(true ? 1 : 2);
// → 1
console.log(false ? 1 : 2);
// → 2
```

