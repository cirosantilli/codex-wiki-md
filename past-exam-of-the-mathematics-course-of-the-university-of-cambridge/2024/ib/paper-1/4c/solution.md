<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

At a regular constrained extremum of $f$ on $g=0$, the tangent [derivatives](../../../../../derivative.md) of $f$ vanish. Since $\nabla g$ is normal to the constraint surface, the [Lagrange multiplier](../../../../../lagrange-multiplier.md) condition is

$$
\nabla f=\lambda\nabla g,
\qquad g=0.
$$

One solves these equations and then compares the resulting candidates, including any boundary or singular cases.

Let the base have dimensions $x$ and $y$, and let the height be $z$. Measure cardboard relative to the thickness of the front and back. The weighted amount used is

$$
A=3xy+2xz+4yz,
$$

because the bottom has triple thickness, the two front and back faces have ordinary thickness, and the two side faces have double thickness. The constraint is $xyz=3$.

The multiplier equations are

$$
3y+2z=\lambda yz,
\qquad
3x+4z=\lambda xz,
\qquad
2x+4y=\lambda xy.
$$

They imply

$$
3xy=2xz=4yz.
$$

Thus $x=2y$ and $z=3y/2$; imposing $xyz=3$ gives $y=1$. Therefore

$$
\boxed{x=2,\qquad y=1,\qquad z=\frac32}.
$$

This is the global minimum: by the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md),

$$
A\geq3\sqrt[3]{(3xy)(2xz)(4yz)}
=3\sqrt[3]{24(xyz)^2}=18,
$$

and equality holds at these dimensions. This is an instance of [weighted open-box minimization](../../../../../weighted-open-box-minimization.md).

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
