# array_merge

array_merge — Merge two datasets.

#### __Description__

```scss
array_merge(mixed $array_or_list, mixed $array_or_list_2) : array
```

#### __Parameters__
array_or_list
- Initial array or list to merge.
  
array_or_list_2
- Array or list to merge into first parameter.

#### __Return Values__
An array containing the result of two merged arrays.


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


