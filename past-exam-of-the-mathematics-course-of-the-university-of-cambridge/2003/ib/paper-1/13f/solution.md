<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

The [Poincaré half-plane model](../../../../../poincare-half-plane-model.md) has [Riemannian metric](../../../../../riemannian-metric.md) $ds^2=(dx^2+dy^2)/y^2=|dz|^2/(\operatorname{Im}z)^2$. Every [Möbius transformation](../../../../../mobius-transformation.md) preserving this half-plane can be represented as $f(z)=(Az+B)/(Cz+D)$ with real coefficients and $\Delta=AD-BC>0$. Direct calculation gives

$$
f'(z)=\frac{\Delta}{(Cz+D)^2},\qquad\operatorname{Im}f(z)=\frac{\Delta\operatorname{Im}z}{|Cz+D|^2}.
$$

Therefore $|df|/\operatorname{Im}f=|dz|/\operatorname{Im}z$, proving it is an [isometry](../../../../../isometry.md).

The imaginary axis is a [hyperbolic geodesic](../../../../../geodesic-in-the-poincare-half-plane-model.md). Its distance from $ib$ to $ic$ is $|\int_b^cdy/y|=|\log(c/b)|$. This is also the minimum over all paths, since path length is at least $|\int dy/y|$. The two vertical points at distance $r$ from $ib$ are $ibe^{-r}$ and $ibe^r$. Reflection in the imaginary axis preserves the [hyperbolic circle](../../../../../hyperbolic-circle.md) and its centre. Since it is assumed to be a Euclidean circle, its Euclidean centre lies on that axis and its two vertical intersections determine the Euclidean centre and radius:

$$
\boxed{\text{Euclidean centre }ib\cosh r,\qquad\text{Euclidean radius }b\sinh r.}
$$

This proves the [hyperbolic circle in the upper half-plane](../../../../../hyperbolic-circle-in-the-upper-half-plane.md) formula for the specified centre.

For the horizontal-distance calculation, the geodesic joining $ib$ to $a+ib$ is the semicircle of centre $a/2$ and radius $R=\sqrt{b^2+a^2/4}$. Parameterize it as $z=a/2+Re^{i\theta}$. Its metric length is $|d\theta|/\sin\theta$. If the right endpoint angle is $\theta_0$, then $\sin\theta_0=b/R$, $\cos\theta_0=a/(2R)$, and the other endpoint angle is $\pi-\theta_0$. Hence

$$
d_H(ib,a+ib)=\int_{\theta_0}^{\pi-\theta_0}\frac{d\theta}{\sin\theta}=2\log\frac{R+a/2}{b}=2\operatorname{arsinh}\frac a{2b}.
$$

The [equality of horizontal hyperbolic and Euclidean distances](../../../../../equality-of-horizontal-hyperbolic-and-euclidean-distances.md) therefore requires

$$
\boxed{b=\frac{a}{2\sinh(a/2)}.}
$$

Let $t=a/2>0$. The derivative of $t/\sinh t$ has the sign of $\sinh t-t\cosh t$. This quantity vanishes at zero and has derivative $-t\sinh t<0$, so the height function is strictly decreasing. Its limits are one at $a\downarrow0$ and zero at $a\to\infty$. Continuity and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) prove that **each $0<b<1$ has exactly one positive matching separation $a$**.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
