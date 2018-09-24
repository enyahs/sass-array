# array_merge_recursive

array_merge_recursive — Merge two arrays recursively.

#### __Description__

```scss
array_merge_recursive(mixed $map_or_list, mixed $map_or_list_2) : array
```

#### __Parameters__
map_or_list
- Initial (map or list) to merge.
  
map_or_list_2
- (Map or list) to merge into initial (map or list).

#### __Return Values__
An array containing the result of two arrays merged recursively.


#### __Examples__
Example #1 array_merge()
```scss
$map2:
(  
    test: (circle: 1, square: 2, triangle: 3),
    test2: numbers,
    test3: names
);

$map2:
(  
    test: (circle: blue, triangle: bob),
    test2: colors,
    test4: shapes
);

$result: array_merge($map, $map2);
```
Output:
```scss
(  
    test: (circle: blue, square: 2, triangle: bob),
    test2: colors,
    test3: names,
    test4: shapes
);
```