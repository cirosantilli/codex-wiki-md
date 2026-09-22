<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

In polar coordinates the metric is

$$
ds^2=\frac{4(dr^2+r^2d\theta^2)}{(1-r^2)^2}.
$$

Along a radius, the hyperbolic distance from the origin to Euclidean radius $r$ is therefore

$$
R=\int_0^r\frac{2\,dt}{1-t^2}
=\log\frac{1+r}{1-r},
$$

so $r=\tanh(R/2)$. The Riemannian area element is

$$
dA=\frac{4r}{(1-r^2)^2}\,dr\,d\theta.
$$

Consequently a hyperbolic disc of radius $R$ has area

$$
\begin{aligned}
A(R)
&=\int_0^{2\pi}\int_0^{\tanh(R/2)}
\frac{4r}{(1-r^2)^2}\,dr\,d\theta\\
&=4\pi\sinh^2(R/2)
=2\pi(\cosh R-1).
\end{aligned}
$$

This proves the [area of a hyperbolic disc](../../../../../area-of-a-hyperbolic-disc.md) formula from the metric.

For area $\pi/2$ we get $\cosh R=5/4$. Hence $\sinh R=3/4$ and $e^R=2$, so $R=\log2$. Tangent equal discs have centers at distance $2R$. Since the centers lie successively on the same radial geodesic,

$$
d(O,c_n)=2nR=n\log4.
$$

If $r_n$ is the Euclidean coordinate of $c_n$, the radial distance formula gives

$$
\frac{1+r_n}{1-r_n}=4^n.
$$

Therefore the [radial chain of equal hyperbolic discs](../../../../../radial-chain-of-equal-hyperbolic-discs.md) has

$$
\boxed{r_n=\frac{4^n-1}{4^n+1}}.
$$

**No such isometry to the stated upper-half-plane configuration exists for $n\geq3$.** The centers $c_0,\ldots,c_n$ lie on one hyperbolic geodesic, so their images under an isometry would also lie on one geodesic. In the upper-half-plane model, geodesics are vertical lines or semicircles orthogonal to the real axis. Neither type can contain three distinct points of the horizontal line $y=1$, while the centers of the distinct discs $D'_0,\ldots,D'_n$ all lie on that line. This is the [geodesic obstruction for a horizontal chain of hyperbolic discs](../../../../../geodesic-obstruction-for-a-horizontal-chain-of-hyperbolic-discs.md).

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
