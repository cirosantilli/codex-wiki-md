<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

In the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md), $\mathbb H=\{x+iy:y>0\}$ has [Riemannian metric](../../../../../riemannian-metric.md)

$$
\boxed{ds^2=\frac{dx^2+dy^2}{y^2}.}
$$

Its orientation-preserving [isometries](../../../../../isometry.md) are the [Möbius transformations](../../../../../mobius-transformation.md) $z\mapsto(az+b)/(cz+d)$ with real coefficients and $ad-bc=1$, with a simultaneous sign change representing the same map. The full [isometry group](../../../../../isometry-group.md) also contains their compositions with $z\mapsto-\overline z$, which reverse [orientation](../../../../../orientation-of-a-simplex.md). The [hyperbolic lines](../../../../../hyperbolic-line.md) are vertical Euclidean lines and upper semicircles centred on the real axis; each meets the boundary orthogonally.

A [hyperbolic line](../../../../../hyperbolic-line.md) with finite endpoints $p<q$ is mapped to the [imaginary axis](../../../../../imaginary-axis.md) by

$$
T(z)=\frac{z-p}{q-z}.
$$

Its coefficient [determinant](../../../../../determinant.md) is $q-p>0$, so rescaling the coefficients makes this an orientation-preserving [isometry](../../../../../isometry.md). The endpoints map to $0$ and $\infty$, which characterize the imaginary-axis [hyperbolic line](../../../../../hyperbolic-line.md). For a vertical line with endpoints $p,\infty$, use $T(z)=z-p$. If $T_1,T_2$ send the two prescribed lines to the [imaginary axis](../../../../../imaginary-axis.md), $T_2^{-1}T_1$ sends the first to the second. This proves [transitivity](../../../../../transitive-relation.md) on [hyperbolic lines](../../../../../hyperbolic-line.md).

For two [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md), choose their common perpendicular and map it to the [imaginary axis](../../../../../imaginary-axis.md). A [hyperbolic line](../../../../../hyperbolic-line.md) perpendicular to that axis is a semicircle centred at zero: [orthogonality](../../../../../orthogonal-vectors.md) at $iy$ forces the [circle](../../../../../circle.md) centre to have real coordinate zero. Thus the reflecting lines become semicircles of distinct radii $r_1,r_2>0$. The [hyperbolic reflection](../../../../../hyperbolic-reflection.md) in the radius-$r$ semicircle is $S_r(z)=r^2/\overline z$; it fixes that semicircle pointwise and reverses [orientation](../../../../../orientation-of-a-simplex.md). Their composition is

$$
S_{r_2}S_{r_1}(z)=\lambda z,\qquad\lambda=(r_2/r_1)^2\ne1.
$$

Its $k$th power is $z\mapsto\lambda^kz$, and no positive power is the identity since $\lambda>0$ and $\lambda\ne1$. Conjugation by the chosen [isometry](../../../../../isometry.md) preserves [order of a group element](../../../../../order-of-a-group-element.md), so **the original composition has infinite order**. Reversing the order of the reflections replaces $\lambda$ by $\lambda^{-1}$ and gives the same conclusion.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
