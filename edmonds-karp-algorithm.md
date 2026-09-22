<h1 id="edmonds-karp-algorithm">Edmonds–Karp algorithm</h1>

↑ **Parent:** [Maximum flow problem](maximum-flow-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edmonds–Karp_algorithm)

This [maximum flow](maximum-flow-problem.md) algorithm repeatedly augments along a shortest residual path found by [Breadth-first search](breadth-first-search.md). Residual distances from the source never decrease. If the same arc becomes saturated again after being restored by a reverse augmentation, the distance to its tail has increased by at least two. Thus each arc is critical only $O(|V|)$ times, yielding $O(|V||E|)$ augmentations. Each search costs $O(|E|)$, so the total time is $O(|V||E|^2)$. Termination with no residual source-sink path supplies a [max-flow min-cut theorem](max-flow-min-cut-theorem.md) certificate.

## ↑ Ancestors (7)

1. [Maximum flow problem](maximum-flow-problem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/b/solution.md)
- [Polynomial-time algorithm](polynomial-time-algorithm.md)
