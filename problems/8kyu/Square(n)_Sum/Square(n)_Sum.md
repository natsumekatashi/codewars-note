# 8kyu Square(n) Sum

---

## Instructions
Complete the square sum function so that it squares each number passed into in and then sums the results together.

For example, for `[1, 2, 3]` it should return `9` because $1^2 + 2^2 + 2^2 = 9$.

---

完善 square sum 函数，使其对传入的每个数字进行平方运算，然后将结果相加。

例如，对 `[1, 2, 3]`，它应该返回 `9`，因为 $1^2 + 2^2 + 2^2 = 9$。

## Solution

### C++

```cpp
#include <vector>

int square_sum(const std::vector<int>& numbers)
{
    int res = 0;
    for (int number : numbers)
    {
        res += number * number;
    }
    return res;
}
```

### Python

```python
def square_sum(numbers):
    return sum([n ** 2 for n in numbers])
```