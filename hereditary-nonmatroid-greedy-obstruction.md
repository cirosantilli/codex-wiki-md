# Hereditary nonmatroid greedy obstruction

↑ **Parent:** [Independence system](independence-system.md)

On the [ground set](ground-set.md) $E=\{x,y,z\}$, permit exactly

$$
\mathcal F=\{\varnothing,\{x\},\{y\},\{z\},\{y,z\}\},
\qquad w(x)=10,\quad w(y)=w(z)=6.
$$

This lists every admissible [subset](subset.md); the excluded [subsets](subset.md) are $\{x,y\}$, $\{x,z\}$, and $\{x,y,z\}$. It is an [independence system](independence-system.md): deleting elements from $\{y,z\}$ produces its listed singletons or the [empty set](empty-set.md), and deleting from a singleton produces the [empty set](empty-set.md). But $I=\{x\}$ and $J=\{y,z\}$ violate exchange: neither $y$ nor $z$ can be added to $I$. Thus it is not a [matroid](matroid.md).

The descending-weight [greedy algorithm](greedy-algorithm.md) admits $x$ first, then rejects both $y$ and $z$, returning $\{x\}$ with weight $10$. Exchanging the tied order of $y,z$ changes nothing. The admissible pair $\{y,z\}$ weighs $12$, exceeding every singleton and the [empty set](empty-set.md), so it is the true optimum. Both $\{x\}$ and $\{y,z\}$ are [maximal elements](maximal-element-of-a-partially-ordered-set.md) under inclusion of [subsets](subset.md), but only the pair has maximum [cardinality](cardinality.md). This identifies exactly where the [matroid greedy algorithm](matroid-greedy-algorithm.md) loses its guarantee: heredity preserves admissibility under deletions, while exchange prevents a locally maximal selection from being too small.

## ↑ Ancestors (6)

1. [Independence system](independence-system.md)
2. [Combinatorial structure](combinatorial-structure.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Basis of a matroid](basis-of-a-matroid.md)
- [Independence system](independence-system.md)
