# Consecutive sum divisible by the sequence length

↑ **Parent:** [Pigeonhole principle](pigeonhole-principle.md)

For any [sequence](sequence.md) of $n\geq1$ [integers](integer-split.md), some nonempty consecutive block has sum divisible by $n$. Form the $n+1$ [prefix sums](prefix-sum.md) $s_0=0,s_j=\sum_{k=1}^ja_k$. There are only $n$ [residue classes](residue-class.md) modulo $n$, so the [pigeonhole principle](pigeonhole-principle.md) gives $s_i\equiv s_j\pmod n$ for some $i<j$. [Subtraction](subtraction.md) proves that $s_j-s_i$ is the required block sum. Negative entries and repeated entries cause no difficulty. Applied after any ordering of a [finite set](finite-set.md), it also gives a nonempty [subset](subset.md) whose sum is divisible by the size of the [set](set-split.md).

## ↑ Ancestors (5)

1. [Pigeonhole principle](pigeonhole-principle.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/3/e/solution.md)
