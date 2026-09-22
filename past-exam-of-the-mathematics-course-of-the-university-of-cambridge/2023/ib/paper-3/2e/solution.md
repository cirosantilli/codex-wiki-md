<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

In the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md), the [Riemannian metric](../../../../../riemannian-metric.md)

$$
ds^2=\frac{dx^2+dy^2}{y^2}
$$

assigns to a [smooth curve](../../../../../smooth-curve.md) $\gamma(t)=(x(t),y(t))$ the length

$$
L(\gamma)=\int
\frac{\sqrt{\dot x(t)^2+\dot y(t)^2}}{y(t)}\,dt.
$$

The metric is conformal to the Euclidean metric, so hyperbolic and Euclidean angles agree. Its area element is

$$
dA=\frac{dx\,dy}{y^2}.
$$

The two geodesics from $e^{i\alpha}$ and $e^{i\beta}$ to infinity are the vertical lines $x=\cos\alpha$ and $x=\cos\beta$, while the third side is the unit semicircle. The triangle lies above that semicircle, so its area is

$$
\begin{aligned}
\operatorname{Area}
&=\int_{\cos\beta}^{\cos\alpha}
\int_{\sqrt{1-x^2}}^\infty\frac{dy\,dx}{y^2}\\
&=\int_{\cos\beta}^{\cos\alpha}
\frac{dx}{\sqrt{1-x^2}}
=\beta-\alpha.
\end{aligned}
$$

Its interior angles are $\alpha$, $\pi-\beta$, and zero at the [ideal](../../../../../ideal.md) vertex, and hence

$$
\operatorname{Area}
=\pi-\bigl(\alpha+(\pi-\beta)+0).
$$

Triangulating a geodesic polygon with $n$ sides into $n-2$ triangles gives

$$
\boxed{
\operatorname{Area}
=(n-2)\pi-\sum_{j=1}^n\theta_j
},
$$

the [area of a hyperbolic geodesic polygon](../../../../../area-of-a-hyperbolic-geodesic-polygon.md) and the polygonal [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md).

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
