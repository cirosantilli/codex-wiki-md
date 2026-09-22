<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Parameterize the second contour by $\zeta=-is$, $s\geq0$. Then

$$
\widetilde F(z)=-i\int_0^\infty\frac{e^{2izs}}{1+is^3}\,ds.
$$

The exponential decays when $\operatorname{Im}z>0$, uniformly on compact subsets of that half-plane. Differentiation under the integral there proves [holomorphy](../../../../../holomorphic-function.md). Thus the maximal open sector of convergence and [holomorphy](../../../../../holomorphic-function.md) in this representation is **$\boxed{\alpha=0,\quad\beta=\pi}$**. The boundary integrals themselves can converge, but that does not enlarge this open analytic sector.

For $0<\arg z<\pi/2$, rotate the original contour clockwise through the fourth quadrant. On a large quarter-circle the integrand is $O(R^{-3})$ times a decaying exponential, so the arc integral tends to zero. The only enclosed pole is $\zeta_0=e^{-i\pi/3}$, and its [residue](../../../../../residue.md) is $e^{-2z\zeta_0}/(3\zeta_0^2)$. The clockwise orientation gives, by the [residue theorem](../../../../../residue-theorem.md),

$$
F(z)-\widetilde F(z)=-2\pi i\frac{e^{-2z\zeta_0}}{3\zeta_0^2}
=-\frac{2\pi i}{3}e^{2\pi i/3}\exp(-2z e^{-i\pi/3}).
$$

Consequently the desired [analytic continuation](../../../../../analytic-continuation.md) for $\pi/2\leq\arg z<\pi$ is

$$
\boxed{F_{\mathrm{cont}}(z)=\widetilde F(z)-\frac{2\pi i}{3}e^{2\pi i/3}\exp(-2z e^{-i\pi/3}).}
$$

Both terms are [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the upper half-plane and the expression agrees with the original function in the overlap, so it is an [analytic continuation](../../../../../analytic-continuation.md). The residue term is essential: the pole lies between the two rays.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
