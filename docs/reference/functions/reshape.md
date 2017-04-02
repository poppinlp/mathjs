<!-- Note: This file is automatically generated from source code comments. Changes made in this file will be overridden. -->

# Function reshape

Reshape a multi dimensional array to fit the specified dimensions


## Syntax

```js
math.reshape(x, sizes)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`x` | Array &#124; Matrix &#124; * | Matrix to be reshaped
`sizes` | number[] | One dimensional array with integral sizes for each dimension

### Returns

Type | Description
---- | -----------
* &#124; Array &#124; Matrix | A reshaped clone of matrix `x`


## Examples

```js
math.reshape([1, 2, 3, 4, 5, 6], [2, 3]);
// returns Array  [[1, 2, 3], [4, 5, 6]]

math.reshape([[1, 2], [3, 4]], [1, 4]);
// returns Array  [[1, 2, 3, 4]]

math.reshape([[1, 2], [3, 4]], [4]);
// returns Array [1, 2, 3, 4]

var x = math.matrix([1, 2, 3, 4, 5, 6, 7, 8]);
math.reshape(x, [2, 2, 2]);
// returns Matrix [[[1, 2], [3, 4]], [[5, 6], [7, 8]]]
```


## See also

[size](size.md),
[squeeze](squeeze.md),
[resize](resize.md)