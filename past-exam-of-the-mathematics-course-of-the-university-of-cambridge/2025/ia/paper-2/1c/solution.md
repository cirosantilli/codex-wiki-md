<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

The critical-point equations are $2xy=0$ and $x^2+y^2=1$, so the points are $(\pm1,0)$ and $(0,\pm1)$. The Hessian is

$$
\begin{pmatrix}2y&2x\\2x&2y\end{pmatrix}.
$$

Thus $(0,1)$ is a strict minimum, $(0,-1)$ a strict maximum, and $(\pm1,0)$ are saddles. The local contour patterns are respectively ellipses, inverted ellipses, and crossing hyperbolas.

The [gradient flow](../../../../../gradient-flow.md) has $\dot x=-2xy$ and $\dot y=1-x^2-y^2$. Hence

$$
2xy\frac{dy}{dx}-y^2=x^2-1.
$$

Putting $u=y^2$ gives $xu'-u=x^2-1$. Multiplication by the [integrating factor](../../../../../integrating-factor.md) $1/x$ yields

$$
\left(\frac ux\right)'=1-\frac1{x^2},
$$

and therefore the general trajectory is

$$
\boxed{y^2=x^2+1+cx.}
$$

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
