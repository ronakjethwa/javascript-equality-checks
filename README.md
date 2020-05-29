# JavaScropt Equality Checks
### Some Fun Equality Checks In JavaScript

There are mainly 3 ways to check the value equality in JavaScrpt. You already know two of them. There is a fun third one.
```js
- Strict Equality: a === b (triple equals).
- Loose Equality: a == b (double equals).
- Same Value Equality: Object.is(a, b).
```

```js
// Zero, look closely!
-0 == 0; // true
-0 === 0; // true
Object.is(-0,0); // false
```

```js
// One, an obvious one!
-1 == 1; //false
-1 === 1; // false
Object.is(-1,1); // false
```

```js
// NaN
NaN == NaN; // false
NaN === NaN; // false
Object.is(NaN,NaN); // true
```

```js
// String, one more obvious one!
'foo' == 'foo'; // true
'foo' === 'foo'; // true
Object.is('foo', 'foo'); // true
```

```js
// Array
[] == []; // false
[] === []; // false 
Object.is([], []); // false
```