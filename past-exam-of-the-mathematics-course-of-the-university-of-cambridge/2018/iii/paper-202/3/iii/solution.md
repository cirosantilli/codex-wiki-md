<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiplication by the integrating factor $e^{t/2}$ and the [Itô product rule](../../../../../../ito-product-rule.md) give the [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md)

$$
X_t=e^{-t/2}X_0+\int_0^te^{-(t-u)/2}\,dB_u.
$$

The two summands are [independent](../../../../../../independent-random-variables.md) centered [normal](../../../../../../normal-distribution.md) [random variables](../../../../../../random-variable-split.md), because $X_0$ is [independent](../../../../../../independent-random-variables.md) of the [Brownian motion](../../../../../../brownian-motion-split.md) and the integrand is deterministic. By the [Itô isometry](../../../../../../ito-isometry.md), their [variances](../../../../../../variance-split.md) sum to $e^{-t}+\int_0^te^{-(t-u)}du=1$. Thus

$$
\boxed{X_t\sim N(0,1)\quad(t\geq0).}
$$

For $t\geq s$, split the [Itô integral](../../../../../../ito-integral.md) at $s$ to obtain $X_t=e^{-(t-s)/2}X_s+\int_s^te^{-(t-u)/2}dB_u$, where the latter term is centered and [independent](../../../../../../independent-random-variables.md) of $X_s$. Consequently

$$
\boxed{\operatorname{Cov}(X_t,X_s)=e^{-|t-s|/2}.}
$$

In particular this initialization makes the [Gaussian process](../../../../../../gaussian-process.md) a [stationary process](../../../../../../stationary-process.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
