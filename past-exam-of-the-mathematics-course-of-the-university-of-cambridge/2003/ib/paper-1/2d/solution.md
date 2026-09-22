<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

For positive differentiable speed $c(y)$ and a smooth ray written as a graph $y(x)$, the [Fermat principle](../../../../../fermat-principle.md) minimizes travel time

$$
\mathcal T[y]=\int_{x_0}^{x_1}\frac{\sqrt{1+y'^2}}{c(y)}\,dx.
$$

A variation vanishing at the endpoints gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) for $F=\sqrt{1+y'^2}/c$. Its derivatives are $F_y=-c'\sqrt{1+y'^2}/c^2$ and $F_{y'}=y'/(c\sqrt{1+y'^2})$. Thus

$$
\frac d{dx}F_{y'}-F_y=\frac{y''}{c(1+y'^2)^{3/2}}+\frac{c'}{c^2\sqrt{1+y'^2}}=0,
$$

and multiplying by $c^2(1+y'^2)^{3/2}$ gives

$$
\boxed{c(y)y''+c'(y)(1+y'^2)=0.}
$$

The displayed differential equation requires differentiability, beyond mere continuity of $c$. For constant positive speed it reduces to $y''=0$, so rays are straight lines; a straight segment minimizes travel time because it has the shortest Euclidean length.

For $c(y)=y$ in the positive-height region, the [Beltrami identity](../../../../../beltrami-identity.md) gives $F-y'F_{y'}=1/[y\sqrt{1+y'^2}]=1/R$. Hence $y^2(1+y'^2)=R^2$, whose nonvertical solutions are $(x-h)^2+y^2=R^2$. Formally imposing the given boundary points fixes $h=1/2$, $R=1/2$, and gives the [ray in a linear-speed medium](../../../../../ray-in-a-linear-speed-medium.md)

$$
\boxed{y(x)=\sqrt{x(1-x)},\qquad 0<x<1.}
$$

It is the upper semicircle of diameter one, with vertical limiting tangents at its endpoints.

<a id="2d/image-formal-semicircular-ray-with-zero-speed-ideal-endpoints-in-the-linear-speed-medium"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1-optical-ray.png)

**[Figure 1](#2d/image-formal-semicircular-ray-with-zero-speed-ideal-endpoints-in-the-linear-speed-medium). Formal semicircular ray with zero-speed ideal endpoints in the linear-speed medium**.

There is a necessary endpoint qualification. The speed is zero at the two stated endpoints. For any rectifiable path entering positive height, $ds/y\geq |dy|/y$, and its travel time diverges logarithmically on leaving or approaching height zero. Thus **the semicircle is the formal interior ray, but there is no finite-time minimizer between the zero-speed endpoints**. For endpoints at height $\epsilon>0$ the circular ray has radius $\sqrt{1/4+\epsilon^2}$ and finite travel time $2\operatorname{arsinh}(1/(2\epsilon))$, which tends to infinity as $\epsilon\downarrow0$. This explains the intended semicircle as a limiting [hyperbolic geodesic](../../../../../geodesic-in-the-poincare-half-plane-model.md), without asserting finite travel time where $c=0$.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
