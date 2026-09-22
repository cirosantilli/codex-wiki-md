<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fermat principle](../../../../../fermat-principle.md) makes the [optical path length](../../../../../optical-path-length.md) stationary. For a graph $y=\xi(x)$ the variational integrand is

$$
\mathcal L(x,\xi,\xi')=n(x,\xi)\sqrt{1+\xi'^2}.
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\frac d{dx}\left[\frac{n(x,\xi)\xi'}{\sqrt{1+\xi'^2}}\right]-n_y(x,\xi)\sqrt{1+\xi'^2}=0.
$$

Use the [chain rule](../../../../../chain-rule.md) $d n(x,\xi(x))/dx=n_x+n_y\xi'$ and differentiate $\xi'/\sqrt{1+\xi'^2}$ to obtain

$$
\frac{(n_x+n_y\xi')\xi'}{\sqrt{1+\xi'^2}}+\frac{n\xi''}{(1+\xi'^2)^{3/2}}-n_y\sqrt{1+\xi'^2}=0.
$$

Multiplying through and combining the $n_y$ terms gives the required second-order [ordinary differential equation](../../../../../ordinary-differential-equation.md) with no derivatives in denominators:

$$
\boxed{n(x,\xi)\xi''=(1+\xi'^2)[n_y(x,\xi)-\xi'n_x(x,\xi)].}
$$

All partial [derivatives](../../../../../derivative.md) of the [refractive index](../../../../../refractive-index.md) are evaluated along the ray.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
