# Regex

|  |  |
| :--- | :--- |
| [Javascript regular expressions aren’t that daunting — here’s how to design your own](https://bestgamingpro.com/javascript-regular-expressions-arent-that-daunting-heres-how-to-design-your-own/) | 7/22 |
| [Regex cheatsheet](https://gomakethings.com/regex-cheatsheet/?mc_cid=7b2b275824&mc_eid=[UNIQID]) | 6/11 |
| [https://ihateregex.io/](https://ihateregex.io/) | 3/4 |
| [http://regexr.com/](http://regexr.com/) | 1/22/2020 |
| [6 Handy Regular Expressions Every Front-End Developer Should Know](https://blog.bitsrc.io/6-handy-regular-expressions-every-front-end-developer-should-know-ac9e0c514b71) | 1/21/2020 |
| [Regex with JavaScript](https://gomakethings.com/regex-with-javascript/?mc_cid=b8a79b9d38&mc_eid=e9174ba77f) | 1/17/2020 |
| [Intro to Regex for Web Developers](https://dev.to/chrisachard/intro-to-regex-for-web-developers-2fj4) |  |
| [Regex tutorial — A quick cheatsheet by examples](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285) |  |

{% code title="Regex" %}
```javascript
[^.!?] //matches any character that’s not a ., !, or ?
[1–9]  //matches a digit between 1 to 9.
*      //matches zero or more sequences of the preceding item
\b     //matches at a position known as a “word boundary” (a position that’s either followed or preceded by an ASCII letter, digit, or underscore).\b matches at a position known as a “word boundary” (a position that’s either followed or preceded by an ASCII letter, digit, or underscore).
\s     //matches a single whitespace character, including ASCII space, tab, line feed, carriage return, vertical tab, and form feed
.      //matches any character that’s not a line break character
+      //matches the previous item one or more times
?      //matches zero or one occurrence of the preceding item
g      //tells the regex engine to match all occurrences rather than stopping after the first match
i      //makes the search case-insensitive

str.match(//gi);
```
{% endcode %}

