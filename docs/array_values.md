# array_values

array_values — Return all the values of an array.

#### __Description__

```scss
array_values(mixed $map_or_list) : array
```

#### __Parameters__
map_or_list
- Initial (map or list).

#### __Return Values__
An indexed array containing the array values.


#### __Examples__
Example #1 array_values()
```scss
$map:(
    shape: square,
    color: blue
);

$result: array_values($map);
```
Output:
```scss
(
    0: square,
    1: blue
)
```