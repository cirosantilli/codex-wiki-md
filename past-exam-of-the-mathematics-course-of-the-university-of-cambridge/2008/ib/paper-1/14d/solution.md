<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

For variations $y+\epsilon\eta$ with $\eta(x_1)=\eta(x_2)=0$, [integration by parts](../../../../../integration-by-parts.md) gives $\delta I=\int_{x_1}^{x_2}[f_y-(d/dx)f_{y'}]\eta\,dx$. Since this vanishes for every such variation, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{\frac{\partial f}{\partial y}-\frac{d}{dx}\frac{\partial f}{\partial y'}=0.}
$$

When $f$ is independent of $y$, it has the [first integral](../../../../../first-integral.md) $\boxed{\partial f/\partial y'=C}$.

For a ray represented as a graph traversed with increasing $x$, the travel time is $T=\int_{x_1}^{x_2}\sqrt{1+y'^2}/c(x)\,dx$, with $c(x)>0$. By [Fermat principle](../../../../../fermat-principle.md), use $f=\sqrt{1+y'^2}/c(x)$. The [first integral](../../../../../first-integral.md) becomes

$$
\frac{y'}{c(x)\sqrt{1+y'^2}}=C.
$$

The sign of $y'$ is constant, and $y_2>y_1$ makes it positive. Write $C=1/k$ with $k>0$ and solve to obtain

$$
\boxed{y'=\frac{c(x)}{\sqrt{k^2-c(x)^2}},\qquad y_2-y_1=\int_{x_1}^{x_2}\frac{c(x)}{\sqrt{k^2-c(x)^2}}\,dx.}
$$

A finite slope requires $k>c(x)$ in the interior; a limiting vertical tangent is possible at an endpoint.

For $c(x)=ax$ and $k=ax_2$, positive speed on the whole interval and $k\geq c(x)$ select $a>0$ and $0<x_1<x_2$. The slope is $x/\sqrt{x_2^2-x^2}$. Integrating backwards from $(x_2,y_2)$ gives

$$
y_2-y=\int_x^{x_2}\frac{u}{\sqrt{x_2^2-u^2}}\,du=\sqrt{x_2^2-x^2},
$$

so $\boxed{(y_2-y)^2=x_2^2-x^2}$, with the branch $y\leq y_2$. The endpoint integral is finite despite the vertical tangent. The specified value $k=ax_2$ fits the first endpoint precisely when $y_2-y_1=\sqrt{x_2^2-x_1^2}$; for other endpoint data the preceding integral determines a different $k$.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
