exists
======

node exists function. plain and simple.

## exists(thing)

```js
var exists = require('exists');

exists(null);      // false
exists(undefined); // false
exists({});        // true
exists([]);        // true
exists('');        // true
exists(false);     // true
```

## exists.allExist(thing)

```js
var allExist = require('exists').allExist;

allExist(null, undefined);   // false
allExist({}, [], '', false); // true
allExist({}, null)  ;        // false
```

## License
MIT