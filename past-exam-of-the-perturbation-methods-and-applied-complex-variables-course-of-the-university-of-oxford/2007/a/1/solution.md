<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Away from the boundary, [derivatives](../../../../derivative.md) of a smoothly varying solution are much smaller than $k^2f$ unless the [outer solution](../../../../outer-expansion.md) vanishes. Nonzero boundary data therefore require a rapidly varying layer. If its thickness is $\delta$, the radial second [derivative](../../../../derivative.md) is of order $f/\delta^2$; balancing it with $k^2f$ gives $\delta=k^{-1}$.

Put $R=k(1-r)$ and write $f(r,\theta)=F(R,\theta)$. The equation becomes

$$
F_{RR}-\frac1{kr}F_R+\frac1{k^2r^2}F_{\theta\theta}=F.
$$

For fixed $R$ and boundary data with angular variation independent of $k$, the leading equation is $F_{RR}=F$. Matching to the zero [outer solution](../../../../outer-expansion.md) removes the growing exponential, and the [boundary value](../../../../boundary-value.md) at $R=0$ fixes its coefficient:

$$
\boxed{F_0(R,\theta)=g(\theta)e^{-R}.}
$$

This approximation describes the layer; it is not a uniform expansion in polar coordinates at the origin.

[Laplace's method](../../../../laplace-s-method.md) localizes an exponential [integral](../../../../integral-split.md) near maxima of its real phase. At an isolated smooth interior [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) $t_0$ with $G''(t_0)<0$ and $F(t_0)\neq0$, [Taylor expansion](../../../../taylor-expansion.md) and [Gaussian integral](../../../../gaussian-integral.md) give

$$
\int F(t)e^{kG(t)}dt\sim F(t_0)e^{kG(t_0)}
\sqrt{\frac{2\pi}{k|G''(t_0)|}}.
$$

An endpoint [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) with nonzero inward phase slope instead gives an inverse-$k$ factor. Degenerate maxima require their first nonzero local phase term; continuous differentiability alone does not guarantee the quadratic formula.

Here $\cos(ix\sin\phi)=\cosh(x\sin\phi)$. In its two exponentials, the positive exponential dominates at the interior [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) $\phi=\pi/2$ of $\sin\phi$. Since $\sin(\pi/2+s)=1-s^2/2+O(s^4)$,

$$
I_0(x)\sim\frac1{2\pi}e^x\int_{-\infty}^{\infty}e^{-xs^2/2}ds
=\frac{e^x}{\sqrt{2\pi x}}.
$$

The negative exponential has no comparable positive [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) and is negligible. Consequently, where $kr\to\infty$,

$$
\frac{I_0(kr)}{I_0(k)}\sim r^{-1/2}e^{-k(1-r)}.
$$

In the [boundary layer](../../../../boundary-layer.md) $r=1-R/k$, $r^{-1/2}=1+O(k^{-1})$, so this reduces to **$e^{-R}$**, agreeing with the formal result when $g=1$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
