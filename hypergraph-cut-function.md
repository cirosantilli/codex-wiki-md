# Hypergraph cut function

↑ **Parent:** [Hypergraph](hypergraph-split.md)

For a [weighted hypergraph](weighted-hypergraph.md), the [hypergraph cut function](hypergraph-cut-function.md) totals the weights of [hyperedges](hyperedge.md) meeting both a [subset](subset.md) and its complement. It is a [normalised set function](normalised-set-function.md) and a [symmetric set function](symmetric-set-function.md). With nonnegative weights it is a [nonnegative function](nonnegative-function.md) and a [submodular set function](submodular-set-function.md). It is generally not a [monotone set function](monotone-set-function.md): a single two-element [hyperedge](hyperedge.md) of weight one has cut value one on either [singleton](singleton-mathematics.md), but zero on the whole [ground set](ground-set.md).

**Proof of [submodularity](submodular-set-function.md) for nonnegative weights.** For one [hyperedge](hyperedge.md) $e$ of size at least two, let $q_e$ indicate whether it is split. Adding $x\notin e$ has zero [marginal increment](marginal-increment-of-a-set-function.md). For $x\in e$, with $x\notin S$, the [marginal increment](marginal-increment-of-a-set-function.md) is $1$ if $S\cap(e\setminus\{x\})$ is empty, $-1$ if it equals $e\setminus\{x\}$, and zero otherwise. These values can only decrease under inclusion of $S$. Thus [diminishing returns](diminishing-returns-characterization-of-submodularity.md) holds for $q_e$, and taking a nonnegative weighted sum preserves it. For a [singleton](singleton-mathematics.md) or empty [hyperedge](hyperedge.md), $q_e$ is identically zero. A negative-weight two-element [hyperedge](hyperedge.md) gives a counterexample to [submodularity](submodular-set-function.md): its two [singleton](singleton-mathematics.md) values sum to a negative number, while the values at their [union](set-union.md) and [intersection](set-intersection.md) are zero.

## ↑ Ancestors (6)

1. [Hypergraph](hypergraph-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Hypergraph cut function](hypergraph-cut-function.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/d/i/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/d/iv/solution.md)
- [Symmetric set function](symmetric-set-function.md)
- [Weighted hypergraph](weighted-hypergraph.md)
