<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $\Omega=\Sigma^{-1}$, the [precision matrix](../../../../../precision-matrix.md). The [conditional independence graph](../../../../../conditional-independence-graph.md) has an edge between $j$ and $k$ exactly when $Z_j$ and $Z_k$ are not conditionally independent given all the remaining components. For the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md),

$$
\boxed{\{j,k\}\text{ is absent}\iff\Omega_{jk}=0.}
$$

Indeed, the conditional density of the pair given the others has its quadratic term determined by the corresponding two-by-two principal submatrix of $\Omega$; its cross term vanishes exactly when $\Omega_{jk}=0$, making the two conditional Gaussian variables independent. This is a [Gaussian graphical model](../../../../../gaussian-graphical-model.md).

To derive the conditional law of one component, isolate $z_k$ in the [multivariate normal density](../../../../../multivariate-normal-density.md) and complete the square. The terms involving it are

$$
-\frac12\Omega_{kk}(z_k-\mu_k)^2-(z_k-\mu_k)\Omega_{k,-k}(z_{-k}-\mu_{-k}).
$$

Therefore

$$
\boxed{Z_k\mid Z_{-k}=z_{-k}\sim N\left(\mu_k-\frac{\Omega_{k,-k}}{\Omega_{kk}}(z_{-k}-\mu_{-k}),\ \frac1{\Omega_{kk}}\right).}
$$

Equivalently, its mean is $\mu_k+\Sigma_{k,-k}\Sigma_{-k,-k}^{-1}(z_{-k}-\mu_{-k})$ and its variance is the [Schur complement](../../../../../schur-complement.md) $\Sigma_{kk}-\Sigma_{k,-k}\Sigma_{-k,-k}^{-1}\Sigma_{-k,k}$. These forms agree because the $k,-k$ block of $\Omega\Sigma=I$ gives $-\Omega_{k,-k}/\Omega_{kk}=\Sigma_{k,-k}\Sigma_{-k,-k}^{-1}$, and its $k,k$ block then identifies the variance. This proves the relevant [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) formula.

In particular, the population regression of component $k$ on the other components has coefficients

$$
\boxed{\theta_{jk}=-\frac{\Omega_{jk}}{\Omega_{kk}}\quad(j\ne k),}
$$

intercept $a_k=\mu_k-\mu_{-k}^{\mathsf T}\theta_{-k,k}$, and a Gaussian residual independent of the predictors with variance $1/\Omega_{kk}$. These are the [conditional regression coefficients from a Gaussian precision matrix](../../../../../conditional-regression-coefficients-from-a-gaussian-precision-matrix.md). The coefficient is zero exactly when the corresponding edge is absent. Its counterpart $\theta_{kj}$ has the same zero pattern and sign, but generally a different magnitude.

This motivates [nodewise regression](../../../../../nodewise-regression.md): for each $k$, regress $X_k$ on $X_{-k}$, estimating an intercept as well. For sparse graph estimation, use the [Nodewise Lasso](../../../../../nodewise-lasso.md) criterion

$$
\frac1{2n}\|X_k-a_k\mathbf1-X_{-k}b\|_2^2+\lambda_k\|b\|_1.
$$

The [Lasso](../../../../../lasso.md) penalty encourages many fitted coefficients to be zero and remains usable when the number of predictors exceeds the sample size. Ordinary unpenalized sample regressions would usually give a dense estimated graph. Separate regressions can disagree about a pair, so an undirected graph can use the [OR rule for nodewise graph selection](../../../../../or-rule-for-nodewise-graph-selection.md), retaining an edge if either fitted direction is nonzero, or the more conservative [AND rule for nodewise graph selection](../../../../../and-rule-for-nodewise-graph-selection.md), retaining it only if both are nonzero. These are choices for combining estimated neighbourhoods, rather than identities forced by finite-sample fits.

The printed joint objective uses a [Group Lasso](../../../../../group-lasso.md) penalty on the unordered pairs

$$
g_{jk}=(\Theta_{jk},\Theta_{kj}),\qquad\sum_{j<k}\|g_{jk}\|_2.
$$

This is [paired group Lasso for Gaussian graph estimation](../../../../../paired-group-lasso-for-gaussian-graph-estimation.md). Each group represents a single undirected edge, coupling its two directional regressions. A sum of group norms encourages entire pairs to be zero; a squared group norm would give smooth ridge-type shrinkage instead of edge deletion. The constraint $\Theta_{kk}=0$ removes self-prediction, and the intercepts are not penalized.

The free symbols called $\mu_k$ in the objective are regression intercepts, not generally the marginal means of the original Gaussian vector. Profiling them out gives

$$
\widehat a_k=\overline X_k-\overline X_{-k}^{\mathsf T}\widehat\Theta_{-k,k},
$$

and replaces all columns by their centred versions in the squared-error terms. This is [profiling intercepts in nodewise regression](../../../../../profiling-intercepts-in-nodewise-regression.md). Scaling predictors to comparable units can also help interpret a common penalty, although the displayed objective itself is well defined on the given data.

The grouped [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md) make the sparsity mechanism precise. With centred residuals $r_k=\widetilde X_k-\widetilde X_{-k}\Theta_{-k,k}$, define

$$
c_{jk}=\left(\frac{\widetilde X_j^{\mathsf T}r_k}{n},\ \frac{\widetilde X_k^{\mathsf T}r_j}{n}\right).
$$

The [subdifferential](../../../../../subdifferential.md) of the [Euclidean norm](../../../../../euclidean-norm.md) at zero is its closed unit ball, and away from zero is $g/\|g\|_2$. Hence a minimizer satisfies

$$
\boxed{g_{jk}=0\Longrightarrow\|c_{jk}\|_2\leq\lambda,\qquad
g_{jk}\ne0\Longrightarrow c_{jk}=\lambda\frac{g_{jk}}{\|g_{jk}\|_2}.}
$$

These are the [paired group Lasso optimality conditions](../../../../../paired-group-lasso-optimality-conditions.md). They jointly threshold the two directional scores, matching the population fact that both directions represent the same edge.

**Estimate the graph by including $\{j,k\}$ exactly when $\|\widehat g_{jk}\|_2>0$.** This graph is undirected by construction. The penalty does not impose $\Theta_{jk}=\Theta_{kj}$, nor does it mathematically require both coordinates of every selected pair to be nonzero. That distinction is appropriate because the population regression coefficients themselves need not have equal magnitudes. The fitted coefficient matrix is not automatically a symmetric positive definite [precision matrix](../../../../../precision-matrix.md); its pair supports, rather than its entries as a precision estimate, supply the requested [conditional independence graph](../../../../../conditional-independence-graph.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
