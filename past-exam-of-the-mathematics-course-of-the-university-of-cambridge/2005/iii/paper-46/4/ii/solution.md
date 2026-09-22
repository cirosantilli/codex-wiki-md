<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Factor analysis](../../../../../../factor-analysis.md) models a large set of correlated measurements using a smaller collection of shared [latent factors](../../../../../../latent-factor.md) and variable-specific variation. A classical [orthogonal factor model](../../../../../../orthogonal-factor-model.md) is

$$
\boxed{X=\mu+LF+\epsilon,\quad\mathbb EF=0,\quad\operatorname{Cov}(F)=I_q,\quad\operatorname{Cov}(\epsilon)=\Psi=\operatorname{diag}(\psi_1,\ldots,\psi_p),\quad\operatorname{Cov}(F,\epsilon)=0.}
$$

Take $q<p$, centered errors, and positive specific [variances](../../../../../../variance-split.md) for the inverse-covariance and [likelihood](../../../../../../likelihood-function.md) formulas below. The [factor loadings](../../../../../../factor-loading.md) form the $p\times q$ [matrix](../../../../../../matrix.md) $L$, and the model [covariance](../../../../../../covariance.md) is

$$
\Sigma=LL^T+\Psi.
$$

Thus for $i\ne k$, $\operatorname{Cov}(X_i,X_k)=\sum_jL_{ij}L_{kj}$; the common [latent factors](../../../../../../latent-factor.md) explain off-diagonal [correlation](../../../../../../pearson-correlation-coefficient.md). The [communality](../../../../../../communality.md) of variable $i$ is $h_i^2=\sum_jL_{ij}^2$, and $\operatorname{Var}(X_i)=h_i^2+\psi_i$. For standardized variables this is $1=h_i^2+\psi_i$. The specific [variance](../../../../../../variance-split.md) represents measurement noise or genuinely unshared variation; it is not another common [latent factor](../../../../../../latent-factor.md).

This differs from [principal component analysis](../../../../../../principal-component-analysis.md). A [principal component](../../../../../../principal-component.md) maximizes projected total [variance](../../../../../../variance-split.md) and is a determined linear score after choosing its direction; a factor model attempts to explain shared [covariance](../../../../../../covariance.md) while reserving diagonal specific [variance](../../../../../../variance-split.md). Low-dimensional [PCA](../../../../../../principal-component-analysis.md) truncation can help initialize a factor fit, but it does not justify setting all specific [variances](../../../../../../variance-split.md) to zero. [Latent factors](../../../../../../latent-factor.md) are unobserved, not directly observed scores. When the [latent factors](../../../../../../latent-factor.md) and the errors are jointly Gaussian, their [conditional mean](../../../../../../conditional-expectation.md) is

$$
\mathbb E(F\mid X=x)=L^T\Sigma^{-1}(x-\mu),
$$

which supplies one factor-score estimate, with remaining uncertainty. This follows from the block conditional normal formula in Question 1; it does not make the [latent factor](../../../../../../latent-factor.md) uniquely recoverable from one observation.

For the Gaussian [likelihood](../../../../../../likelihood-function.md), use the empirical covariance $S_0=n^{-1}\sum_i(x_i-\bar x)(x_i-\bar x)^T$. Fit the factor model by minimizing $\log|LL^T+\Psi|+\operatorname{tr}(S_0(LL^T+\Psi)^{-1})$ subject to admissible specific [variances](../../../../../../variance-split.md). Other approaches estimate [communalities](../../../../../../communality.md) and extract [latent factors](../../../../../../latent-factor.md) from the reduced [correlation matrix](../../../../../../correlation-matrix.md). Choose $q$ using substantive plausibility, a [scree plot](../../../../../../scree-plot.md), fitted residual [correlations](../../../../../../pearson-correlation-coefficient.md) and model-fit assessment. Under local [identifiability](../../../../../../identifiability.md), a [likelihood](../../../../../../likelihood-function.md) goodness-of-fit count for the [covariance](../../../../../../covariance.md) model is

$$
\frac{p(p+1)}2-\left[pq+p-\frac{q(q-1)}2\right],
$$

where the subtracted rotational dimension must be removed from the loading parameter count. This count alone does not establish [identifiability](../../../../../../identifiability.md), and boundary fits with zero specific [variance](../../../../../../variance-split.md) need special care.

[Factor rotation](../../../../../../factor-rotation.md) addresses interpretability and nonuniqueness. For every [orthogonal matrix](../../../../../../orthogonal-matrix.md) $Q$, replace $(L,F)$ by $(LQ,Q^TF)$; then $(LQ)(LQ)^T=LL^T$, so the fit is unchanged. The absolute orientation of unrestrained [latent factors](../../../../../../latent-factor.md) is therefore not identified by the [covariance](../../../../../../covariance.md). [Varimax rotation](../../../../../../varimax-rotation.md) chooses orthogonal axes favoring a simple pattern of large and small squared loadings. Oblique rotation can permit correlated [latent factors](../../../../../../latent-factor.md), provided their [covariance](../../../../../../covariance.md) is transformed consistently. Sign changes and permutations are further harmless relabelings; an interpretation must state its chosen convention.

<a id="4/ii/image-two-factor-loading-directions-an-equivalent-rotated-representation-and-the-covariance-scree-plot"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46-factor-rotation.png)

**[Figure 3](#4/ii/image-two-factor-loading-directions-an-equivalent-rotated-representation-and-the-covariance-scree-plot). Two-factor loading directions, an equivalent rotated representation and the covariance scree plot**.

The sketch uses four standardized hypothetical measurements sharing two orthogonal [latent factors](../../../../../../latent-factor.md). Rotating the factor coordinates changes the loading descriptions while preserving every implied [covariance](../../../../../../covariance.md) and [communality](../../../../../../communality.md); the scree plot belongs to that same constructed [covariance matrix](../../../../../../covariance-matrix.md). **[Factor analysis](../../../../../../factor-analysis.md) separates shared variation from specific [variance](../../../../../../variance-split.md), and its [latent factors](../../../../../../latent-factor.md) require an identifying or interpretive orientation.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
