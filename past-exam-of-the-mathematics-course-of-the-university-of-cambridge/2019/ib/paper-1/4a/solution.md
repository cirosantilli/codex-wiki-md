<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Introduce the orthogonal coordinates

$$
u=\frac{x-z}{\sqrt2},
\qquad
v=\frac{x+z}{\sqrt2}.
$$

Then the constraint and objective become

$$
u^2+v^2+2y^2=1,
\qquad
\phi=\sqrt2uy.
$$

The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations for a [stationary point](../../../../../stationary-point.md) are

$$
\sqrt2y=2\lambda u,
\qquad
\sqrt2u=4\lambda y,
\qquad
0=2\lambda v.
$$

If $\lambda=0$, then $u=y=0$ and $v=\pm1$, giving

$$
(x,y,z)=\left(\frac1{\sqrt2},0,\frac1{\sqrt2}\right),
\quad
\left(-\frac1{\sqrt2},0,-\frac1{\sqrt2}\right).
$$

If $\lambda\ne0$, then $v=0$. The first two equations and the constraint imply

$$
\lambda=\pm\frac12,
\qquad
u=\pm\frac1{\sqrt2},
\qquad
y=\sqrt2\lambda u.
$$

Converting back to $(x,y,z)$ gives the other four points. Therefore all stationary points are

$$
\boxed{\left(\pm\frac1{\sqrt2},0,\pm\frac1{\sqrt2}\right)}
$$

with matching signs, together with

$$
\boxed{\left(\frac12,\frac12,-\frac12\right),
\left(-\frac12,-\frac12,\frac12\right),
\left(\frac12,-\frac12,-\frac12\right),
\left(-\frac12,\frac12,\frac12\right)}.
$$

The middle pair has $\phi=1/2$, the last pair has $\phi=-1/2$, and the first pair has $\phi=0$.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
