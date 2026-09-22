<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [finite Gaussian mixture with a common variance](../../../../../../finite-gaussian-mixture-with-a-common-variance.md), introduce independent latent labels $Z_i\in\{1,\ldots,k\}$ with probabilities $\pi_j>0$, $\sum_j\pi_j=1$, and conditional responses $Y_i\mid Z_i=j\sim N(\mu_j,\sigma^2)$, with common $\sigma^2>0$. The observed density and [log-likelihood](../../../../../../log-likelihood.md) are

$$
f(y)=\sum_{j=1}^k\pi_j\phi(y;\mu_j,\sigma^2),\qquad
\ell=\sum_{i=1}^n\log\left\{\sum_j\pi_j\phi(y_i;\mu_j,\sigma^2)\right\}.
$$

The [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) replaces the difficult log of sums by an expected complete-data objective. Choose positive initial weights and variance and separated initial means. At iteration $r$, the E-step computes the [mixture responsibilities](../../../../../../mixture-responsibility.md)

$$
\tau_{ij}^{(r)}=\mathbb P_{\theta^{(r)}}(Z_i=j\mid y_i)
=\frac{\pi_j^{(r)}\exp\{-(y_i-\mu_j^{(r)})^2/(2\sigma^{2(r)})\}}
{\sum_{l=1}^k\pi_l^{(r)}\exp\{-(y_i-\mu_l^{(r)})^2/(2\sigma^{2(r)})\}}.
$$

The common normalizing factor cancels. For numerical stability the probabilities can be evaluated by subtracting the largest log weight before exponentiating.

With the old responsibilities held fixed, the expected complete-data [log-likelihood](../../../../../../log-likelihood.md), up to irrelevant constants, is

$$
Q=\sum_{i,j}\tau_{ij}^{(r)}\log\pi_j-\frac n2\log\sigma^2
-\frac1{2\sigma^2}\sum_{i,j}\tau_{ij}^{(r)}(y_i-\mu_j)^2.
$$

Let $N_j=\sum_i\tau_{ij}^{(r)}$. A Lagrange multiplier for $\sum_j\pi_j=1$, weighted least squares for the means, and differentiation in the common variance give the M-step:

$$
\boxed{\pi_j^{(r+1)}=\frac{N_j}{n},\qquad
\mu_j^{(r+1)}=\frac{\sum_i\tau_{ij}^{(r)}y_i}{N_j},\qquad
\sigma^{2(r+1)}=\frac1n\sum_{i,j}\tau_{ij}^{(r)}(y_i-\mu_j^{(r+1)})^2.}
$$

The variance update uses the **new means and old responsibilities**, with denominator $n$, not a residual degrees-of-freedom adjustment: this is [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md). Repeat the E- and M-steps until the observed [log-likelihood](../../../../../../log-likelihood.md) and parameters stabilize.

By [EM likelihood monotonicity](../../../../../../em-likelihood-monotonicity.md), exact updates do not decrease the observed likelihood. They need not reach its global maximum, so use several starting configurations and keep the best converged fit, checking for empty or nearly empty components and vanishing variance. The labels are interchangeable; sorting means after fitting supplies an interpretable labeling. Distinct starting means do not guarantee that all fitted components remain distinct. With a common variance and the usual fixed small $k$ relative to distinct observations the model avoids the individual-component variance-collapse pathology of unrestricted Gaussian mixtures, but degenerate data or too many components still require attention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
