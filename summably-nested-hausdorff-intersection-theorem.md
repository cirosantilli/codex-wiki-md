# Summably nested Hausdorff intersection theorem

↑ **Parent:** [Hausdorff distance](hausdorff-distance.md)

Let $X$ be a [complete metric space](complete-metric-space.md) and let $F_n$ be nonempty [closed](closed-set.md) bounded subsets with $F_{n+1}\subseteq F_n$ and [Hausdorff distance](hausdorff-distance.md) $d_H(F_n,F_{n+1})\leq a_n$, where $a_n\geq0$ and $\sum_n a_n<\infty$. Then $G=\bigcap_n F_n$ is nonempty and [closed](closed-set.md), and $d_H(F_n,G)\leq\sum_{k=n}^{\infty}a_k\to0$.

To prove this, start with any $x_n\in F_n$ and choose $x_{k+1}\in F_{k+1}$ with $d(x_k,x_{k+1})<a_k+\eta2^{n-k-1}$. The [triangle inequality](triangle-inequality.md) makes the resulting sequence a [Cauchy sequence](cauchy-sequence.md). Its limit exists by [completeness](completeness.md) and belongs to every $F_j$ by nesting and closedness. Its distance from the starting point is at most $\sum_{k=n}^{\infty}a_k+\eta$. Let $\eta\downarrow0$ and take the [supremum](supremum.md) over starting points. The reverse directed distance is zero since $G\subseteq F_n$. Unlike the usual shrinking-diameter form of [Cantor's intersection theorem](cantor-s-intersection-theorem.md), the sets need not have diameters tending to zero.

## ↑ Ancestors (7)

1. [Hausdorff distance](hausdorff-distance.md)
2. [Metric space](metric-space.md)
3. [Topological analysis](topological-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Completeness of the Hausdorff hyperspace](completeness-of-the-hausdorff-hyperspace.md)
- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2023/1/b/ii/solution.md)
