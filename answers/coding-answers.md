# Coding Questions

#### *Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Answer:* `'1020'`, because of type coercion from Number to String.

#### *Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

*Answer:* `one`, `three` and `two`. The console will print `one` and `three`, and then print `two` on the next event loop.


