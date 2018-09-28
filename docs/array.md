# array

array — Create an array.

#### __Description__

```scss
array(mixed $map_or_list) : array
```

#### __Parameters__
map_or_list
- Initial (map or list).

#### __Return Values__
The initial map or list converted to an array.


#### __Examples__
Example #1 array()
```scss
$list:(
    10,
    5,
    0
);

$result: array($list);
```
Output:
```scss
(
    0: 10,
    1: 5,
    2: 0
)
```
\
Example #2 array()
```scss
$map:(
    list1: (1, 2, 3),
    list2: (4, 5, 6)
);

$result: array($map);
```
Output:
```scss
(
    list1: (
        0: 1,
        1: 2,
        2: 3
    ),
    list2: (
        0: 4,
        1: 5,
        2: 6
    )
)
```