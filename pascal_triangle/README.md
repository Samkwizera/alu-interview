# Pascal's Triangle

## Problem Description
Create a function that returns a list of lists of integers representing the Pascal's triangle of n.

## Solution
The solution is implemented in `0-pascal_triangle.py`. The function `pascal_triangle(n)` generates Pascal's triangle up to n rows.

### Usage
```python
from 0-pascal_triangle import pascal_triangle

# Example usage
n = 5
result = pascal_triangle(n)
print(result)
# Output: [[1], [1, 1], [1, 2, 1], [1, 3, 3, 1], [1, 4, 6, 4, 1]]
```

### How it works
1. If n <= 0, return an empty list
2. Start with the first row [1]
3. For each subsequent row:
   - Start with 1
   - Calculate middle numbers by adding adjacent numbers from the previous row
   - End with 1

### Example
For n = 5, the output will be:
```
[
    [1],
    [1, 1],
    [1, 2, 1],
    [1, 3, 3, 1],
    [1, 4, 6, 4, 1]
]
``` 