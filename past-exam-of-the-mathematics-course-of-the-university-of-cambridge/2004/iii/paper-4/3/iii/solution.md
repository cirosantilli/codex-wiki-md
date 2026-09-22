<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First, the images of $a_1^p,\ldots,a_n^p$ span $G_2/G_3$ by the surjective [group homomorphism](../../../../../../group-homomorphism.md) in (ii). Part (i) identifies $G_3$ with $\Phi(G_2)$, so the [Burnside basis theorem](../../../../../../burnside-basis-theorem.md) gives

$$
\boxed{G^p=\langle a_1^p,\ldots,a_n^p\rangle.}
$$

This proves generation by the indicated powers; it does not yet prove that an arbitrary product of powers is itself a power.

For that stronger assertion, let $y\in P_1=G^p$. Part (ii) supplies $x$ with $x^p\equiv y\pmod {P_2}$. Suppose at some stage $x^p\equiv y\pmod {P_{j+1}}$, where $j\geq1$. Apply (ii) to the [powerful p-group](../../../../../../powerful-p-group.md) $P_j$: its first two power layers are $P_{j+1},P_{j+2}$. We can therefore choose $u\in P_j$ with

$$
u^p\equiv(x^p)^{-1}y\pmod {P_{j+2}}.
$$

The preliminary power congruence gives $(xu)^p\equiv y\pmod {P_{j+2}}$. Replacing $x$ by $xu$ improves the root by one layer. The [lower p-series](../../../../../../lower-p-series.md) terminates, so finitely many corrections yield $x^p=y$ exactly. **Every element of $G^p$ is a $p$-th power in $G$.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
