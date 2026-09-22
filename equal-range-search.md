# Equal-range search

↑ **Parent:** [Binary search](binary-search.md)

Find both the [lower-bound search](lower-bound-search.md) boundary $i$ and the [upper-bound search](upper-bound-search.md) boundary $j$ of a key $x$ in a [sorted array](sorted-array.md). Every entry in $[i,j)$ is at least and at most $x$, so all are equal to $x$. Values immediately outside this interval, when present, are strictly smaller or strictly larger; the interval is consequently maximal. An absent key gives $i=j$ at its insertion position. Two [binary searches](binary-search.md) give total [time complexity](time-complexity.md) $O(\log(N+1))$ under constant-cost comparison and indexed access.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/2/d/solution.md)
