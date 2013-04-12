# vector

This library provides simple vectors implementation. It doesn't create much
garbage by allowing reusing existing objects.

## API

```javascript
var v = new Vector(3, 2),
    u = new Vector(1, 4);

// arithmetic

v.nadd(0, 3); // v == (3, 5)
v.vadd(u); // v == (4, 9)

v.nsubtract(1, 1); // v == (3, 8)
v.vsubtract(u); // v == (2, 4)

v.multiply(3); // v == (6, 12)
v.divide(2); // v == (3, 6)

// manipulation

v.nupdate(4, 7); // v == (4, 7)
v.vupdate(u) // v == u == (1, 4)

// length

var len = v.length(), // len == 4.123
    len2 = v.length2(); // len2 == 17

// comparing

Vector.equal(u, v) // true
```
