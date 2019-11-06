# this

{% embed url="https://dev.to/naveenkolambage/test-11fd" %}



### What does 'this' return?

Here's an object which uses this keyword  


```
const man = {
  name: "rick",
  adventure() {
    console.log(this);
  }
};

man.adventure(); 
```

Executing above you will see the man object on the console.

[![Alt Text](https://res.cloudinary.com/practicaldev/image/fetch/s--4D-RibuK--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/b0a1xhy987g2frfc6hxx.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--4D-RibuK--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/b0a1xhy987g2frfc6hxx.png)

But what if you do;  


```
const adventure_reference = man.adventure;

adventure_reference();
```

Output then would be;

[![Alt Text](https://res.cloudinary.com/practicaldev/image/fetch/s--q9vmteTI--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/9sfmbc2htt3ga27yu46z.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--q9vmteTI--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/9sfmbc2htt3ga27yu46z.png)

### Explanation

Value of 'this' is determined by how a function is called;

* If we call a function as a method in an object this will always return a reference to that object.
* If we call a function as a standalone object - or outside an object this will return the global object which is the window object in browsers.

