<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Laplace approximation](../../../../../../laplace-approximation.md) evaluates an integral dominated by an interior maximum. Suppose $h$ has a unique interior maximizer $x_0\in\mathbb R^d$, negative-definite Hessian there, and sufficient smoothness and tail control. Put $H=-\nabla^2h(x_0)>0$. Taylor expansion under $x=x_0+u/\sqrt n$ gives a Gaussian leading integrand and

$$
\boxed{\int e^{nh(x)}g(x)dx=e^{nh(x_0)}g(x_0)\left(\frac{2\pi}{n}\right)^{d/2}|H|^{-1/2}\{1+O(n^{-1})\}.}
$$

The leading factor follows from the multivariate [Gaussian integral](../../../../../../gaussian-integral.md). Odd cubic terms integrate to zero over the limiting symmetric domain; fourth-order terms and squared cubic terms contribute to the first correction, assuming enough derivatives. If $g(x_0)=0$, a different leading term may be needed.

For a likelihood integral with prior density $\pi$, a common version is $\int e^{\ell(\theta)}\pi(\theta)d\theta\approx e^{\ell(\widehat\theta)}\pi(\widehat\theta)(2\pi)^{d/2}|j(\widehat\theta)|^{-1/2}$, because observed information is of order $n$. This is useful for posterior normalization, marginal likelihood and approximating integrated nuisance effects. A prior or integration measure is part of that construction; integrating nuisance parameters is different from merely profiling them. Boundary maxima, degenerate curvature, multiple modes or uncontrolled tails invalidate the simple one-mode formula.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
