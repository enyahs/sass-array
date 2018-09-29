# array_count_recursive

array_count_recursive — Count all elements in an array recursively.

#### __Description__

```scss
array_count_recursive(mixed $map_or_list) : int
```

#### __Parameters__
map_or_list
- Initial (map or list).

#### __Return Values__
The number of elements in the given array.


#### __Examples__
Example #1 array_count_recursive()
```scss
$map:(
    sizes: (small, medium, large), // 4
    colors: (blue, red, green, orange) // 5
);

$result: array_count_recursive($map);
```
Output:
```scss
9
```
\
Example #2 array_count_recursive()
```scss
$list:(
    (left: left, center: center, right: right), // 4
    (10px, 20px) // 3
);

$result: array_count_recursive($list);
```
Output:
```scss
7
```