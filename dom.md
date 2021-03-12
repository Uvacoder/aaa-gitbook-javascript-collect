# DOM

### 2021

|  |  |
| :--- | :--- |
| [The difference between attributes and properties in vanilla JS](https://gomakethings.com/the-difference-between-attributes-and-properties-in-vanilla-js/) | 3/12 |
| [The Element.style.cssText property in vanilla JS](https://gomakethings.com/the-element.style.csstext-property-in-vanilla-js/) | 2/1 |

### 2020

|  |  |
| :--- | :--- |
| [Nodes vs Elements in the DOM](https://medium.com/@issabmsangare/nodes-vs-elements-in-the-dom-1865885d0b9b#:~:text=An%20element%20is%20a%20specific,are%20one%20type%20of%20node.) | 11/20 |
| [How to check if an element contains another one with the vanilla JS Node.contains\(\) method](https://gomakethings.com/how-to-check-if-an-element-contains-another-one-with-the-vanilla-js-node.contains-method/?mc_cid=8a49ef3986&mc_eid=[UNIQID]) | 9/3 |
| [How to replace an element and its content using vanilla JS](https://gomakethings.com/how-to-replace-an-element-and-its-content-using-vanilla-js/?mc_cid=a31a2cd0aa&mc_eid=[UNIQID]) | 6/20 |
| [JavaScript Fundamentals: Master the DOM! \(Part 2\)](https://medium.com/@timothyrobards/javascript-fundamentals-master-the-dom-part-2-bef36405598e) | 5/11 |
| [https://htmldom.dev/](https://htmldom.dev/) | 4/2 |

### DOM

|  |  |
| :--- | :--- |
| console |  |
| document |  |
| window |  |
| node |  |
| getters / setters |  |

|  |  |
| :--- | :--- |
| elements | [https://developer.mozilla.org/en-US/docs/Web/API/Element](https://developer.mozilla.org/en-US/docs/Web/API/Element) |
| methods |  |
| properties |  |
| classes |  |
| data attributes |  |

### Element Properties and Methods

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">.children()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.childNodes()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Element/closest">.closest()</a>
      </td>
      <td style="text-align:left">Starting with the <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> itself,
        the <b><code>closest()</code></b> method traverses parents (heading toward
        the document root) of the <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> until
        it finds a node that matches the provided selectorString. Will return itself
        or the matching ancestor. If no such element exists, it returns <code>null</code>.</td>
    </tr>
    <tr>
      <td style="text-align:left">.createRange()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/dispatchEvent">.dispatchEvent()</a>
      </td>
      <td style="text-align:left">Dispatches an <a href="https://developer.mozilla.org/en-US/docs/Web/API/Event"><code>Event</code></a> at
        the specified <a href="https://developer.mozilla.org/en-US/docs/Web/API/EventTarget"><code>EventTarget</code></a>,
        (synchronously) invoking the affected <a href="https://developer.mozilla.org/en-US/docs/Web/API/EventListener"><code>EventListener</code></a>s
        in the appropriate order. The normal event processing rules (including
        the capturing and optional bubbling phase) also apply to events dispatched
        manually with <code>dispatchEvent()</code>.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Element/classList">Element.classList()</a>
      </td>
      <td style="text-align:left">The <b><code>Element.classList</code></b> is a read-only property that returns
        a live <a href="https://developer.mozilla.org/en-US/docs/Web/API/DOMTokenList"><code>DOMTokenList</code></a> collection
        of the <code>class</code> attributes of the element. This can then be used
        to manipulate the class list.</td>
    </tr>
    <tr>
      <td style="text-align:left">.firstChild()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/ParentNode/firstElementChild">.firstElementChild()</a>
      </td>
      <td style="text-align:left">The <b><code>ParentNode.firstElementChild</code></b> read-only property
        returns the object&apos;s first child <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a>,
        or <code>null</code> if there are no child elements.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById">.getElementbyId()</a>
      </td>
      <td style="text-align:left">The <a href="https://developer.mozilla.org/en-US/docs/Web/API/Document"><code>Document</code></a> method <b><code>getElementById()</code></b> returns
        an <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> object
        representing the element whose <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element/id"><code>id</code></a> property
        matches the specified string. Since element IDs are required to be unique
        if specified, they&apos;re a useful way to get access to a specific element
        quickly.</td>
    </tr>
    <tr>
      <td style="text-align:left">.lastChild()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/ParentNode/lastElementChild">.lastElementChild()</a>
      </td>
      <td style="text-align:left">The <b><code>ParentNode.lastElementChild</code></b> read-only property returns
        the object&apos;s last child <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> or <code>null</code> if
        there are no child elements.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Element/innerHTML">.innerHTML()</a>
      </td>
      <td style="text-align:left">The <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> property <b><code>innerHTML</code></b> gets
        or sets the HTML or XML markup contained within the element.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/innerText">.innerText()</a>
      </td>
      <td style="text-align:left">The <b><code>innerText</code></b> property of the <a href="https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement"><code>HTMLElement</code></a> interface
        represents the &quot;rendered&quot; text content of a node and its descendants.
        As a getter, it approximates the text the user would get if they highlighted
        the contents of the element with the cursor and then copied it to the clipboard.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML">.insertAdjacentHTML()</a>
      </td>
      <td style="text-align:left">The insertAdjacentHTML() method of the Element interface parses the specified
        text as HTML or XML and inserts the resulting nodes into the DOM tree at
        a specified position. It does not reparse the element it is being used
        on, and thus it does not corrupt the existing elements inside that element.
        This avoids the extra step of serialization, making it much faster than
        direct innerHTML manipulation.</td>
    </tr>
    <tr>
      <td style="text-align:left">.insertAdjacentText()</td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li><code>&apos;beforebegin&apos;</code>: Before the <code>element</code> itself.</li>
          <li><code>&apos;afterbegin&apos;</code>: Just inside the <code>element</code>,
            before its first child.</li>
          <li><code>&apos;beforeend&apos;</code>: Just inside the <code>element</code>,
            after its last child.</li>
          <li><code>&apos;afterend&apos;</code>: After the <code>element</code> itself.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Node/nextSibling">.nextSibling()</a>
      </td>
      <td style="text-align:left">The <b><code>Node.nextSibling</code></b> read-only property returns the
        node immediately following the specified one in their parent&apos;s <a href="https://developer.mozilla.org/en-US/docs/Web/API/Node/childNodes"><code>childNodes</code></a>,
        or returns <code>null</code> if the specified node is the last child in the
        parent element.</td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/NonDocumentTypeChildNode/nextElementSibling">.nextElementSibling()</a>
      </td>
      <td style="text-align:left">The <b><code>NonDocumentTypeChildNode.nextElementSibling</code></b> read-only
        property returns the element immediately following the specified one in
        its parent&apos;s children list, or <code>null</code> if the specified element
        is the last one in the list.</td>
    </tr>
    <tr>
      <td style="text-align:left">.outerHTML()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.parentNode()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.parentElement()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.previousSibling()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.previousElementSibling()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.remove()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.textContent()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><a href="https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector">.querySelector()</a>
      </td>
      <td style="text-align:left">The <a href="https://developer.mozilla.org/en-US/docs/Web/API/Document"><code>Document</code></a> method <b><code>querySelector()</code></b> returns
        the first <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element"><code>Element</code></a> within
        the document that matches the specified selector, or group of selectors.
        If no matches are found, <code>null</code> is returned.</td>
    </tr>
    <tr>
      <td style="text-align:left">.querySelectorAll()</td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

### Attributes

|  |  |
| :--- | :--- |
| .dataset\(\) |  |
| .getAttribute\(\) |  |
| .hasAttribute\(\) |  |
| [.removeAttribute\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Element/removeAttribute) | The [`Element`](https://developer.mozilla.org/en-US/docs/Web/API/Element) method **`removeAttribute()`** removes the attribute with the specified name from the element. |
| [.setAttribute\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Element/setAttribute) | Sets the value of an attribute on the specified element. If the attribute already exists, the value is updated; otherwise a new attribute is added with the specified name and value. |

### HTML

|  |  |
| :--- | :--- |
| [.appendChild\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild) | The **`Node.appendChild()`** method adds a node to the end of the list of children of a specified parent node. If the given child is a reference to an existing node in the document, `appendChild()` moves it from its current position to the new position \(there is no requirement to remove the node from its parent node before appending it to some other node\). |
| .cloneNode\(\) |  |
| [.createElement\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement) | In an HTML document, the document.createElement\(\) method creates the HTML element specified by tagName, or an HTMLUnknownElement if tagName isn't recognized. |
| .insertAdjacentElement\(\) |  |

