# Minimum Operations

## Problem Description
In a text file, there is a single character H. Your text editor can execute only two operations in this file: Copy All and Paste. Given a number n, write a method that calculates the fewest number of operations needed to result in exactly n H characters in the file.

## Solution
The solution is implemented in `0-minoperations.py`. The function `minOperations(n)` calculates the minimum number of operations needed to achieve n H characters.

### Usage
```python
from 0-minoperations import minOperations

# Example usage
n = 9
result = minOperations(n)
print(result)  # Output: 6
```

### How it works
1. If n is less than or equal to 1, return 0 as no operations are needed
2. For n > 1, we find the prime factors of n
3. The sum of the prime factors gives us the minimum number of operations needed

### Example
For n = 9:
- Prime factors: 3 * 3
- Operations needed: 3 + 3 = 6 