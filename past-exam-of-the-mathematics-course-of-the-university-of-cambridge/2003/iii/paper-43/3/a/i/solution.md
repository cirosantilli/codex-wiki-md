<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $v_i=\sigma_i^2$ for each component [variance](../../../../../../../variance-split.md) and $\tau^2$ for the fixed prior [variance](../../../../../../../variance-split.md) denoted $\sigma^2$ in the source; these must not be confused. Let $\varphi(x;\mu,v)$ be the [normal distribution](../../../../../../../normal-distribution.md) [probability density function](../../../../../../../probability-density-function.md) and $D_j=\sum_{i=1}^k\omega_i\varphi(x_j;\mu_i,v_i)$. Independent observations and independent parameter priors give the [posterior distribution](../../../../../../../bayesian-posterior.md)

$$
\boxed{\pi(\boldsymbol\mu,\mathbf v,\boldsymbol\omega\mid\mathbf x)\propto\left[\prod_{j=1}^nD_j\right]\prod_{i=1}^k\left\{\exp\left(-\frac{\mu_i^2}{2\tau^2}\right)v_i^{-\alpha-1}\exp\left(-\frac\beta{v_i}\right)\omega_i^{\epsilon_i-1}\right\}.}
$$

Its support has $v_i>0$, $\omega_i>0$ and $\sum_i\omega_i=1$, with $\alpha,\beta,\tau^2,\epsilon_i>0$. The component means have independent fixed-variance [priors](../../../../../../../prior-probability.md) with a [normal distribution](../../../../../../../normal-distribution.md), not means with variances proportional to $v_i$. The factor $e^{-\beta/v_i}$ follows from the stated [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md). The later printed augmented expression instead has $e^{-\beta v_i}$ and an undefined prior mean; those are inconsistent with this specification. The intended model uses $e^{-\beta/v_i}$ and prior mean zero throughout.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
