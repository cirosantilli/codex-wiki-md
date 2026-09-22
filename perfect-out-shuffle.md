# Perfect out-shuffle

↑ **Parent:** [Permutation](permutation.md)

Interleave the two equal halves of an even finite [list](list-abstract-data-type.md), placing the first half's next entry before the second half's next entry. With zero-based positions and length $n>2$, position $i<n-1$ moves to $2i\bmod(n-1)$, and the last position stays fixed. For an index in the first half the new position is $2i$; in the second it is $2i-(n-1)$, proving the formula. The least positive period of the whole [permutation](permutation.md) is the [multiplicative order](multiplicative-order.md) of $2$ modulo $n-1$: equality of the multiplier to one fixes every position, and fixing position one requires that equality. In particular, a 52-entry [list](list-abstract-data-type.md) has period eight. The empty and two-entry cases are identity [permutations](permutation.md) with least positive period one.

## ↑ Ancestors (5)

1. [Permutation](permutation.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/4/c/solution.md)
