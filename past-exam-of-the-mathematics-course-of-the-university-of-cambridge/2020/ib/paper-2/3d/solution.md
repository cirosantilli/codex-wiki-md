<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

Because the constraint determines

$$
x=b^2-a^2y^2-z^2,
$$

the constrained function is

$$
\Phi(y,z)=yz(b^2-a^2y^2-z^2).
$$

Its [stationary points](../../../../../stationary-point.md) satisfy

$$
\frac{\partial\Phi}{\partial y}
=z(b^2-3a^2y^2-z^2)=0,
\qquad
\frac{\partial\Phi}{\partial z}
=y(b^2-a^2y^2-3z^2)=0.
$$

When $yz=0$, these equations give

$$
(x,y,z)=(b^2,0,0),\quad
(0,\pm b/a,0),\quad
(0,0,\pm b).
$$

When $yz\ne0$, subtracting the two bracketed equations gives $z^2=a^2y^2$, and substitution then gives

$$
x=\frac{b^2}{2},
\qquad
y=\pm\frac b{2a},
\qquad
z=\pm\frac b2,
$$

with the two signs chosen independently. These are exactly the constrained stationary points; equivalently they follow from the [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations.

Under the additional restriction $x\ge0$, the constraint gives the compact elliptical disc $a^2y^2+z^2\le b^2$. On its boundary $x=0$, the objective is zero. At the four nonzero interior stationary points,

$$
\phi=xyz=\pm\frac{b^4}{8a},
$$

with the sign determined by $yz$. Therefore

$$
\boxed{\max\phi=\frac{b^4}{8a},
\qquad
\min\phi=-\frac{b^4}{8a}}.
$$

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
