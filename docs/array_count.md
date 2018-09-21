# array_count

array_count — Count all elements in an array.

#### __Description__

```scss
array_count(mixed $map_or_list) : int
```

#### __Parameters__
map_or_list
- Initial (map or list).

#### __Return Values__
The number of elements in the given array.


#### __Examples__
Example #1 array_count()
```scss
$list:(
    1px,
    5px,
    10px,
    20px
);

$result: array_count($list);
```
Output:
```scss
4
```