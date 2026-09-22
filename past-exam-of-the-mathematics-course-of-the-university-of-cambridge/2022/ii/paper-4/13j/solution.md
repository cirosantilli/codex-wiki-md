<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

This is [attenuation bias from classical measurement error](../../../../../attenuation-bias-from-classical-measurement-error.md), also called regression dilution. The latent predictor is $Z$, but $X_1$ and $X_2$ are noisy proxies. The noisier proxy produces a slope closer to zero.

For a regression with an intercept, the population slope is

$$
\frac{\operatorname{Cov}(X,Y)}{\operatorname{Var}(X)}.
$$

Here all variables are centred and the noises are independent. Therefore

$$
\operatorname{Cov}(Z,Y)=\beta\sigma_z^2,
\qquad
\operatorname{Var}(Z)=\sigma_z^2,
$$

so regressing $Y$ on $Z$ has slope $\beta=2$. For

$$
X_j=Z+\eta_j,
$$

we have

$$
\operatorname{Cov}(X_j,Y)=\beta\sigma_z^2,
\qquad
\operatorname{Var}(X_j)=\sigma_z^2+\sigma_{x_j}^2.
$$

Thus

$$
\boxed{
\beta_{\rm slope}(Y\sim X_j)
=\beta\frac{\sigma_z^2}
{\sigma_z^2+\sigma_{x_j}^2}
}.
$$

With the stated values, the slopes are

$$
2\frac1{1+0.5^2}=1.6,
\qquad
2\frac1{1+1^2}=1,
$$

matching the simulation.

Under this independent additive measurement-error model, the magnitude of the $Y$-on-$X_1$ slope is generally smaller than the magnitude of the $Y$-on-$Z$ slope whenever $\sigma_{x_1}^2>0$. Increasing $\sigma_y$ does not change the population slope, because response noise contributes neither to $\operatorname{Cov}(X_1,Y)$ nor to $\operatorname{Var}(X_1)$. It increases residual variance and the sampling variability of the estimate; with one million observations, doubling it should leave the displayed slope close to $1.6$ while increasing its standard error.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
