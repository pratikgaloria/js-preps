# js-preps
Simplified document and reads for Javascript

_This document is yet to be organized in a better way_

## OOPs

**Javascript supports method overridding and not method overloading**

Any function with the same name in the given context overrides the previous definition. Hence,

```javascript
function sum(a, b, c) {
  return a + b + c;
}

function sum(a, b) {
  return a + b;
}

sum(1, 2);        // return 3
sum(1, 2, 3);     // returns 3 and not 6
```
**Hack!**

You can use `arguments` object in a parent function and decide which child function to call based on its length.

https://jsfiddle.net/pratikgaloria/fpe4bmua/

