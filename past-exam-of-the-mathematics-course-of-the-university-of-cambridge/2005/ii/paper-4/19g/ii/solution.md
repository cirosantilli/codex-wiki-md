<h1 id="19g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the standard two-dimensional [representation](../../../../../../group-representation.md), $t_\theta$ has [eigenvalues](../../../../../../eigenvalue.md) $e^{i\theta},e^{-i\theta}$. Its $m$th [symmetric power](../../../../../../symmetric-power.md) has monomial basis $X^{m-j}Y^j$, $j=0,\ldots,m$, of weights $m-2j$. The [character](../../../../../../character-of-a-representation.md) is therefore

$$
\boxed{\chi_m(t_\theta)=\sum_{j=0}^m e^{i(m-2j)\theta}
=\frac{\sin((m+1)\theta)}{\sin\theta}}.
$$

The quotient is interpreted by [continuity](../../../../../../continuous-function.md) at $0,\pi$, where its values are $m+1$ and $(-1)^m(m+1)$.

Apply the [Weyl integration formula for SU2](../../../../../../weyl-integration-formula-for-su-2.md) to the [character](../../../../../../character-of-a-representation.md) product:

$$
\langle\chi_m,\chi_n\rangle
=\frac2\pi\int_0^\pi
\sin((m+1)\theta)\sin((n+1)\theta)\,d\theta
=\delta_{mn}.
$$

The last equality follows directly by product-to-sum integration. A finite-dimensional [representation](../../../../../../group-representation.md) of a [compact](../../../../../../compact-space.md) group decomposes into [irreducibles](../../../../../../irreducible-representation.md), and the squared [character](../../../../../../character-of-a-representation.md) [norm](../../../../../../norm.md) is the sum of squared multiplicities. Since this [norm](../../../../../../norm.md) is one, there is exactly one constituent with multiplicity one. Thus **every [symmetric power](../../../../../../symmetric-power.md) is [irreducible](../../../../../../irreducible-representation.md)**, and the different powers are pairwise inequivalent.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19G](../../19g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
