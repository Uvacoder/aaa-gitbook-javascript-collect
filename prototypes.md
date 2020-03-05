# Prototypes

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes">class</a>
      </td>
      <td style="text-align:left">JavaScript classes, introduced in ECMAScript 2015, are primarily syntactical
        sugar over JavaScript&apos;s existing prototype-based inheritance. The
        class syntax <em>does not</em> introduce a new object-oriented inheritance
        model to JavaScript.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new">new</a>
      </td>
      <td style="text-align:left">
        <p></p>
        <p>The <b><code>new</code> operator</b> lets developers create an instance
          of a user-defined object type or of one of the built-in object types that
          has a constructor function. The <b><code>new</code></b> keyword does the
          following things:</p>
        <ol>
          <li>Creates a blank, plain JavaScript object;</li>
          <li>Links (sets the constructor of) this object to another object;</li>
          <li>Passes the newly created object from <em>Step 1</em> as the <code>this</code> context;</li>
          <li>Returns <code>this</code> if the function doesn&apos;t return its own object.</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">prototype</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this">this</a>
      </td>
      <td style="text-align:left">
        <p>A <b>function&apos;s <code>this</code> keyword</b> behaves a little differently
          in JavaScript compared to other languages. It also has some differences
          between <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions_and_function_scope/Strict_mode">strict mode</a> and
          non-strict mode.</p>
        <p>In most cases, the value of <code>this</code> is determined by how a function
          is called (runtime binding). It can&apos;t be set by assignment during
          execution, and it may be different each time the function is called. ES5
          introduced the <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind"><code>bind()</code></a> method
          to <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this#The_bind_method">set the value of a function&apos;s <code>this</code> regardless of how it&apos;s called</a>,
          and ES2015 introduced <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions">arrow functions</a> which
          don&apos;t provide their own <code>this</code> binding (it retains the <code>this</code> value
          of the enclosing lexical context).</p>
      </td>
    </tr>
  </tbody>
</table>