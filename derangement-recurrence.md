# Derangement recurrence

↑ **Parent:** [Derangement of a permutation](derangement-of-a-permutation.md)

The number $d_n$ of [derangements](derangement-of-a-permutation.md) of an $n$-element [set](set-split.md) satisfies $d_0=1$, $d_1=0$, $d_2=1$ and the displayed [recurrence relation](recurrence-relation.md) for $n\ge2$. Choose the image $j$ of a distinguished element, in $n-1$ ways. If those two elements form a two-cycle, removing them leaves $d_{n-2}$ choices. Otherwise remove the distinguished element from its longer [permutation cycle](permutation-cycle.md), leaving a [derangement](derangement-of-a-permutation.md) on $n-1$ elements. The inverse operation inserts it immediately before $j$. Thus the two disjoint cases contribute $d_{n-2}+d_{n-1}$ for each $j$.

## ↑ Ancestors (6)

1. [Derangement of a permutation](derangement-of-a-permutation.md)
2. [Permutation](permutation.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/3/a/ii/solution.md)
