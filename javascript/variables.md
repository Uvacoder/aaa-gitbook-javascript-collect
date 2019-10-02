# Variables

{% embed url="https://medium.com/startcode/javascript-basics-variables-389d4f2401d7" %}



_Definition \(Wiki\): A variable is a storage location in memory paired with a symbolic name \(identifier\), which contains some known quantity of information referred to as a value._

Just like any other popular programming language, Javascript can store information in **variables**.

If you are interested in other topics related to Javascript Basics please check them out:

* [Data Types — Part 1](https://medium.com/startcode/javascript-basics-data-types-part-1-b6dc500c74ff)

### 1. Basic syntax <a id="100d"></a>

If we would want to declare a variable identified with the symbolic name _**a**_ that contains the value _**10**_ we would use the following syntax:Fig.1.1 Basic variable declaration \(INCOMPLETE\)

However our code is not complete, even though it runs and we have no error thrown in browser’s console tab. The complete version of the example would look like this:Fig.1.2 Basic variable declaration \(COMPLETE\)

Our new version of the code contains a keyword called _**var**_ before the declaration of _**a**_ and explicitly marks it as a variable. This approach will help other programmers that will take a look at our code in order to understand our logic.

> But why we didn’t got an error from running the first example?

Javascript is not a compiled programming language and it’s interpreted by a tool named **Javascript Engine.** One of the components of the Javascript Engine is the **Syntax Parser** that analyzes our code and makes sure that it is correct from a syntactic point of view. So if you forgot to add the **var** keyword, the Syntax Parser will add it for you. Be careful though because you shouldn’t relay on this approach because your code won’t be readable by other developers.

### 2. Variable shadowing <a id="6d9f"></a>

_Definition: The shadowing concept refers to the declaration of a variable with the same name in a different scope \(decision block, method, inner class\)._

_**Example 1:**_Fig.2.1 Variable Shadowing \(Example 1\)

When **syntax parser** analyzes the first example, it finds the first declaration of the **a** variable in the **global execution context**. On the call of the function **shadowing** a new **execution context** is created and the parser allocates the memory for variable **a** on the stack. There are no instructions left to be executed and the context is destroyed. That means that the variable **a** declared in the function **shadowing** doesn’t exist in memory anymore. The last instruction **console.log\(a\)** will look for variable a and print its value. The parser finds the associated name variable in the global execution context with the value 10 and prints it.

**Example 2:**Fig.2.2 Variable Shadowing \(Example 2\)

The difference between first and second example is the missing keyword from the instruction **a = 20**. When the execution context of the function **shadowing** is created it looks for a variable with associated name a and the parser finds it in the global execution context. The instruction changes the value of variable a from 10 to 20, so when **console.log\(a\)** is executed it will print 20.

### 3. Block scoped variables <a id="851b"></a>

In 2015 when ECMAScript 6 \(conventionally named **ES6**\) was released, it introduced a new concept called block scoped variable.

_Definition: A block scoped variable is declared inside of a pair of curly brackets and it’s visible only in that specific scope._

**Example 1:**Fig.3.1 Block scoped variables \(Example 1\)

When the **blockScoped** function is called a new execution context is created and the parser looks for the **a** variable that is found in the global execution context \(with the associated value 10\). The condition of the control structure **if** is passed because **10 &gt; 5** and the variable a is created in the block associated with the control structure. After the execution of **let a = 20** the next instruction **console.log\(a\)** will look for the variable a that is only visible from the global execution context, so the printed value is 10.

**Example 2:**Fig.3.2 Block scoped variables \(Example 2\)

Moving the **console.log\(a\)** instruction inside the control structure will make the functions **blockScoped** to behave in a different way and the printed result will be 20.

### **4. Immutable variables** <a id="0f19"></a>

Another type that was released in ES6 gives the developers the possibility to create immutable variables by using **const** keyword.

_Definition: An immutable variable is a variable whose value cannot be modified after it was created._

**Example 1:**Fig.4.1 Immutable variables \(Example 1\)

If we would remove the second line from the example our code will run without any problems and the printed value will be 20.

> Note: Immutability of const variables is only applied to primitives. However if we would declare an object instead, we could add new properties and modify them.

### 5. Variable’s behavior in closures <a id="cac8"></a>

_Definition: A closure is the combination of a function and the lexical environment within which that function was declared._

**Example 1 \(using var keyword\):**![](https://miro.medium.com/max/60/1*OSEYXcyv50HPIaaxPJrOuw.png?q=20)![](https://miro.medium.com/max/2108/1*OSEYXcyv50HPIaaxPJrOuw.png)Fig.5.1 Variable’s behavior in closures \(Example 1\)

Let’s break the 3rd example into smaller pieces starting from the call of the function **print\(\)** and storing its returned value into a variable **printer**.![](https://miro.medium.com/max/34/1*MgA-YIejawpf0mBbfgnAKQ.png?q=20)![](https://miro.medium.com/max/506/1*MgA-YIejawpf0mBbfgnAKQ.png)Fig.5.2 Call Stack

Let’s see if you can guess the printed values for the code above. You’re right, in the console you will see 3 3 3.

> How is this value obtained?

Analyzing the for block iteration by iteration we will obtain the following values for i:

**FIRST ITERATION \(i = 0\):**

* 0 &lt; 3 is true;
* Add to the functions array the function with the instruction console.log\(i\);
* i++;

**SECOND ITERATION \(i = 1\):**

* 1 &lt; 3 is true;
* Add to the functions array the function with the instruction console.log\(i\);
* i++;

**THIRD ITERATION \(i=2\):**

* 2 &lt; 3 is true;
* Add to the functions array the function with the instruction console.log\(i\);
* i++;

After the third iteration **i** does not meet the condition **i &lt; 3 \(i = 3 now\)** and the loop is finished. There are no other instructions to be executed in the function so the **execution context** of function **print\(\)** is destroyed and removed from the **call stack**. The engine is smart enough to see that we used the variable **i** in another function that is not called yet so it will keep in memory the last value of **i**, which is **3**.

**Example 2 \(using let keyword\):**![](https://miro.medium.com/max/60/1*yPeIUaUO6PDPZxcLSIDtfw.png?q=20)![](https://miro.medium.com/max/1760/1*yPeIUaUO6PDPZxcLSIDtfw.png)Fig.5.3 Variable’s behavior in closures \(Example 2\)

Running the second example we will see a different result in the console: 0, 1, 2.

> Why is this happening?

The call stack with the execution contexts \(_Fig.5.2_\) is the same for this example, but the single difference is made by the **let** keyword from the **for loop.** Instead of holding one reference to the last value of **i** \(take a look to the previous example\), the engine will hold a reference of **i** for each iteration block.

> If you have any questions related to this article please leave a comment below. Subscribe to our publication in order to find more articles like this and enhance your developer skills on various topics. Thanks!

