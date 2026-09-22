<h1 id="d/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [dominated differentiation under the integral sign](../../../../dominated-differentiation-under-the-integral-sign.md) suffices. Suppose $\phi(\cdot,t)$ is measurable, $\phi(\cdot,t_0)$ is integrable at one parameter value, and for almost every $x$ the map $t\mapsto\phi(x,t)$ is continuously differentiable on an interval. If $|\partial_t\phi(x,t)|\leq H(x)$ throughout that interval for an integrable $H$, then the parameter integral is differentiable, and

$$
\frac d{dt}\int\phi(x,t)dx=\int\partial_t\phi(x,t)dx.
$$

One direct sufficient version assumes $\partial_t\phi(x,t)$ is continuous in $t$ almost everywhere and has that common domination; [dominated convergence theorem](../../../../dominated-convergence-theorem.md) then proves the assertion.

Here $|f(x)e^{itx}|=|f(x)|$, so the [complex-valued function](../../../../complex-valued-function.md) $h$ is integrable for every real $t$. For a real increment $u\neq0$, the elementary bound $|e^{iux}-1|\leq|ux|$ gives

$$
\left|f(x)e^{itx}\frac{e^{iux}-1}{u}\right|
\leq|xf(x)|.
$$

The right side is integrable by hypothesis and the integrand converges pointwise to $ixf(x)e^{itx}$. [dominated convergence theorem](../../../../dominated-convergence-theorem.md), applied to real and imaginary parts, proves

$$
\boxed{\widehat f'(t)=\int_{\mathbb R}ixf(x)e^{itx}dx.}
$$

This supplies the domination explicitly rather than merely differentiating a formal [Fourier transform](../../../../fourier-transform-split.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [D](../../d.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
