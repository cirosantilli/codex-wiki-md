<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The join has matching positions and first [derivatives](../../../../../derivative.md):

$$
F(1)=E(0)=(0,0),\qquad
F'(t)=(4-4t,2-4t),\qquad E'(t)=(4t,-2+4t),
$$



$$
\boxed{F'(1)=E'(0)=(0,-2)\ne(0,0).}
$$

Because both pieces have unit parameter intervals, these are also the one-sided [derivatives](../../../../../derivative.md) of $S$ at $u=1$. Thus $S$ has first-order [parametric continuity](../../../../../parametric-continuity.md), and hence first-order [geometric continuity](../../../../../geometric-continuity.md), with no corner or cusp. Its nonzero tangent [vector](../../../../../vector.md) points vertically downward.

The second [derivatives](../../../../../derivative.md) do not agree:

$$
F''(1)=(-4,-4),\qquad E''(0)=(4,4).
$$

So this is $C^1$ but not $C^2$ [parametric continuity](../../../../../parametric-continuity.md). The signed planar [curvature](../../../../../curvature.md) $\kappa=(x'y''-y'x'')/(x'^2+y'^2)^{3/2}$ has one-sided values

$$
\kappa_F(1)=\frac{-8}{8}=-1,\qquad
\kappa_E(0)=\frac{8}{8}=1.
$$

The unsigned [curvatures](../../../../../curvature.md) agree, but the bending switches sides; there is no second-order [geometric continuity](../../../../../geometric-continuity.md) through a regular orientation-preserving reparametrization. The join is a reversal of bending with a curvature jump, rather than a smooth zero-curvature inflection.

For the “gradient” compute $dy/dx=y'/x'$ away from the join:

$$
\frac{F_y'(t)}{F_x'(t)}=\frac{2-4t}{4-4t}\longrightarrow-\infty\quad(t\to1^-),\qquad
\frac{E_y'(t)}{E_x'(t)}=\frac{-2+4t}{4t}\longrightarrow-\infty\quad(t\to0^+).
$$

Hence

$$
\boxed{\text{no finite }dy/dx\text{ at the join; the tangent line is }x=0.}
$$

The zero horizontal [derivative](../../../../../derivative.md) is not a stationary [point](../../../../../point-geometry.md) of the [parametric curve](../../../../../parametric-curve.md), since its vertical [derivative](../../../../../derivative.md) is $-2$. It means that the locally regular [curve](../../../../../curve.md) has a vertical [tangent line](../../../../../tangent-line.md) and cannot have a finite graph [derivative](../../../../../derivative.md) as $y(x)$ there.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
