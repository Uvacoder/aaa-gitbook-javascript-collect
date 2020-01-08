# DOM

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
      <td style="text-align:left">.firstElementChild()</td>
      <td style="text-align:left"></td>
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
      <td style="text-align:left">.lastElementChild()</td>
      <td style="text-align:left"></td>
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
      <td style="text-align:left">.nextSibling()</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">.nextElementSibling()</td>
      <td style="text-align:left"></td>
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
</table>### Attributes

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
| [.appendChild\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild) |  |
| .cloneNode\(\) |  |
| [.createElement\(\)](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement) | In an HTML document, the document.createElement\(\) method creates the HTML element specified by tagName, or an HTMLUnknownElement if tagName isn't recognized. |
| .insertAdjacentElement\(\) |  |

