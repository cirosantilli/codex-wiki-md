<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Differentiate the position vector with respect to each of the [spherical polar coordinates](../../../../../spherical-coordinate-system.md). The derivatives are

$$
\begin{aligned}
\partial_r\mathbf x&=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta),\\
\partial_\theta\mathbf x&=r(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\\
\partial_\phi\mathbf x&=r\sin\theta(-\sin\phi,\cos\phi,0).
\end{aligned}
$$

Their lengths give the [scale factors of orthogonal coordinates](../../../../../scale-factors-of-orthogonal-coordinates.md):

$$
\boxed{h_r=1,\qquad h_\theta=r,\qquad h_\phi=r\sin\theta.}
$$

Dividing the derivatives by these lengths yields

$$
\begin{aligned}
\mathbf e_r&=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta),\\
\mathbf e_\theta&=(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\\
\mathbf e_\phi&=(-\sin\phi,\cos\phi,0).
\end{aligned}
$$

Each has unit length. For example, $\mathbf e_r\cdot\mathbf e_\theta=\sin\theta\cos\theta(\cos^2\phi+\sin^2\phi)-\cos\theta\sin\theta=0$; the other two [dot products](../../../../../dot-product.md) vanish because their first two terms cancel. Thus these are mutually [orthogonal vectors](../../../../../orthogonal-vectors.md), and the total differential has the required form. The coordinates degenerate at $r=0$ and on the polar axis, but this does not affect an area integral.

On the [parametrized surface](../../../../../parametrized-surface.md) $\theta=\alpha$, use $r,\phi$ as parameters. The [surface integral](../../../../../surface-integral.md) area element is

$$
dS=|\partial_r\mathbf x\times\partial_\phi\mathbf x|\,dr\,d\phi=r\sin\alpha\,dr\,d\phi.
$$

For $0\leq\alpha\leq\pi$, its lateral area, with no closing disk, is therefore

$$
\boxed{A=\int_0^{2\pi}\!\int_0^R r\sin\alpha\,dr\,d\phi=\pi R^2\sin\alpha.}
$$

At $\alpha=0,\pi$ the surface collapses to a line and its area is zero.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
