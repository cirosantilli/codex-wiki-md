<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Set $r_H=2m$. Since $f'(r_H)=2\kappa$, the integrand defining the [tortoise coordinate](../../../../../../tortoise-coordinate.md) has a simple pole:

$$
r_* =\frac1{2\kappa}\log|r-r_H|+h(r),
$$

where $h$ is analytic near $r_H$. Define the [Kruskal–Szekeres coordinates](../../../../../../kruskal-szekeres-coordinates.md) in the right exterior by $U=-e^{-\kappa u}$ and $V=e^{\kappa v}$. Then

$$
-UV=e^{2\kappa r_*}=(r-r_H)e^{2\kappa h(r)}.
$$

The right-hand side has positive nonzero derivative at $r_H$. Continuing this relation analytically, rather than retaining an absolute value, makes $r$ an analytic function of $UV$ through both signs. The [Kruskal extension across a simple static horizon](../../../../../../kruskal-extension-across-a-simple-static-horizon.md) has metric

$$
ds^2=\frac{f(r)}{\kappa^2UV}\,dU\,dV+R(r)^2d\Omega^2.
$$

Its radial coefficient tends to $-2e^{-2\kappa h(r_H)}/\kappa$, finite and nonzero, while $R(r_H)^2=4m^2\cosh\alpha$. Therefore both null surfaces $U=0$ and $V=0$ are regular horizon branches, intersecting at a smooth two-sphere $U=V=0$.

The stationary [Killing vector field](../../../../../../killing-vector-field.md) becomes

$$
\boxed{K=\kappa\bigl(V\partial_V-U\partial_U\bigr).}
$$

It is null, tangent and normal on each horizon branch and vanishes on their intersection. This proves that $r=2m$ is a [bifurcate Killing horizon](../../../../../../bifurcate-killing-horizon.md), with [bifurcation surface](../../../../../../bifurcation-surface.md) of area $\boxed{A_H=16\pi m^2\cosh\alpha}$. The exponential definitions specify one exterior; allowing all signs of $U,V$ supplies the remaining quadrants of the extension.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
