# Minimum number of symbols for a permutation of prescribed order

↑ **Parent:** [Order of a permutation](order-of-a-permutation.md)

Write the [prime factorization](fundamental-theorem-of-arithmetic.md) of $m>1$ as $m=q_1\cdots q_t$, with each $q_j$ a positive power of a distinct [prime number](prime-number-split.md). The least $n$ such that $S_n$ contains a [permutation](permutation.md) of order $m$ is $q_1+\cdots+q_t$.

For existence, take [disjoint permutation cycles](disjoint-permutation-cycles.md) of lengths $q_j$. Their [order of a permutation](order-of-a-permutation.md) is the [least common multiple](least-common-multiple.md) of those lengths, namely $m$. For minimality, start with the [disjoint cycle decomposition](disjoint-cycle-decomposition.md) of any [permutation](permutation.md) of order $m$. Assign each full prime-power factor $q_j$ to one cycle whose length is divisible by it; one exists because the [least common multiple](least-common-multiple.md) of all cycle lengths is $m$. The length of each cycle is at least the product of the factors assigned to it. For integers $a,b\geq2$, $ab\geq a+b$, so a product of at least two assigned factors is at least their sum; the assertion is immediate for one factor. Summing over cycles gives at least $\sum_jq_j$ symbols. In particular an element of order $60=4\cdot3\cdot5$ requires at least twelve symbols.

## ↑ Ancestors (6)

1. [Order of a permutation](order-of-a-permutation.md)
2. [Permutation](permutation.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-i/5/d/solution.md)
