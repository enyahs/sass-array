# array_keys

array_keys — Return all the keys of an array.

#### __Description__

```scss
array_keys(mixed $map_or_list) : array
```

#### __Parameters__
map_or_list
- Initial (map or list).

#### __Return Values__
An indexed array containing the array keys.


#### __Examples__
Example #1 array_keys()
```scss
$map:(
    shape: square,
    color: blue
);

$result: array_keys($map);
```
Output:
```scss
(
    0: shape,
    1: color
)
```