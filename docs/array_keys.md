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
$list:(
    go,
    stop
);

$result: array_keys($list);
```
Output:
```scss
(
    0: 0,
    1: 1
)
```
\
Example #2 array_keys()
```scss
$map:(
    colors: (primary: blue, secondary: red)
);

$result: array_get($map, 'colors.primary');
```
Output:
```scss
blue
```