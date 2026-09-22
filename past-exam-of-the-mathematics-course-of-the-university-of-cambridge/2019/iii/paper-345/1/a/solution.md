<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $D=\partial_t+U\partial_x$, write $p$ for perturbation pressure divided by $\rho_0$, and set $b=-g\rho'/\rho_0$. The linearized [Boussinesq approximation](../../../../../../boussinesq-approximation.md), [incompressibility](../../../../../../incompressible-flow.md) and [material derivative](../../../../../../material-derivative.md) give

$$
Du+U'w=-p_x,\qquad Dw=-p_z+b,\qquad Db+N^2w=0,\qquad u_x+w_z=0.
$$

Taking the curl eliminates [pressure](../../../../../../pressure.md); differentiating the resulting [vorticity](../../../../../../vorticity.md) equation in $x$ and using [incompressibility](../../../../../../incompressible-flow.md) gives $D\nabla^2w-U''w_x=b_{xx}$. A further application of $D$ therefore yields

$$
\boxed{D^2\nabla^2w-U''D\partial_xw+N^2\partial_x^2w=0.}
$$

For a stationary nonzero horizontal [Fourier mode](../../../../../../fourier-mode.md), $D=U\partial_x$, so cancellation of $\partial_x^2$ gives the stationary [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md)

$$
\boxed{\left(\nabla^2+\frac{N^2}{U^2}-\frac{U''}{U}\right)w=0.}
$$

This division requires $U\ne0$ on the interval considered: a zero of $U$ is a [critical level of an internal gravity wave](../../../../../../critical-level-of-an-internal-gravity-wave.md). The mean profiles must be sufficiently smooth for the displayed derivatives, with background [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) and stable [density stratification](../../../../../../density-stratification.md), $N^2>0$, for propagating [internal gravity waves](../../../../../../internal-wave.md). The horizontally uniform component is excluded from the cancellation. For a horizontal [wavenumber](../../../../../../wavenumber.md) $k$, local vertical propagation additionally requires $N^2/U^2-U''/U>k^2$; this is distinct from the smoothness restrictions. If stability of the background against other disturbances is needed, the [Miles–Howard theorem](../../../../../../miles-howard-theorem.md) supplies the sufficient condition $N^2\geq(U')^2/4$, rather than a necessary condition for deriving the equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
