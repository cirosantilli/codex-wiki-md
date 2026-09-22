<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [orthogonal group](../../../../../../orthogonal-group.md) acts transitively on unoriented lines in $\mathbb R^n$. The stabilizer of the line spanned by the first coordinate is

$$
\boxed{H=\{\operatorname{diag}(\epsilon,A):\epsilon\in O(1),\ A\in O(n-1)\}\cong O(1)\times O(n-1).}
$$

Thus $G/H=\mathbb{RP}^{n-1}$; using only $O(n-1)$ would stabilize a vector and give a sphere instead. For the universal contractible free $G$-space $EG$, the associated bundle $EG/H\to EG/G$ gives the [Serre fibration](../../../../../../serre-fibration.md) $G/H\to BH\to BG$. Its total space identifies up to [homotopy](../../../../../../homotopy.md) with $BO(1)\times BO(n-1)$.

If $n$ is odd, $n-1$ is even and the rational [cohomology](../../../../../../cohomology-split.md) of $\mathbb{RP}^{n-1}$ is just $\mathbb Q$ in degree zero. This follows from the integral projective cellular differentials, alternating zero and multiplication by two, with the even-dimensional top class killed rationally. The cohomological [Serre spectral sequence](../../../../../../serre-spectral-sequence.md) therefore has only the row

$$
E_2^{p,0}=H^p(BO(n);\mathbb Q),
$$

with all other rows zero. The local system in degree zero is trivial because the fiber is connected. There can be no differential or extension, and the multiplicative edge map $H^*(BO(n);\mathbb Q)\to H^*(BH;\mathbb Q)$ is an isomorphism of rings.

Also $BO(1)=\mathbb{RP}^{\infty}$ has rational [cohomology](../../../../../../cohomology-split.md) $\mathbb Q$ in degree zero only, by the same cellular calculation. The [Künneth theorem](../../../../../../kunneth-theorem.md) identifies $H^*(BH;\mathbb Q)$ with $H^*(BO(n-1);\mathbb Q)$. The inclusion fixing the first coordinate factors through $H$, setting its $O(1)$ coordinate to one; hence the resulting isomorphism is the actual restriction along this inclusion:

$$
\boxed{H^*(BO(n);\mathbb Q)\xrightarrow{\cong}H^*(BO(n-1);\mathbb Q)\qquad(n\text{ odd}).}
$$

This includes $n=1$, with $BO(0)$ a point, and proves [rational odd-rank stabilization of orthogonal classifying spaces](../../../../../../rational-odd-rank-stabilization-of-orthogonal-classifying-spaces.md).

For even $n$, the fiber is odd-dimensional real projective space and has a further rational class in degree $n-1$. The spectral sequence has a possible additional row, now with determinant-sign local coefficients: an orientation-reversing [orthogonal matrix](../../../../../../orthogonal-matrix.md) acts with degree $-1$ on the covering sphere and hence on the odd-dimensional projective space. Therefore the one-row collapse argument is unavailable; this top row must not be treated as automatically untwisted.

There is an actual failure of injectivity in every even rank. Write $n=2m$. The universal class $p_m\in H^{4m}(BO(2m);\mathbb Q)$ is nonzero: pull the universal bundle back to the sum of the real underlying bundles of $m$ complex lines over $(\mathbb{CP}^{\infty})^m$. If their first [Chern classes](../../../../../../chern-class.md) are $x_j$, the Pontryagin formula $p_m(E)=(-1)^mc_{2m}(E\otimes\mathbb C)$ gives $p_m=\prod_jx_j^2\ne0$. On $BO(2m-1)$ the restricted bundle is $\varepsilon^1\oplus\gamma_{2m-1}$; its top complex [Chern class](../../../../../../chern-class.md) $c_{2m}$ vanishes by the rank bound and the trivial summand. Thus $p_m$ restricts to zero. The natural restriction is not injective for even $n$, as the extra fiber [cohomology](../../../../../../cohomology-split.md) already warns.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
