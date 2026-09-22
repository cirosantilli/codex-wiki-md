<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $D=\partial_\rho A^\rho$. The gauge-fixing variation is

$$
\delta\!\left(-\frac12D^2\right)=-D\partial^\nu\delta A_\nu.
$$

After integration by parts its contribution to the [Euler-Lagrange field equations](../../../../../../euler-lagrange-field-equation.md) is $+\partial^\nu D$. It cancels the $-\partial^\nu D$ from the [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md), giving **$\Box A^\nu=0$ for all four components**. This is the [Feynman gauge](../../../../../../feynman-gauge.md) equation; the physical [Lorenz gauge](../../../../../../lorenz-gauge-condition.md) condition must still be imposed on states rather than inferred as an additional classical equation from this gauge-fixed density.

Treating the covariant components $A_\mu$ as coordinates, the derivative of the actual displayed density with respect to $\partial_0A_\mu$ gives the [canonical momenta](../../../../../../canonical-momentum.md)

$$
\boxed{\pi^\mu=-F^{0\mu}-\eta^{0\mu}D.}
$$

In terms of lower-index spatial coordinates,

$$
\pi^0=-\dot A_0+\partial_iA_i,\qquad
\pi^i=\dot A_i-\partial_iA_0\quad(i=1,2,3).
$$

The [gauge fixing](../../../../../../gauge-fixing.md) has supplied the nonzero momentum of $A_0$, absent from the ungauge-fixed [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md).

There is a boundary-term convention needed for the next part's printed momentum expansion. Direct expansion gives the [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](../../../../../../feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction.md):

$$
\mathcal L=\mathcal L'+\partial_\rho K^\rho,
\qquad\mathcal L'=-\frac12\partial_\rho A_\sigma\partial^\rho A^\sigma,
\qquad K^\rho=\frac12(A_\sigma\partial^\sigma A^\rho-A^\rho D).
$$

To verify it, the difference of the densities is $\tfrac12[(\partial_\rho A_\sigma)(\partial^\sigma A^\rho)-D^2]$; differentiating $K^\rho$ gives these two terms, while the remaining second-derivative terms cancel after renaming indices. The subtracted density has $\widetilde\pi^\mu=-\dot A^\mu$, which is exactly the momentum used by the mode expansion in part (c). The literal momenta asked for here are the boxed expression, not $-\dot A^\mu$. Both densities have the same field equations, and their [canonical commutation relations](../../../../../../canonical-commutation-relation.md) agree through the [boundary-induced canonical transformation in Feynman gauge](../../../../../../boundary-induced-canonical-transformation-in-feynman-gauge.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
