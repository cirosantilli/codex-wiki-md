# Maximum all-true rectangle

↑ **Parent:** [Algorithm](algorithm-split.md)

In a [Boolean](boolean-data-type.md) [matrix](matrix.md), find an axis-aligned [rectangle](rectangle.md) containing only true entries and having maximum area. One approach first records each row's consecutive true run ending at each column. For each possible top-right corner, extend downwards, maintaining the minimum run width and maximizing height times width. This uses $O(N^3)$ [time complexity](time-complexity.md) on an $N$ by $N$ [matrix](matrix.md) after $O(N^2)$ preprocessing.

**Table of contents**

- [Row run length](row-run-length.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
