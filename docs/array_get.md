# array_get

array_get — Get a value in an array from the given key path.

#### __Description__

```scss
array_get(mixed $map_or_list, string $path) : mixed
```

#### __Parameters__
map_or_list
- Initial (map or list).

path
- Key path of initial (map or list) seperated with dot notation.

#### __Return Values__
An indexed array containing the array values.


#### __Examples__
Example #1 array_get()
```scss
$list:(
    1px,
    2px,
    5px
);

$result: array_get($list, '0');
```
Output:
```scss
blue
```
\
Example #2 array_get()
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
\
Example #3 array_get()
```scss
$map:(
    small: (1px, 3px, 5px),
    large: (10px, 30px 50px)
);

$result: array_get($map, 'small.1');
```
Output:
```scss
3px
```