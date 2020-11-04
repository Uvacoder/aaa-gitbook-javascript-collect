# Vue

|  |  |
| :--- | :--- |
| [Converting the Vue.js markdown editor demo to vanilla JS](https://gomakethings.com/converting-the-vue.js-markdown-editor-demo-to-vanilla-js/) | 11/3 |
| [Vuebersicht - custom desktop widgets](https://github.com/nickforddesign/vuebersicht) | 9/20 |
| [A Complete Beginner's Guide to Vue](https://dev.to/aspittel/a-complete-beginners-guide-to-vue-422n) | 8/17 |
| [5 JavaScript Tips I Learned From Vue Source Code](https://levelup.gitconnected.com/5-javascript-tips-i-learned-from-vue-source-code-6095df4e9bc1) | 5/17 |
| [How to Boost Vue.js Performance](https://itnext.io/how-to-boost-vue-js-performance-c7df027ff3f5) | 4/19 |
| [Add a Timeline to Your Vue.js App](https://medium.com/javascript-in-plain-english/add-a-timeline-to-your-vue-js-app-3b0804c06c0a) | 4/8 |
| [7 Great Vue3 Tutorials and Resources to Start Learning Today](https://learnvue.co/2020/03/7-great-vue3-tutorials-and-resources-to-start-learning-today/?utm_source=newsletter&utm_medium=email&utm_campaign=4_2) | 4/2 |
| [Why I prefer Vue over React](https://medium.com/@gaute.meek/why-i-prefer-vue-over-react-12ab1da113be) | 3/9 |
| [VueJS Cheatsheet for Developers](https://attachments.convertkitcdnn2.com/234155/4726aa35-b3dc-4d94-9981-e38f91dc5802/A%20VueJS%20Cheatsheet%20for%20Developers-LearnVue.pdf) | 3/2 |
| [5 Tools for Faster Vue.js App Development](https://blog.bitsrc.io/5-tools-for-faster-vue-js-app-development-ad7eda1ee6a8) | 2/13 |

|  |  |
| :--- | :--- |
| v-bind | Dynamically binds an attribute to an expression. |

```javascript
const app = new Vue({
  el: "#app",
  data: {
    product: "socks",
    image: './assets/vmSocks-green.jpg'
  },
});
```

```javascript
{{ }} //expression
```

```markup
<img v-bind:src="image"> //v-bind
:src //short-hand

:alt="description"
:href="url"
:title="toolTip"
:class="isActive"
:style="isStyled"
:disabled="isDisabled"

```

