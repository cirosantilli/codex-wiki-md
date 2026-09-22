<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For increments $h=x-x_s$ and $k=y-y_s$, the second-order multivariable [Taylor expansion](../../../../taylor-expansion.md) is

$$
z=z_s+(z_x)_s h+(z_y)_s k+\frac12\left[(z_{xx})_s h^2+2(z_{xy})_s hk+(z_{yy})_s k^2\right]+o(h^2+k^2).
$$

At a [stationary point](../../../../stationary-point.md) $(x_s,0)$, $\sin x_s=-2x_s\cos x_s$ and $z_s=\cos x_s e^{-x_s^2}$. Direct differentiation gives

$$
(z_{xx})_s=-(4x_s^2+3)z_s,\qquad(z_{xy})_s=0,\qquad(z_{yy})_s=-2z_s.
$$

Thus, since this particular [function](../../../../function-split.md) is analytic, the expansion can be written

$$
\boxed{z(x,y)=z_s\left[1-\frac{4x_s^2+3}{2}(x-x_s)^2-y^2\right]+O\!\left(((x-x_s)^2+y^2)^{3/2}\right)}.
$$

There are no linear terms because the [gradient](../../../../gradient.md) vanishes, and no mixed quadratic term because the mixed [derivative](../../../../derivative.md) vanishes on the axis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
