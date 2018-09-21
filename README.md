# Sass Array
A library that takes the hassle away from dealing with both maps and lists with extra functionality to use in your sass code. ( Note: Each array function converts combinations of maps and lists to full array maps using array() before the function handle is called. )

#### __Array Functions__

- [array_get](docs/array_get.md) — Get an item inside an array.
- [array_merge](docs/array_merge.md) — Merge two arrays.
- [array_merge_recursive](docs/array_merge_recursive.md) — Merge two arrays recursively.
- [array_count](docs/array_count.md) — Count all elements in an array.
- [array_count_recursive](docs/array_count_recursive.md) — Count all elements in an array recursively.
- [array_values](docs/array_values.md) — Return all the values of an array
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

@debug(array_merge($test, $test2));
// (0: 1, 1: 2, 2: 3, 3: 4, 4: 5, 5: 6)

@debug(array_count($test));
// 3

@debug(array_values($test3));
// (0: circle, 1: red)

@debug(array_get($test4, 'people.shayne'));
// 21
```
