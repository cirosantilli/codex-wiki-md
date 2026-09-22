# Sorted-coordinate criterion for box containment

↑ **Parent:** [Box nesting](box-nesting.md)

Let $a_1\le\cdots\le a_d$ and $b_1\le\cdots\le b_d$ be the separately sorted dimension vectors. Matching corresponding ranks proves the forward construction when every $a_i<b_i$. Conversely, if $a_k\ge b_k$, then the $d-k+1$ source dimensions from rank $k$ onward require distinct targets strictly larger than $a_k$, but only the last $d-k$ target ranks could qualify. The [pigeonhole principle](pigeonhole-principle.md) rules out such a permutation. Strict inequality matters: equal side lengths do not fit under this convention. Sorting and checking gives an $O(d\log d)$ decision [algorithm](algorithm-split.md).

## ↑ Ancestors (6)

1. [Box nesting](box-nesting.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Box nesting](box-nesting.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/d/i/solution.md)
