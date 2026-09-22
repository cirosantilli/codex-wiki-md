<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The command centres the log measurements and performs [principal component analysis](../../../../../../principal-component-analysis.md) of their [covariance matrix](../../../../../../covariance-matrix.md). With `cor=F`, it does not first standardize the variables to variance one. For a unit [principal component loading](../../../../../../principal-component-loading.md) vector $q$, the score $q^T(z_i-\bar z)$ has [sample variance](../../../../../../sample-variance.md) $q^T\widehat\Sigma q$. By the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md), expand $q$ in an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md); that [variance](../../../../../../variance-split.md) is a weighted average of the [eigenvalues](../../../../../../eigenvalue.md). Its maximum is the largest [eigenvalue](../../../../../../eigenvalue.md), reached at the corresponding [eigenvector](../../../../../../eigenvector.md). Repeating subject to [orthogonality](../../../../../../orthogonal-vectors.md) to previous directions gives the other [principal components](../../../../../../principal-component.md).

The software uses the divisor-$31$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md) for its component standard deviations, whereas `var` used divisor $30$. Diagonalizing the displayed matrix gives approximately

$$
\lambda(\widehat\Sigma)=(0.3323932,\ 0.00552536,\ 0.000970632),
\qquad
\lambda(S_{31})=\frac{30}{31}\lambda(\widehat\Sigma).
$$

Taking square roots of the latter gives $(0.5671603,0.07312405,0.03064834)$, agreeing with the output to the rounding of the displayed [sample covariance matrix](../../../../../../sample-covariance-matrix.md). The normalization changes these numerical standard deviations but leaves the [eigenvectors](../../../../../../eigenvector.md) and proportions of [explained variance of a principal component](../../../../../../explained-variance-of-a-principal-component.md) unchanged.

The first [principal component](../../../../../../principal-component.md) explains **about $98.08\%$ of the total log-variable variance**, the second another $1.63\%$, and the last about $0.286\%$. Keeping two preserves about $99.714\%$. An original [scree plot](../../../../../../scree-plot.md) displays the sharp drop after the first component:

<a id="3/ii/image-principal-component-variances-and-cumulative-explained-variance-for-the-log-tree-measurements"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42-pca-scree.png)

**[Figure 2](#3/ii/image-principal-component-variances-and-cumulative-explained-variance-for-the-log-tree-measurements). Principal-component variances and cumulative explained variance for the log-tree measurements**.

Consequently the centered cloud is very elongated along one direction: a one-dimensional approximation represents almost all of its squared variation. From the displayed [covariance matrix](../../../../../../covariance-matrix.md), a unit first [eigenvector](../../../../../../eigenvector.md), with its arbitrary sign chosen positive, is approximately

$$
q_1=(0.3980,\ 0.09514,\ 0.9124)^T.
$$

Its [principal component score](../../../../../../principal-component-score.md) is therefore $0.3980(\log G_i-\overline{\log G})+0.09514(\log H_i-\overline{\log H})+0.9124(\log V_i-\overline{\log V})$. All coefficients have the same sign, so this direction describes overall tree size, with log volume dominating the unstandardized variation. The summary alone supplies proportions, not the loading directions; the displayed [sample covariance matrix](../../../../../../sample-covariance-matrix.md) supplies the latter. This is a geometric approximation, not evidence of an exact deterministic relation or independent original variables.

One further use is [principal component analysis on a correlation matrix](../../../../../../principal-component-analysis-on-a-correlation-matrix.md), obtained with `cor=T`, which equalizes marginal variances and answers a different scaling-sensitive question. Another is [principal component regression](../../../../../../principal-component-regression.md): fit a response to selected [principal component scores](../../../../../../principal-component-score.md) rather than highly correlated original predictors, choosing the number using prediction assessment. The fitted transformation also projects new measurements into the same low-dimensional coordinates, provided the training centering and scaling are retained.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
