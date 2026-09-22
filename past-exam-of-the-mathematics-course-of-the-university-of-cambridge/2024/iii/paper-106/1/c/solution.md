<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $X$ is reflexive, then $X^*$ is reflexive. The weak topology $\sigma(X^*,X^{**})$ and [weak-star topology](../../../../../../weak-star-topology.md) $\sigma(X^*,X)$ therefore coincide under the canonical identification $X^{**}=X$. Thus every weak-star convergent sequence in $X^*$ is weakly convergent, so $X$ is a [Grothendieck space](../../../../../../grothendieck-space.md).

Conversely, suppose that $X$ is separable and Grothendieck. The [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) and [weak-star metrizability of the dual ball](../../../../../../weak-star-metrizability-of-the-dual-ball.md) make $B_{X^*}$ weak-star compact and metrizable, hence weak-star sequentially compact. Every convergent subsequence is weakly convergent by the Grothendieck property. Thus $B_{X^*}$ is weakly sequentially compact. The stated converse to part (a), equivalently the other direction of the [Eberlein-Šmulian theorem](../../../../../../eberlein-smulian-theorem.md), makes $B_{X^*}$ weakly compact. Hence $X^*$ is reflexive, and therefore so is $X$.

Finally let $T:X\to Y$ be bounded and onto, with $X$ Grothendieck, and suppose $y_n^*\to y^*$ weak-star in $Y^*$. Then

$$
T^*y_n^*\longrightarrow T^*y^*
$$

weak-star in $X^*$, hence weakly. The [open mapping theorem](../../../../../../open-mapping-theorem-functional-analysis.md) implies that $T^*:Y^*\to X^*$ is an isomorphism onto its closed range. Given $y^{**}\in Y^{**}$, the functional

$$
T^*y^*\longmapsto y^{**}(y^*)
$$

is bounded on $T^*(Y^*)$ and extends by the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) to some $x^{**}\in X^{**}$. Therefore

$$
y^{**}(y_n^*)=x^{**}(T^*y_n^*)longrightarrow x^{**}(T^*y^*)=y^{**}(y^*).
$$

This is weak convergence in $Y^*$, so $Y$ is Grothendieck.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
