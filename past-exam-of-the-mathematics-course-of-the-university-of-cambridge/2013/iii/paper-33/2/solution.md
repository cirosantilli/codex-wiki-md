<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [unit-width box kernel](../../../../../unit-width-box-kernel.md), the [convolution](../../../../../convolution.md) and [kernel density estimator](../../../../../kernel-density-estimation.md) are

$$
g_h(x)=(K_h*f)(x)=\int_{\mathbb R}K_h(x-y)f(y)\,dy=\frac1h\int_{x-h/2}^{x+h/2}f(y)\,dy,
$$

and

$$
\widehat f_{n,h}^K(x)=\frac1n\sum_{i=1}^nK_h(x-X_i)=\frac1{nh}\sum_{i=1}^n\mathbf1_{\{|x-X_i|\le h/2\}}.
$$

In particular $\mathbb E\widehat f_{n,h}^K=g_h$. The scaling gives $\|K_h\|_2^2=h^{-1}\|K\|_2^2=h^{-1}$. Even if $f$ is not square-integrable, [Young's convolution inequality](../../../../../young-s-convolution-inequality.md) gives $g_h\in L^2$ because $f\in L^1$ and $K_h\in L^2$.

Using independence to eliminate the cross terms in the centred estimator, and [Tonelli theorem](../../../../../tonelli-theorem.md) to integrate the nonnegative variance, gives the exact [integrated variance of a kernel density estimator](../../../../../integrated-variance-of-a-kernel-density-estimator.md):

$$
\mathbb E\|\widehat f_{n,h}^K-g_h\|_2^2=\frac1n\left(\int_{\mathbb R}\mathbb E K_h(x-X)^2\,dx-\|g_h\|_2^2\right)=\frac1n\left(\frac1h-\|g_h\|_2^2\right)\le\frac1{nh}.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) now yields

$$
\boxed{\mathbb E\|\widehat f_{n,h}^K-K_h*f\|_2\le\frac1{\sqrt{nh}},\qquad\kappa=1.}
$$

This constant comes from the unit $L^2$ norm of the unscaled [unit-width box kernel](../../../../../unit-width-box-kernel.md).

For the piecewise constant [probability density function](../../../../../probability-density-function.md), integrability forces the constants on both unbounded outer intervals to be zero. Thus $f$ is bounded, has compact support, and has finitely many jumps. Let $\Delta_r=f(x_r+)-f(x_r-)$ denote the jump at $x_r$. For $h$ smaller than the least gap between consecutive breakpoints, the smoothing regions $[x_r-h/2,x_r+h/2]$ do not overlap. Outside these regions the [convolution](../../../../../convolution.md) equals $f$.

Within a region, put $v=x-x_r$. For $-h/2<v<0$, the bias is $\Delta_r(1/2+v/h)$; for $0<v<h/2$, it is $-\Delta_r(1/2-v/h)$. Endpoint values do not affect an $L^2$ norm. Integrating these two triangular errors gives

$$
\|K_h*f-f\|_2^2=\sum_{r=0}^k2\Delta_r^2\int_0^{h/2}(1/2-v/h)^2\,dv=\frac h{12}\sum_{r=0}^k\Delta_r^2.
$$

This is the [box-kernel bias of a piecewise constant density](../../../../../box-kernel-bias-of-a-piecewise-constant-density.md). By the triangle inequality, with $C_f=(\sum_r\Delta_r^2/12)^{1/2}$,

$$
\mathbb E\|\widehat f_{n,h}^K-f\|_2\le\frac1{\sqrt{nh}}+C_f\sqrt h.
$$

Balancing this [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md) with $h_n=n^{-1/2}$ gives, for all sufficiently large $n$,

$$
\boxed{\mathbb E\|\widehat f_{n,h_n}^K-f\|_2\le(1+C_f)n^{-1/4}=O(n^{-1/4}).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
