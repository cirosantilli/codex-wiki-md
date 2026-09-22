<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Now complete the square in the other order:

$$
a^2-2\rho ab+b^2=(a-\rho b)^2+(1-\rho^2)b^2.
$$

Divide the joint [probability density function](../../../../../../probability-density-function.md) by the positive marginal density

$$
f_{X_2}(x_2)=\frac1{\sqrt{2\pi}\sigma_2}e^{-b^2/2}.
$$

The factor $e^{-b^2/2}$ cancels, giving the [conditional probability density](../../../../../../conditional-density.md)

$$
f_{X_1\mid X_2=x_2}(x_1)=
\frac1{\sqrt{2\pi}\sigma_1\sqrt{1-\rho^2}}
\exp\left[-\frac{(a-\rho b)^2}{2(1-\rho^2)}\right].
$$

Since

$$
a-\rho b=\frac{x_1-\left(\mu_1+\rho\sigma_1(x_2-\mu_2)/\sigma_2\right)}{\sigma_1},
$$

this is a normalized [normal distribution](../../../../../../normal-distribution.md) density. **Hence**

$$
\boxed{X_1\mid X_2=x_2\sim
N\left(\mu_1+\rho\frac{\sigma_1}{\sigma_2}(x_2-\mu_2),
\ \sigma_1^2(1-\rho^2)\right).}
$$

Conditioning on an exact observation is interpreted through this [conditional probability density](../../../../../../conditional-density.md), rather than conditioning by a ratio of event [probabilities](../../../../../../probability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
