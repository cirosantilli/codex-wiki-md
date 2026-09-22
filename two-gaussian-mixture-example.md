# Two-Gaussian mixture example

↑ **Parent:** [Finite mixture model](finite-mixture-model.md)

Stipulate an original [Gaussian mixture distribution](gaussian-mixture-distribution.md) with [mixture weights](mixture-weight.md) $\pi_1=1/3$, $\pi_2=2/3$, component [means](expected-value-split.md) $\mu_1=-2$, $\mu_2=2$, and component [variances](variance-split.md) both equal to one. These are chosen [statistical parameters](statistical-parameter.md), with no observed sample or fitting. If $\phi(t)=(2\pi)^{-1/2}e^{-t^2/2}$ is the [standard normal distribution](standard-normal-distribution.md) [probability density function](probability-density-function.md), then

$$
f(x)=\frac13\phi(x+2)+\frac23\phi(x-2).
$$

In the figure, the two colored curves are weighted [probability density functions](probability-density-function.md), with areas $1/3$ and $2/3$. Adding their heights at every $x$ gives the black curve. Neither colored curve stops at a dividing line.

<a id="image-stipulated-two-gaussian-mixture-weighted-component-densities-and-their-sum"></a>
![](two-gaussian-mixture-density-decomposition.png)

**[Figure 5](#image-stipulated-two-gaussian-mixture-weighted-component-densities-and-their-sum). Stipulated two-Gaussian mixture: weighted component densities and their sum**. Original analytic curves for component means $-2$ and $2$, component variances one, and mixture weights $1/3$ and $2/3$. No observed points, histogram, or fitted parameters are used.

The [law of total expectation](law-of-total-expectation.md) and [law of total variance](law-of-total-variance.md) give the total [mean](expected-value-split.md) and [variance](variance-split.md):

$$
\mathbb E[X]=\frac13(-2)+\frac23(2)=\frac23,
\qquad
\operatorname{Var}(X)=\underbrace{1}_{\mathbb E[\operatorname{Var}(X\mid Z)]}+\underbrace{\frac13\left(-2-\frac23\right)^2+\frac23\left(2-\frac23\right)^2}_{\operatorname{Var}(\mathbb E[X\mid Z])=32/9}=\frac{41}{9}.
$$

All of the extra [variance](variance-split.md) $32/9$ comes from variation between component [means](expected-value-split.md). Equivalently, the second [moment](moment.md) is $\mathbb E[X^2]=1+4=5$, so the [variance](variance-split.md) is $5-(2/3)^2$.

A [mixture distribution](mixture-distribution.md) is different from a deterministic [linear combination](linear-combination.md) of [random variables](random-variable-split.md). If independent $Y_1\sim N(-2,1)$ and $Y_2\sim N(2,1)$ are drawn and $W=Y_1/3+2Y_2/3$, then $W$ has a [normal distribution](normal-distribution.md) with the same [mean](expected-value-split.md) $2/3$ but [variance](variance-split.md) $1/9+4/9=5/9$, rather than $41/9$. Every draw of $W$ uses both [random variables](random-variable-split.md). A draw from the [mixture distribution](mixture-distribution.md) instead uses $X=I_1Y_1+I_2Y_2$, where the [mixture allocation indicators](mixture-allocation-indicator.md) are independent of $(Y_1,Y_2)$ and select exactly one of them. The expression for $f$ adds densities, not simultaneous random outcomes.

## ↑ Ancestors (8)

1. [Finite mixture model](finite-mixture-model.md)
2. [Mixture model](mixture-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Mixture model](mixture-model.md)
- [Responsibility curve for a two-Gaussian mixture](responsibility-curve-for-a-two-gaussian-mixture.md)
