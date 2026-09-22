<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The calculation is [principal component analysis on a correlation matrix](../../../../../principal-component-analysis-on-a-correlation-matrix.md), rather than on an unscaled [covariance matrix](../../../../../covariance-matrix.md). For each of the eleven rating variables, subtract its column mean and divide by its column [standard deviation](../../../../../standard-deviation.md). If $Z$ is the resulting $43\times11$ [matrix](../../../../../matrix.md), use the divisor convention of the fitted object to write

$$
R=\frac1{43}Z^TZ,
\qquad R a_k=\lambda_k a_k,
\qquad a_k^Ta_\ell=\delta_{k\ell},
\qquad\lambda_1\ge\cdots\ge\lambda_{11}\ge0.
$$

Here the scaling [standard deviations](../../../../../standard-deviation.md) use divisor $43$, consistently with this convention. Using sample [standard deviations](../../../../../standard-deviation.md) with divisor $42$ gives the same [correlation matrix](../../../../../correlation-matrix.md) and directions, with the corresponding score scale. Every diagonal entry of $R$ is one, so $\sum_k\lambda_k=\operatorname{tr}R=11$.

A [principal component](../../../../../principal-component.md) is the [linear combination](../../../../../linear-combination.md) of the standardized ratings along $a_k$. Its [principal component score](../../../../../principal-component-score.md) for judge $i$ is $t_{ik}=z_i^Ta_k$, and its [variance](../../../../../variance-split.md) is $\lambda_k$. The displayed component [standard deviations](../../../../../standard-deviation.md) are $\sqrt{\lambda_k}$; the [explained variance of a principal component](../../../../../explained-variance-of-a-principal-component.md) is $\lambda_k/11$. In particular,

$$
\lambda_1\simeq(3.1833029)^2\simeq10.1334,\qquad
\lambda_2\simeq(0.65163561)^2\simeq0.424629.
$$

The first component explains about $92.122\%$ of the standardized variation, and the first two jointly explain **$95.982\%$**. Components three, four and five add about $2.321\%$, $0.830\%$ and $0.339\%$. The cumulative line adds these proportions successively; it is not the proportion explained by that component alone. Retaining two components discards about $4.018\%$ of the total standardized squared variation.

The displayed [principal component loadings](../../../../../principal-component-loading.md) are the unit [eigenvector](../../../../../eigenvector.md) coefficients $a_{jk}$. The first direction has positive, broadly similar weights for all ratings. It measures an overall favorable-rating tendency: a judge high on most ratings has a high first score. The second direction compares integrity and demeanour, with large positive coefficients, against such attributes as decision promptness, case-flow management and physical ability, with negative coefficients. Thus among similarly rated judges, a positive second score indicates relatively stronger integrity/demeanour compared with those operational ratings. This is a description of a data direction, not a causal interpretation. Multiplying a whole [eigenvector](../../../../../eigenvector.md) and its scores by minus one reflects the display but changes nothing substantive.

These [principal component loadings](../../../../../principal-component-loading.md) are not themselves variable-component correlations. With standardized variables,

$$
\operatorname{Cov}(Z_j,a_k^TZ)=\lambda_k a_{jk},
\qquad\operatorname{Corr}(Z_j,a_k^TZ)=\sqrt{\lambda_k}\,a_{jk}.
$$

For example, the integrity correlation with component one is approximately $3.1833\times0.289\simeq0.920$. Blank loadings in the printed second column indicate suppressed small entries, not exact zeros. The complete unrounded loading vectors in the fitted object must be used to calculate scores.

A two-dimensional representation plots the 43 pairs

$$
\boxed{(t_{i1},t_{i2})=(z_i^Ta_1,z_i^Ta_2),\qquad i=1,\ldots,43,}
$$

with each point labeled by its judge. In the fitted software object these are the first two columns of the score [matrix](../../../../../matrix.md). Nearby points have similar projections of their standardized ratings. The rank-two reconstruction $\widehat z_i=t_{i1}a_1+t_{i2}a_2$ is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the leading principal plane and minimizes the total squared reconstruction error over all two-dimensional linear subspaces. To see this, for any orthonormal pair of directions the captured [variance](../../../../../variance-split.md) is the sum of its two Rayleigh quotients, at most $\lambda_1+\lambda_2$ by diagonalizing $R$; the remaining [variance](../../../../../variance-split.md) is the total minus that captured sum. Distances in the plot omit the smaller components, so a close projected pair need not be equally close in every original rating. The actual 43 coordinates cannot be recovered from the summary alone; the supplied data [matrix](../../../../../matrix.md) or fitted score [matrix](../../../../../matrix.md) is needed.

The printed descriptive list omits INTG, although the loading table includes it. INTG denotes integrity and supplies the eleventh variable. The standard data set also contains a contacts variable; the stated eleven-rating analysis uses the ratings, not contacts.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
