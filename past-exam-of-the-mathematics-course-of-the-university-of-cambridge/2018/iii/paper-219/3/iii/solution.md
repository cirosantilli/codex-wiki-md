<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At the fitted [hyperparameters](../../../../../../hyperparameter.md), define $K= k_0(t,t)$, $K_{**}=k_0(t^*,t^*)$, and $K_{*t}=k_0(t^*,t)$, with the matrices formed by pairwise kernel evaluations. Conditional independence of observation noise and future latent values gives

$$
\begin{pmatrix}y\\f_*\end{pmatrix}\sim N\left(0,\begin{pmatrix}V&K_{t*}\\K_{*t}&K_{**}\end{pmatrix}\right),\qquad V=K+R.
$$

The residual $f_*-K_{*t}V^{-1}y$ has zero [covariance](../../../../../../covariance.md) with $y$, so the joint normal law makes it independent of $y$. This derives the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) and the [Gaussian process regression posterior](../../../../../../gaussian-process-regression-posterior.md):

$$
\boxed{f_*\mid y,t,t^*,\widehat{\mathcal H}\sim N(m_*,\Sigma_*),\qquad m_*=K_{*t}V^{-1}y,\qquad\Sigma_*=K_{**}-K_{*t}V^{-1}K_{t*}}.
$$

The [covariance](../../../../../../covariance.md) is a [Schur complement](../../../../../../schur-complement.md) and is positive semidefinite. When nonsingular, its joint density is $(2\pi)^{-M/2}|\Sigma_*|^{-1/2}\exp[-\frac12(f_*-m_*)^T\Sigma_*^{-1}(f_*-m_*)]$. Repeated phases can make it singular, in which case the displayed normal law is interpreted on its support.

This predicts the true latent [light curve](../../../../../../light-curve.md), so no future measurement [variance](../../../../../../variance-split.md) is added. For noisy future observations, add their independent noise [covariance](../../../../../../covariance.md) to $\Sigma_*$. Fixing the [hyperparameters](../../../../../../hyperparameter.md) omits their estimation uncertainty, as requested; integrating over their posterior would add it. The periodic model extrapolates by phase, even though all prediction times follow the observed times.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
