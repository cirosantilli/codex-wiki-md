# Balanced component cut

↑ **Parent:** [Graph cut](graph-cut.md)

If every [graph component](component-graph-theory.md) has at most $(k+1)n/[k(2k+1)]$ [vertices](vertex-graph-theory.md), assigning whole [graph components](component-graph-theory.md) to two sides gives an empty [graph cut](graph-cut.md) with the displayed bound. To prove it, maximize the smaller side's weight $S\leq n/2$. If $S<kn/(2k+1)$, every component on the larger side has weight at least $n-2S$, because moving a smaller one would improve the smaller side. There are at least $k+1$ such components, since their total exceeds $k$ times the permitted maximum weight. Thus $n-S\geq(k+1)(n-2S)$, a contradiction. The proof also works for arbitrary positive weights.

## ↑ Ancestors (7)

1. [Graph cut](graph-cut.md)
2. [Graph](graph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/5/i/solution.md)
- [Simultaneous giant for fixed random-edge choice](simultaneous-giant-for-fixed-random-edge-choice.md)
