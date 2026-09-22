# Ordered word concatenation dynamic programming

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

Given ordered words $w_1,\ldots,w_n$ and a target $s$, minimise the number of words in an order-preserving [subsequence](subsequence.md) whose [concatenation](concatenation.md) is $s$. Let $D(i,j)$ be the optimum using the first $i$ words to produce the first $j$ symbols. Either skip $w_i$, or, when it matches the target suffix ending at $j$, take it and add one to $D(i-1,j-|w_i|)$. The state records both the available-word boundary and target progress, preventing reuse or reordering of words. For $|s|=O(n)$ and bounded word length, this is an $O(n^2)$-time algorithm with straightforward predecessor reconstruction.

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/6/c/solution.md)
