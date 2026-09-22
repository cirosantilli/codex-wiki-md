<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

Vary $g$ to $g+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$. The [first variation](../../../../../first-variation.md) of the functional is

$$
\delta\mathcal E=\int_a^b(f_g\eta+f_{g'}\eta')\,dr
=\int_a^b\left(f_g-\frac d{dr}f_{g'}\right)\eta\,dr.
$$

The endpoint term vanishes. Since every smooth test variation is allowed, stationarity gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\frac d{dr}\frac{\partial f}{\partial g'}-\frac{\partial f}{\partial g}=0.}
$$

The constant prefactor in the specified energy does not affect its stationary equation. Its integrand gives $f_{\phi'}=r^2\phi'$ and $f_\phi=r^2\phi/\lambda^2$, so

$$
(r^2\phi')'-\frac{r^2}{\lambda^2}\phi=0,
\qquad
\boxed{\frac1r(r\phi)''-\frac1{\lambda^2}\phi=0.}
$$

Take $\lambda>0$ as a screening length; for a nonzero real parameter of either sign its absolute value gives the same equation. Setting $u=r\phi$ yields $u''-u/\lambda^2=0$, hence

$$
\boxed{\phi(r)=\frac{Ae^{r/\lambda}+Be^{-r/\lambda}}r.}
$$

For $0<R_1<R_2$ and the prescribed endpoint values, the convenient hyperbolic form is

$$
\boxed{\phi(r)=\phi_1\frac{R_1}{r}
\frac{\sinh[(R_2-r)/\lambda]}{\sinh[(R_2-R_1)/\lambda]}.}
$$

It directly satisfies both endpoint values. The energy is a positive quadratic functional, so this stationary solution is its unique minimizer for fixed endpoints: any zero-endpoint variation adds a positive quadratic energy, with the cross term zero by the equation.

In two dimensions, cylindrical area measure replaces the radial factor $r^2$ by $r$. Up to an irrelevant common normalization, the corresponding energy and its [modified Helmholtz equation](../../../../../modified-helmholtz-equation.md) are

$$
\mathcal E_2[\phi]=2\pi\int_{R_1}^{R_2}\left[\frac12\phi'^2+\frac{\phi^2}{2\lambda^2}\right]r\,dr,
\qquad
\boxed{\frac1r(r\phi')'-\frac1{\lambda^2}\phi=0.}
$$

Thus the two-dimensional radial equation is $\phi''+r^{-1}\phi'-\lambda^{-2}\phi=0$, rather than the three-dimensional equation with coefficient $2/r$ on the first [derivative](../../../../../derivative.md).

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
