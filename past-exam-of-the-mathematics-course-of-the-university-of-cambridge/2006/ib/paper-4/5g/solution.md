<h1 id="5g/solution">Solution</h1>

↑ **Parent:** [5G](../5g.md)

Write $\mu=\cos\theta$. Separation of the axisymmetric [Laplace equation](../../../../../laplace-equation.md) in [spherical coordinates](../../../../../spherical-coordinate-system.md), with regularity at the poles, gives the [Legendre polynomial](../../../../../legendre-polynomial.md) expansion

$$
f_-(r,\theta)=\sum_{\ell=0}^\infty a_\ell r^\ell P_\ell(\mu),\qquad
f_+(r,\theta)=\sum_{\ell=0}^\infty b_\ell r^{-\ell-1}P_\ell(\mu).
$$

The discarded interior terms are singular at the origin; the discarded exterior terms fail the prescribed decay at infinity. Continuity at $r=1$ gives $a_\ell=b_\ell=c_\ell$.

Take the radial derivative jump to mean the exterior derivative minus the interior derivative. Then

$$
\partial_r f_+-\partial_r f_-=-\sum_{\ell\geq0}(2\ell+1)c_\ell P_\ell(\mu).
$$

Since $1-\mu^2=\frac23(P_0(\mu)-P_2(\mu))$, comparison with the prescribed jump gives $c_0=-2A/3$, $c_2=2A/15$, and all other coefficients zero. Thus

$$
\boxed{f_-(r,\theta)=-\frac{2A}{3}+\frac{2A}{15}r^2P_2(\cos\theta),\qquad
f_+(r,\theta)=-\frac{2A}{3r}+\frac{2A}{15r^3}P_2(\cos\theta).}
$$

These expressions satisfy the [Laplace equation](../../../../../laplace-equation.md), continuity, regularity and decay, and their jump is $A\sin^2\theta$. If the opposite convention for the word jump is chosen, both expressions change sign. Although only the axisymmetric expansion is needed, no additional nonaxisymmetric solution can be added: zero jump and continuity glue such an addition into an everywhere regular harmonic function decaying at infinity, which vanishes by the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md).

## ↑ Ancestors (10)

1. [5G](../5g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
