<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $v=\sigma^2$, $d=k+1$, $X=X_k$, $a=a_k$, $\mu=\mu_k$ and $\Sigma=\Sigma_k$, with $\Sigma$ [positive-definite](../../../../../../../positive-definite-bilinear-form.md). For fixed $v$, the terms involving $a$ in the posterior exponent are

$$
-\frac12\left[a^T\left(\frac{X^TX}{v}+\Sigma^{-1}\right)a-2a^T\left(\frac{X^Ty}{v}+\Sigma^{-1}\mu\right)\right].
$$

Complete the square. With $V_k=(X_k^TX_k/v+\Sigma_k^{-1})^{-1}$ and $m_k=V_k(X_k^Ty/v+\Sigma_k^{-1}\mu_k)$, this gives

$$
\boxed{a_k\mid v,x,y\sim N_{k+1}(m_k,V_k).}
$$

For fixed $a_k$, collect the powers and exponential terms involving $v$:

$$
\pi(v\mid a_k,x,y)\propto v^{-(\alpha+n/2)-1}\exp\left[-\frac{\beta+\tfrac12\|y-X_ka_k\|^2}{v}\right].
$$

Hence, in the paper's shape-scale [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md) convention,

$$
\boxed{v\mid a_k,x,y\sim\operatorname{IG}\left(\alpha+\frac n2,\beta+\frac12\|y-X_ka_k\|^2\right).}
$$

There is no extra $(k+1)/2$ in this shape, because the normal coefficient prior is independent of $v$. These are the [independent normal and inverse-gamma regression priors](../../../../../../../independent-normal-and-inverse-gamma-regression-priors.md) conditionals.

The Gaussian normalization printed in the PDF is incorrect. The proper $d$-dimensional prior [probability density function](../../../../../../../probability-density-function.md) is $(2\pi)^{-d/2}|\Sigma_k|^{-1/2}\exp[-(a_k-\mu_k)^T\Sigma_k^{-1}(a_k-\mu_k)/2]$. For fixed $k$ this correction is constant in $a_k,v$ and leaves the two conditionals unchanged, but it must be retained when comparing different model orders in part (b).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
