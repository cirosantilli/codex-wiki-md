<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

An action assigns each $g\in G$ a [homeomorphism](../../../../../homeomorphism.md) of $X$, with $e\cdot x=x$ and $g\cdot(h\cdot x)=(gh)\cdot x$. For the covering assertion use a properly discontinuous free action: every $x$ has an open neighbourhood $U$ such that $gU\cap U=\varnothing$ for every $g\ne e$. Then the translates $gU$ are pairwise disjoint. The [quotient map](../../../../../quotient-map.md) $p$ is open because $p^{-1}(p(U))=\bigcup_g gU$ is open. Each restriction $p:gU\to p(U)$ is a continuous open bijection and hence a [homeomorphism](../../../../../homeomorphism.md). Thus $p(U)$ is evenly covered and **$p:X\to X/G$ is a [covering map](../../../../../covering-space.md)**.

For the surjective [homomorphism](../../../../../homomorphism.md) one additionally needs $X$ path connected; choose $x_0$ and its image $y_0$. Lift a based loop at $y_0$ from $x_0$. Its endpoint has a unique form $gx_0$. Homotopy lifting makes this assignment well-defined on the [fundamental group](../../../../../fundamental-group.md). With concatenation meaning first the first loop and then the second, the second lift from $gx_0$ is $g$ times the lift from $x_0$, so the endpoint is $ghx_0$. This proves the [homomorphism](../../../../../homomorphism.md) property. For each $g$, a path in $X$ from $x_0$ to $gx_0$ projects to a loop realizing $g$. Hence

$$
\boxed{\pi_1(X/G,y_0)\twoheadrightarrow G.}
$$

Pointwise freeness alone is insufficient for a covering: an irrational rotation action of $\mathbb Z$ on the circle is free but its orbits are dense. Path connectedness is also essential for the final surjectivity claim as written: the discrete space $X=G$ with left translation is a free properly discontinuous action whose quotient is a point, and its trivial [fundamental group](../../../../../fundamental-group.md) cannot surject onto nontrivial $G$. The proof supplies the standard connected covering-space interpretation rather than hiding these hypotheses.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
