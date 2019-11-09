# Math.random\(\)

{% embed url="https://gomakethings.com/generating-random-numbers-with-vanilla-js/" %}

## Generating random numbers with vanilla JS

Today, we’re going to look at how to create random numbers with vanilla JavaScript.

### The `Math.random()` method [\#](https://gomakethings.com/generating-random-numbers-with-vanilla-js/#the-math-random-method) <a id="the-math-random-method"></a>

The `Math.random()` method generates a random float \(a number with decimals\) between `0` and `1`.

```text
// Logs something like this: 0.37111265461165543
// It will be different every time
var rand = Math.random();
console.log(rand);
```

The number the `Math.random()` method generates is inclusive of `0` \(as in, it _could_ sometimes be `0`, though I’ve never personally seen that happen\), but exclusive of `1` \(as in, it will never reach `1`\).

[Here’s a demo.](https://codepen.io/cferdinandi/pen/OJJyGxz)

### Getting numbers bigger than `0` [\#](https://gomakethings.com/generating-random-numbers-with-vanilla-js/#getting-numbers-bigger-than-0) <a id="getting-numbers-bigger-than-0"></a>

What if you wanted to get integers, or whole numbers, instead of floats?

To do that, we can multiply whatever `Math.random()` returns by a number that’s a power of ten. The bigger the number you multiple by, the more digits in the number.

```text
var randomOverZero = function (pow) {
	return Math.random() * pow;
};

// Logs something like: 14.48985072988853
var rand100 = randomOverZero(100);
console.log(rand100);

// Logs something like: 9005.187977724258
var rand10000 = randomOverZero(10000);
console.log(rand10000);
```

[Here’s another demo.](https://codepen.io/cferdinandi/pen/mddegKB)

### Getting a random integer [\#](https://gomakethings.com/generating-random-numbers-with-vanilla-js/#getting-a-random-integer) <a id="getting-a-random-integer"></a>

What if you wanted a random integer, or whole number, instead of a float?

For that, we can use the `Math.floor()` method after multiplying the returned value of `Math.random()` by our power of ten.

```text
var randomInteger = function (pow) {
	return Math.floor(Math.random() * pow);
};

// Logs something like: 14
var rand100 = randomInteger(100);
console.log(rand100);

// Logs something like: 9005
var rand10000 = randomInteger(10000);
console.log(rand10000);
```

[Here’s a demo of the random integer technique.](https://codepen.io/cferdinandi/pen/RwwWOYL)

### Getting a random integer between two numbers [\#](https://gomakethings.com/generating-random-numbers-with-vanilla-js/#getting-a-random-integer-between-two-numbers) <a id="getting-a-random-integer-between-two-numbers"></a>

Finally, let’s look at how to get a random integer between two numbers. For example, let’s say you wanted a number that was at least 5, but no bigger than 42.

For that, we’ll create a helper function that accepts a `min` and `max` for the random number as arguments.

Then, we’ll subtract the `min` from the `max`, and add `1` to it \(otherwise the `max` would never be reached\). We’ll multiply the returned value of `Math.random()` by this new number, and add the `min` to it. This gives us a random float between our two values.

Finally, we’ll use `Math.floor()` to turn it into an integer, and return the result.

```text
var randomNumber = function (min, max) {
	return Math.floor(Math.random() * (max - min + 1) + min);
};

// Logs something like 37
var rand = randomNumber(5, 42);
console.log(rand);
```

_Props to_ [_the MDN examples section for `Math.random()`_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random#Examples) _for helping me figure this one out._

You can [play with a demo on CodePen](https://codepen.io/cferdinandi/pen/BaaoEXq), or [download this on the Vanilla JS Toolkit](https://vanillajstoolkit.com/helpers/).

