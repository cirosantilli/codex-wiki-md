<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\tau=T-t$ and $a=e^{-\alpha\tau}$. The [stochastic integral](../../../../stochastic-integral.md) in [b](../b.md) has a deterministic integrand, so it is a [Gaussian random variable](../../../../gaussian-random-variable.md) independent of the information available at $t$. Its [variance](../../../../variance-split.md), by the [Itô isometry](../../../../ito-isometry.md), is

$$
v=\sigma^2 e^{-2\alpha T}\int_t^T e^{2\alpha u}du=\frac{\sigma^2}{2\alpha}(1-a^2).
$$

Thus $x_T$ conditionally has a [normal distribution](../../../../normal-distribution.md) with [expected value](../../../../expected-value-split.md) $m=ax_t+(1-a)\widetilde\mu$ and [variance](../../../../variance-split.md) $v$. The [moment-generating function of a normal distribution](../../../../moment-generating-function-of-a-normal-distribution.md) gives $\mathbb E_t[e^{x_T}]=e^{m+v/2}$, so the [conditional mean of a log-mean-reverting price](../../../../conditional-mean-of-a-log-mean-reverting-price.md) is

$$
\boxed{F(t,T)=\exp\!\left[e^{-\alpha(T-t)}\log S_t+\widetilde\mu(1-e^{-\alpha(T-t)})+\frac{\sigma^2}{4\alpha}(1-e^{-2\alpha(T-t)})\right]}.
$$

The correction $v/2$ is essential: exponentiating the conditional mean of the logarithm alone would omit the dispersion of the [lognormal distribution](../../../../log-normal-distribution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
