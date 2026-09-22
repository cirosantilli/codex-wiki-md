# Amortized time complexity

↑ **Parent:** [Amortized analysis](amortized-analysis.md)

An [amortized analysis](amortized-analysis.md) can bound the total [time complexity](time-complexity.md) $T(m,n)$ of every allowed [sequence](sequence.md) of $m$ operations by $ma(n)+I(n)$, where $n$ is a size parameter and $I(n)$ accounts for initialization or the specified initial state. The bound $a(n)$ is then an amortized per-operation [time complexity](time-complexity.md). Dividing the total bound by $m$ explains the averaging; it is a guarantee over every permitted [sequence](sequence.md), without an assumed [probability distribution](probability-distribution-split.md) on requests. Individual operations can cost more than $a(n)$.

## ↑ Ancestors (7)

1. [Amortized analysis](amortized-analysis.md)
2. [Time complexity](time-complexity.md)
3. [Complexity class](complexity-class.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/7/b/solution.md)
- [Self-Adjusting Binary Search Trees by Daniel Sleator and Robert Tarjan](self-adjusting-binary-search-trees-by-daniel-sleator-and-robert-tarjan.md)
- [Splay tree](splay-tree.md)
