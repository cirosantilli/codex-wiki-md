<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\widehat\theta_{\mathrm{MLE}}=\overline X.
$$

Under the score-outer-product convention stated in the question,

$$
\widehat i_n
=\frac1n\sum_{j=1}^n
(X_j-\overline X)(X_j-\overline X)^T.
$$

This is the sample covariance matrix with divisor $n$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md), applied entrywise, gives

$$
\boxed{\widehat i_n\longrightarrow I_p\quad\text{almost surely}.}
$$

Thus the [empirical score outer-product information](../../../../../../empirical-score-outer-product-information.md) consistently estimates the per-observation Fisher information.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
