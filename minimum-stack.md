# Minimum stack

↑ **Parent:** [Stack (data structure)](stack-data-structure.md)

A [stack](stack-data-structure.md) supporting access to its [minimum](minimum-of-a-subset-of-a-total-order.md) in constant [time complexity](time-complexity.md) when its contents are nonempty. Each [linked list node](linked-list-node.md) stores its value and the minimum of the suffix beginning there. Pushing computes one new cached minimum; popping reveals the previous cached minimum. Keeping one cached value per node handles repeated minima without a special case.

## ↑ Ancestors (4)

1. [Stack (data structure)](stack-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/5/a/solution.md)
