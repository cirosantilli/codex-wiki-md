<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [ordinary least squares](../../../../../../ordinary-least-squares.md) equations for model 2 are

$$
X^T(\log T-X\widehat\alpha)=0.
$$

For the Gamma [generalized linear model](../../../../../../generalized-linear-model.md), $V(\mu)=\mu^2$ and $d\mu/d\eta=\mu$, so its score equation under the logarithmic link is

$$
X^T\left(\frac{T}{\mu}-\mathbf1\right)=0,
\qquad \mu_i=e^{x_i^T\widehat\gamma}.
$$

When $T_i$ is close to $\mu_i$,

$$
\frac{T_i}{\mu_i}-1
=e^{\log T_i-\log\mu_i}-1
\simeq\log T_i-x_i^T\widehat\gamma
$$

by the first-order [Taylor expansion](../../../../../../taylor-expansion.md) of the exponential function. The Gamma score equations then become the model-2 normal equations, so their coefficient estimates are close.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
