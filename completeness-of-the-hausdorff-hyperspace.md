# Completeness of the Hausdorff hyperspace

↑ **Parent:** [Hausdorff distance](hausdorff-distance.md)

For any nonempty [complete metric space](complete-metric-space.md) $X$, the family of its nonempty [closed](closed-set.md) bounded subsets is a [complete metric space](complete-metric-space.md) under the [Hausdorff distance](hausdorff-distance.md). Boundedness of the entire ambient space is unnecessary in this general form.

For a [Cauchy sequence](cauchy-sequence.md) $(F_n)$ of these sets, define $A_n=\overline{\bigcup_{m\geq n}F_m}$ and $\delta_n=\sup_{p,q\geq n}d_H(F_p,F_q)$. A [Cauchy sequence](cauchy-sequence.md) in any [metric space](metric-space.md) is bounded, so its tail sets are contained in a common finite-radius neighbourhood of one bounded $F_N$; hence every $A_n$ is bounded. The [distance to a set](distance-to-a-set.md) is one-[Lipschitz](lipschitz-continuity.md), so estimates pass to the [closure](closure-topology.md), giving $d_H(F_n,A_n)\leq\delta_n$ and $d_H(A_n,A_m)\leq\delta_n$ for $m\geq n$. Choose $n_j$ with $\delta_{n_j}\leq2^{-j}$. The [Summably nested Hausdorff intersection theorem](summably-nested-hausdorff-intersection-theorem.md) gives $A_{n_j}\to G\ne\varnothing$. The [triangle inequality](triangle-inequality.md) now gives $F_n\to G$, proving [completeness](completeness.md).

## ↑ Ancestors (7)

1. [Hausdorff distance](hausdorff-distance.md)
2. [Metric space](metric-space.md)
3. [Topological analysis](topological-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2023/1/b/iii/solution.md)
