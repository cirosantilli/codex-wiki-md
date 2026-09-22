<h1 id="23i/solution">Solution</h1>

↑ **Parent:** [23I](../23i.md)

For a regular parameter $t$, the [curvature](../../../../../curvature.md) and [torsion of a space curve](../../../../../torsion-of-a-curve.md) are

$$
\kappa=\frac{|\alpha'\times\alpha''|}{|\alpha'|^3},\qquad
\tau=\frac{\det(\alpha',\alpha'',\alpha''')}{|\alpha'\times\alpha''|^2}.
$$

The [torsion of a space curve](../../../../../torsion-of-a-curve.md) requires $\kappa\ne0$. Reparameterize by [arc length](../../../../../arc-length.md) $s$ and set $T=\alpha_s$, $N=T_s/\kappa$, $B=T\times N$. Differentiating the pairwise inner products of this orthonormal [Frenet frame](../../../../../frenet-frame.md) shows that its [derivative](../../../../../derivative.md) [matrix](../../../../../matrix.md) is skew symmetric. Since $T_s=\kappa N$, defining $\tau=N_s\cdot B$ gives the [Frenet-Serret formulas](../../../../../frenet-serret-formulas.md)

$$
\boxed{T_s=\kappa N,\quad N_s=-\kappa T+\tau B,\quad B_s=-\tau N.}
$$

The [fundamental theorem of regular space curves](../../../../../fundamental-theorem-of-regular-space-curves.md) says that prescribed smooth $\kappa>0$ and smooth $\tau$ on an interval determine a unit-speed curve uniquely up to an orientation-preserving Euclidean rigid motion. Solve this frame's [linear differential equation](../../../../../linear-differential-equation.md) with an initial oriented orthonormal frame, then integrate $\alpha_s=T$; uniqueness proves the assertion.

Under the intended convention that the shared parameter $s$ is [arc length](../../../../../arc-length.md), equality on an open interval gives equal position and equal [Frenet frames](../../../../../frenet-frame.md) at one point. Equal $\kappa,\tau$ give identical differential equations, so uniqueness gives $\boxed{\widetilde\alpha=\alpha\text{ on }I}$. The printed “regular smooth” hypothesis alone does not establish this convention. Without common [arc length](../../../../../arc-length.md), an orientation-preserving smooth change of speed that is the identity on $J$ but not elsewhere reparameterizes a [circle](../../../../../circle.md) into a counterexample: both curves have $\kappa=1$, $\tau=0$ and agree on $J$, but differ elsewhere as parameterized curves.

For an oriented surface with [unit normal](../../../../../unit-normal.md) $n$, define [normal curvature](../../../../../normal-curvature.md) $\kappa_n=T_s\cdot n$ and [geodesic curvature](../../../../../geodesic-curvature.md) $\kappa_g=T_s\cdot(n\times T)$. Thus

$$
T_s=\kappa_g(n\times T)+\kappa_n n.
$$

A unit-speed curve is a [geodesic](../../../../../geodesic.md) exactly when $\kappa_g=0$. If also $\kappa_n\equiv0$, then $T_s=0$, so it is a straight line. A vertical ruling of a circular cylinder is such a [geodesic](../../../../../geodesic.md), although the cylinder contains no open piece of a plane. A nonconstant regular straight line cannot be a simple closed curve. Hence **no planar patch is required, and such a [geodesic](../../../../../geodesic.md) cannot be simple and closed**.

Finally let the [principal curvatures](../../../../../principal-curvature.md) be $\kappa_1,\kappa_2$. If the [Gaussian curvature](../../../../../gaussian-curvature.md) $K=\kappa_1\kappa_2\geq0$, they have the same sign or one vanishes. [Euler formula for normal curvature](../../../../../euler-formula-for-normal-curvature.md) makes $\kappa_n$ a weighted average of them. For a [geodesic](../../../../../geodesic.md), $\kappa=|\kappa_n|$, so

$$
\boxed{\kappa\leq\max(|\kappa_1|,|\kappa_2|)\leq|\kappa_1+\kappa_2|=2|H|.}
$$

A horizontal [circle](../../../../../circle.md) on a cylinder of radius $R$ is a [geodesic](../../../../../geodesic.md) with $\kappa=1/R$, $K=0$, $|H|=1/(2R)$, attaining equality.

## ↑ Ancestors (10)

1. [23I](../23i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
