<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

A valid [covariance matrix](../../../../../../covariance-matrix.md) must be real symmetric and a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md), with $C_{ii}=\sigma_i^2\ge0$. Conversely, every such matrix is the [covariance](../../../../../../covariance.md) of a possibly degenerate [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md). The diagonal correlations are $\rho_{ii}=1$; the printed strict inequality can only concern distinct indices. Pairwise bounds do not suffice: the $3$ by $3$ correlation matrix with diagonal $1$ and every off-diagonal entry $-0.9$ has [eigenvalue](../../../../../../eigenvalue.md) $-0.8$ along $\mathbf1$ and is invalid. Even strict pairwise inequalities allow singularity: off-diagonal entries $-1/2$ give an [eigenvalue](../../../../../../eigenvalue.md) zero.

For the inverse requested in the question, assume in addition that $C$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md). Write $x=(\widehat\mu_i)$, $\Lambda=C^{-1}$ and $S=\mathbf1^T\Lambda\mathbf1>0$. Up to a constant, the [log-likelihood](../../../../../../log-likelihood.md) is $-\frac12(x-\mu\mathbf1)^T\Lambda(x-\mu\mathbf1)$. Its [score function](../../../../../../informant-function.md) and second derivative are

$$
\ell'(\mu)=\mathbf1^T\Lambda(x-\mu\mathbf1),\qquad\ell''(\mu)=-S<0.
$$

The [correlated Gaussian common-mean estimator](../../../../../../correlated-gaussian-common-mean-estimator.md) is therefore

$$
\boxed{\widehat\mu_{\rm MLE}=\frac{\mathbf1^T\Lambda x}{\mathbf1^T\Lambda\mathbf1}=\frac{\sum_{i,j}\Lambda_{ij}\widehat\mu_j}{\sum_{i,j}\Lambda_{ij}}}.
$$

Its expectation is $\mu$, and direct [covariance](../../../../../../covariance.md) propagation gives

$$
\boxed{\operatorname{Bias}(\widehat\mu_{\rm MLE})=0,\qquad\operatorname{Var}(\widehat\mu_{\rm MLE})=\frac{\mathbf1^T\Lambda C\Lambda\mathbf1}{S^2}=S^{-1}}.
$$

The [Fisher information](../../../../../../fisher-information-matrix.md) is $-\mathbb E\ell''(\mu)=S$, so this [variance](../../../../../../variance-split.md) attains the [Cramér-Rao bound](../../../../../../cramer-rao-bound.md) and the estimator is an [efficient estimator](../../../../../../efficient-estimator.md).

If $C$ is singular, an ordinary Lebesgue density and $C^{-1}$ are unavailable. When $\mathbf1$ lies in the range of $C$, the same formulas hold on that range with its [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md). Otherwise there is $u\in\ker C$ with $u^T\mathbf1\ne0$, and $u^Tx=\mu u^T\mathbf1$ determines $\mu$ exactly with zero [variance](../../../../../../variance-split.md). The usual nonsingular Cramér–Rao calculation then does not apply.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
