# array_merge

array_merge — Merge two arrays.

#### __Description__

```scss
array_merge(mixed $map_or_list, mixed $map_or_list_2) : array
```

#### __Parameters__
map_or_list
- Initial (map or list) to merge.
  
map_or_list_2
- (Map or list) to merge into initial (map or list).

#### __Return Values__
An array containing the result of two arrays merged.


#### __Examples__
Example #1 array_merge()
```scss
$map:(
    color: red
);

$list:
(  
    1,
    2,
    5
);

$result: array_merge($map, $list);
```
Output:
```scss
(
    color: red,
    0: 1,
    1: 2,
    2: 5
)
```
\
Example #2 array_merge()
```scss
$list:
(
    1,
    2,
    3
);

$list2:
(  
    4,
    5,
    6
);

$result: array_merge($list, $list2);
```
Output:
```scss
(
    0: 1,
    1: 2,
    2: 3,
    3: 4,
    4: 5,
    5: 6
)
```