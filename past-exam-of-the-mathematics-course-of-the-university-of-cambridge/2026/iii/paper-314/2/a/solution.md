<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p=K\rho^{1+1/m}$. [Hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) in the uniform gravitational field gives

$$
\frac{dp}{dz}=-\rho g.
$$

Substitution and integration with $\rho=0$ at $z=0$ gives

$$
\rho=\rho_0\left(\frac{-z}{H}\right)^m,
\qquad z\leq0,
$$

where $H$ fixes the normalization. Integrating the hydrostatic equation from $z$ to the free surface gives the pressure directly:

$$
p(z)=g\int_z^0\rho(z')\,dz'
=\boxed{\frac{\rho_0gH}{m+1}
\left(\frac{-z}{H}\right)^{m+1}}.
$$

This indeed has $p\propto\rho^{1+1/m}$ and $p(0)=0$, as required for a [polytropic atmosphere](../../../../../../polytropic-atmosphere.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
