<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** We prove [weak-star topology on an entire infinite-dimensional Banach dual is not metrizable](../../../../../../weak-star-topology-on-an-entire-infinite-dimensional-banach-dual-is-not-metrizable.md). Suppose instead that $E'$ has a countable local base $(W_n)$ at zero. Choose a basic [weak-star topology](../../../../../../weak-star-topology.md) neighbourhood $U_n\subseteq W_n$, with its conditions involving a finite set $S_n\subseteq E$. The $U_n$ still form a local base.

For any $x\in E$, the set $\{\phi:|\phi(x)|<1\}$ is a neighbourhood of zero, so some $U_n$ is contained in it. Every functional annihilating $S_n$, and every scalar multiple of that functional, belongs to $U_n$. Consequently every such functional also annihilates $x$. This forces

$$
x\in\operatorname{span}S_n.
$$

Indeed a finite-dimensional span is norm closed, and the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) supplies a [bounded linear functional](../../../../../../continuous-linear-functional.md) vanishing on it and nonzero at any point outside it.

It follows that $E=\bigcup_n\operatorname{span}S_n$. Each span is a proper finite-dimensional closed [vector subspace](../../../../../../vector-subspace.md) and has empty interior in the infinite-dimensional [Banach space](../../../../../../banach-space-split.md) $E$. This contradicts the [Baire category theorem](../../../../../../baire-category-theorem.md). Hence

$$
\boxed{E'\text{ with its weak-star topology is not metrizable}.}
$$

The uniform norm bound that made the metric work on $B'$ is absent on the whole dual. The answers to (i), (ii), (iii) and (iv) are therefore **all true**.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
