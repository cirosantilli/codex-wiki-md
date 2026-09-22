<h1 id="31e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The off-axis equilibria exist for $|a|\leq1$ and coalesce with an axial equilibrium at each endpoint. Thus the stationary bifurcations occur at

$$
\boxed{\ a=\pm1.\ }
$$

For the positive bifurcation, $a_0=y_0=1$. Put

$$
Y=y-1,
\qquad \mu=a-1,
$$

so that

$$
\dot x=2x(Y-\mu),
\qquad
\dot Y=-x^2-2Y-Y^2,
\qquad
\dot\mu=0.
$$

Write the extended [center manifold](../../../../../../center-manifold.md) as $Y=h(x,\mu)$. Its invariance equation is

$$
2x(h-\mu)h_x=-x^2-2h-h^2.
$$

Under the scaling $\mu=O(x^2)$, comparison of the terms of order $x^2$ gives

$$
\boxed{\ Y=h(x,\mu)=-\frac{x^2}{2}+O(x^4).\ }
$$

Substitution into the $x$ equation gives

$$
\boxed{\ \dot x=-2\mu x-x^3+O(x^5).\ }
$$

With the reversed parameter $\nu=-2\mu=2(1-a)$, this is the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) normal form $\dot x=\nu x-x^3$. Therefore the positive stationary bifurcation is a **supercritical pitchfork in the parameter $\nu=2(1-a)$**, or equivalently the stable daughter equilibria exist on the $a<1$ side.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
