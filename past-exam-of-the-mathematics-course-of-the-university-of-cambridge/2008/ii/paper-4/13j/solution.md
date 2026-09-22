<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

Write $\theta_i=\theta(\mu_i)$ and $\eta_i=x_i^T\beta=g(\mu_i)$. Differentiating $\mu_i=K'(\theta_i)$ gives $d\mu_i/d\theta_i=V(\mu_i)$, so

$$
\frac{\partial\theta_i}{\partial\beta_j}
=\frac{x_{ij}}{V(\mu_i)g'(\mu_i)}.
$$

In the [independent](../../../../../independent-random-variables.md) [exponential dispersion family](../../../../../exponential-dispersion-model.md), only $[y_i\theta_i-K(\theta_i)]/\sigma_i^2$ depends on $\beta$. Its derivative therefore gives the [score function](../../../../../informant-function.md)

$$
\boxed{U_j=\sum_i\frac{(y_i-\mu_i)x_{ij}}{\sigma_i^2V(\mu_i)g'(\mu_i)}.}
$$

The residuals are [independent](../../../../../independent-random-variables.md), have mean zero and variance $\sigma_i^2V(\mu_i)$. Consequently their score covariance is the [Fisher information matrix](../../../../../fisher-information-matrix.md):

$$
\boxed{\mathcal I_{jk}=\mathbb E(U_jU_k)
=\sum_i\frac{x_{ij}x_{ik}}{\sigma_i^2V(\mu_i)[g'(\mu_i)]^2}.}
$$

This also equals minus the expected likelihood Hessian under the usual regularity conditions.

For the [canonical link function](../../../../../canonical-link-function.md), $g(\mu)=\theta(\mu)$ and $g'=1/V$, so

$$
\boxed{U_j=\sum_i\frac{(y_i-\mu_i)x_{ij}}{\sigma_i^2},\qquad
\mathcal I_{jk}=\sum_i\frac{V(\mu_i)x_{ij}x_{ik}}{\sigma_i^2}.}
$$

To obtain the [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md), solve $U(\widehat\beta)=0$, for example with [Fisher scoring](../../../../../scoring-algorithm.md) iterations $\beta^{new}=\beta+\mathcal I(\beta)^{-1}U(\beta)$. Equivalently use [iteratively reweighted least squares](../../../../../iteratively-reweighted-least-squares.md), with weights $[\sigma_i^2V(\mu_i)g'(\mu_i)^2]^{-1}$ and working response $\eta_i+(y_i-\mu_i)g'(\mu_i)$. Since $\sigma_i^2=\sigma^2a_i$, the common dispersion scale cancels from this update for $\beta$. A nonsingular information matrix and a finite interior likelihood maximum are needed; iteration does not assert those for every possible dataset.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
