# Upper-bound search

↑ **Parent:** [Binary search](binary-search.md)

For a [sorted array](sorted-array.md) $a[0..N)$, find the unique boundary $p\in[0,N]$ with $a[0..p)\leq x<a[p..N)$. A [binary search](binary-search.md) maintains $0\leq l\leq r\leq N$, an excluded prefix $a[0..l)\leq x$, and an excluded suffix $x<a[r..N)$. At an interior midpoint $m$, replace $l$ by $m+1$ when $a(m)\leq x$, and otherwise replace $r$ by $m$. [Sortedness](sortedness.md) preserves the [loop invariant](loop-invariant.md); the width $r-l$ is a decreasing [loop variant](loop-variant.md). Termination at $l=r$ gives the boundary, including $p=0$ and $p=N$. The [time complexity](time-complexity.md) is $O(\log(N+1))$ with constant-cost comparisons and indexed access. Unlike searching for $x+1$, this formulation does not risk [integer overflow](integer-overflow.md) at the largest representable key.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Equal-range search](equal-range-search.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/2/c/solution.md)
