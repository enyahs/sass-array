# Sass Array
A library that converts combinations of maps and lists to associative arrays and provides extra functionality to make working with both lists and maps more simplified.

__Note:__
All array functions in this package will use the array() function to convert combinations of lists and maps to associative arrays before the handle function is executed.

#### __Array Functions__

- [array_count_recursive](docs/array_count_recursive.md) — Count all elements in an array recursively.
- [array_count](docs/array_count.md) — Count all elements in an array.
- [array_get](docs/array_get.md) — Get a value in an array from the given key path.
- [array_keys](docs/array_keys.md) — Return all the keys of an array.
- [array_merge_recursive](docs/array_merge_recursive.md) — Merge two arrays recursively.
- [array_merge](docs/array_merge.md) — Merge two arrays.
- [array_values](docs/array_values.md) — Return all the values of an array.
- [array](docs/array.md) — Create an array.

#### __Install__
```bash
npm install sass-array --save-dev
```

#### __Example__
```scss
@import '~sass-array';

$test:(1,2,3);
$test2:(4,5,6);
$test3:(shape: circle, color: red);
$test4:(people: (shayne: 21, john: 24));

@debug(array_count($test));
// 3

@debug(array_get($test4, 'people.shayne'));
// 21

@debug(array_keys($test3));
// (0: shape, 1: color)

@debug(array_merge($test, $test2));
// (0: 1, 1: 2, 2: 3, 3: 4, 4: 5, 5: 6)

@debug(array_values($test3));
// (0: circle, 1: red)
```