<h1 id="13j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on the observed colleges, the [stochastic block model](../../../../../../stochastic-block-model.md) assumes that the friendship indicators are [independent random variables](../../../../../../independent-random-variables.md). For arbitrary linear predictors $\theta_{ij}$, their [Bernoulli distribution](../../../../../../bernoulli-distribution.md) likelihood is

$$
L(\theta;y)
=\prod_{1\leq i<j\leq m}
\left(\frac{e^{\theta_{ij}}}{1+e^{\theta_{ij}}}\right)^{y_{ij}}
\left(\frac1{1+e^{\theta_{ij}}}\right)^{1-y_{ij}}
=\prod_{i<j}\frac{e^{y_{ij}\theta_{ij}}}{1+e^{\theta_{ij}}}.
$$

Thus the three requested likelihoods are

$$
\boxed{
\begin{aligned}
L_1(\beta;y)
&=\prod_{i<j}\frac{e^{y_{ij}\beta_{z_i z_j}}}{1+e^{\beta_{z_i z_j}}},\\
L_2(\beta;y)
&=\prod_{i<j}\frac{e^{y_{ij}(\beta_{z_i}+\beta_{z_j})}}{1+e^{\beta_{z_i}+\beta_{z_j}}},\\
L_3(\beta;y)
&=\prod_{i<j}
\frac{e^{y_{ij}(\beta_{z_i}+\beta_{z_j}+\beta_0\delta_{z_i z_j})}}
{1+e^{\beta_{z_i}+\beta_{z_j}+\beta_0\delta_{z_i z_j}}}.
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
