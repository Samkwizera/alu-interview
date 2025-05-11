# Rain

## Problem Description
Given a list of non-negative integers representing walls of width 1, calculate how many square units of water will be retained between walls after it rains.

## Solution
The solution is implemented in `0-rain.py`. The function `rain(walls)` calculates the amount of water that can be trapped between the walls.

### Usage
```python
from 0-rain import rain

# Example usage
walls = [0, 1, 0, 2, 0, 3, 0, 4]
result = rain(walls)
print(result)  # Output: 6
```

### How it works
1. For each position, we need to find the maximum height of walls on both left and right sides
2. The amount of water that can be trapped at each position is the minimum of left and right maximum heights minus the current wall height
3. The total water trapped is the sum of water trapped at each position

### Example
For walls = [0, 1, 0, 2, 0, 3, 0, 4]:
- The water will be trapped between walls of heights 1, 2, 3, and 4
- The total water trapped will be 6 square units 