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