<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [periodic covariance function](../../../../../../periodic-covariance-function.md)

$$
k_P(t,t')=A^2\exp\left[-\frac2{\ell^2}\sin^2\left(\frac{\pi(t-t')}P\right)\right],\qquad\mathcal H=(A,\ell,P),\quad A,\ell,P>0.
$$

Its positive semidefiniteness follows by pulling back a [Gaussian kernel](../../../../../../gaussian-kernel.md) to the circle $(\cos(2\pi t/P),\sin(2\pi t/P))$. A zero [Gaussian process](../../../../../../gaussian-process.md) mean is an ensemble statement, whereas an exactly zero long-term average for every periodic [light curve](../../../../../../light-curve.md) is stronger. To impose the latter literally, use a [periodic Gaussian process with zero period average](../../../../../../periodic-gaussian-process-with-zero-period-average.md), replacing the kernel by

$$
k_0(t,t')=k_P(t,t')-c_0,\qquad c_0=A^2e^{-\ell^{-2}}I_0(\ell^{-2}).
$$

Here $I_0$ is a [modified Bessel function](../../../../../../modified-bessel-function.md), and $c_0$ is the period average of the kernel. Subtracting each process's random period average produces this [covariance](../../../../../../covariance.md), so it remains positive semidefinite. We use $k_0$ to enforce the stated mean subtraction; using $k_P$ gives the usual ensemble-zero-mean formulation and the same likelihood derivation.

Let $K_{ij}=k_0(t_i,t_j)$ and $R=\operatorname{diag}(\sigma_1^2,\ldots,\sigma_N^2)$. The prior latent vector is $f\sim N(0,K)$ and the independent [Gaussian noise](../../../../../../gaussian-noise.md) is $\varepsilon\sim N(0,R)$, so $y=f+\varepsilon\sim N(0,V)$ with $V=K+R$. The [Gaussian-process marginal likelihood](../../../../../../gaussian-process-marginal-likelihood.md) is

$$
\boxed{p(y\mid t,\mathcal H)=(2\pi)^{-N/2}|V|^{-1/2}\exp(-\tfrac12y^TV^{-1}y)}.
$$

Positive measurement [variances](../../../../../../variance-split.md) make $V$ positive definite even if $K$ is singular. Maximize $\ell(\mathcal H)=-\frac12y^TV^{-1}y-\frac12\log|V|-\frac N2\log(2\pi)$ over all three [hyperparameters](../../../../../../hyperparameter.md), using a broad search in $P$ to find competing aliases, followed by joint optimization. [Cholesky decomposition](../../../../../../cholesky-decomposition.md) evaluates the likelihood without explicitly forming an inverse.

For a well-resolved interior maximum, let $J=-\nabla^2\ell(\widehat{\mathcal H})$ be the [Observed Fisher information](../../../../../../observed-fisher-information.md) in the coordinates $(A,\ell,P)$. Then $\boxed{\widehat P=(\widehat{\mathcal H})_P,\qquad\sigma_P\approx\sqrt{(J^{-1})_{PP}}}$. Equivalently, the profile-likelihood curvature in $P$ gives the same local nuisance-adjusted [variance](../../../../../../variance-split.md); keeping the other [hyperparameters](../../../../../../hyperparameter.md) fixed would generally underestimate it. A profile interval with $\ell_{\rm prof}(\widehat P)-\ell_{\rm prof}(P)=1/2$ is a local $1\sigma$ approximation. If the period likelihood is multimodal or poorly constrained, fit the complete posterior with proper [hyperparameter](../../../../../../hyperparameter.md) priors and report its modes and marginal credible intervals rather than a single Hessian error bar. The sampling pattern can create period aliases that a single local search misses.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
