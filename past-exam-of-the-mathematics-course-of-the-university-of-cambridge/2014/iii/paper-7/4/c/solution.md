<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $F=F_N$ and integrate the [Kac master equation](../../../../../../kac-master-equation.md) over $v_2,\ldots,v_N$. For a pair $i,j\geq2$, the rotation acts only on integrated variables. Its unit [Jacobian determinant](../../../../../../jacobian-determinant.md) makes the integrated gain identical to the integrated loss, so all those pairs cancel.

The only remaining pairs are $(1,j)$, $j=2,\ldots,N$. For such a pair, first integrate over every variable except $v_1$ and $v_j$. This yields the corresponding two-coordinate [marginal distribution](../../../../../../marginal-distribution.md) evaluated at the rotated pair. Permutation symmetry of $F_N$ makes all $N-1$ resulting [integrals](../../../../../../integral.md) identical to the one for $(1,2)$. The coefficient is

$$
 \frac{N(N-1)}{2\pi\binom N2}=\frac1\pi.
$$

Consequently the [Kac marginal evolution equation](../../../../../../kac-marginal-evolution-equation.md) is

$$
 \boxed{\partial_t\Pi_1(F_N)(v_1)
 =\frac1\pi\int_{\mathbb R}\int_0^{2\pi}
 \left[\Pi_2(F_N)(v_1\cos\theta+v_2\sin\theta,
 -v_1\sin\theta+v_2\cos\theta)-\Pi_2(F_N)(v_1,v_2)\right]d\theta\,dv_2.}
$$

The time argument has been suppressed on the right. The loss is consistent with normalization, since $\int\Pi_2(v_1,v_2)dv_2=\Pi_1(v_1)$. Under the printed definition $k<N$, this use of $\Pi_2$ requires $N\geq3$. For $N=2$ the same formula holds with the natural extension $\Pi_N(F_N)=F_N$.

This identity is exact and generally unclosed. Replacing the two-coordinate [marginal distribution](../../../../../../marginal-distribution.md) by the product of one-coordinate marginals would produce the quadratic collision equation associated with [Kac chaos](../../../../../../kac-chaos.md). Permutation symmetry alone does not imply that product approximation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
