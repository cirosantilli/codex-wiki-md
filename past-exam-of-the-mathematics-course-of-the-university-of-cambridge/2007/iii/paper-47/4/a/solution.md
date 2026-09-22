<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For rows $x_i,x_j$, three useful choices are [Euclidean distance](../../../../../../euclidean-distance.md), [standardized Euclidean distance](../../../../../../standardized-euclidean-distance.md), and [Mahalanobis distance](../../../../../../mahalanobis-distance.md):

$$
d_E(i,j)=\sqrt{\sum_{r=1}^p(x_{ir}-x_{jr})^2},\qquad
d_S(i,j)=\sqrt{\sum_{r=1}^p\frac{(x_{ir}-x_{jr})^2}{s_r^2}},\qquad
d_M(i,j)=\sqrt{(x_i-x_j)^TS^{-1}(x_i-x_j)}.
$$

The Euclidean choice is simple, rotation invariant and appropriate when the original coordinate scales carry comparable meaning. It is sensitive to scale changes, may be dominated by a high-variance variable and gives correlated or duplicate variables repeated influence. Squared Euclidean dissimilarity is sometimes used algorithmically, but removing the square root generally loses the [triangle inequality](../../../../../../triangle-inequality.md).

The standardized Euclidean choice removes marginal units using fixed positive sample scales $s_r$. It gives equal marginal weight to variables, but ignores correlations and can magnify noise when an estimated [variance](../../../../../../variance-split.md) is small. Constant variables require omission or an explicitly chosen positive external scale.

The Mahalanobis choice incorporates the full [positive-definite](../../../../../../positive-definite-bilinear-form.md) sample covariance $S$, so it is [Euclidean distance](../../../../../../euclidean-distance.md) after whitening. It accounts for both scale and redundancy and is invariant under an invertible change of coordinates when $S$ is transformed consistently. However estimating $S$ requires enough observations and can be sensitive to extreme values; inversion is unstable near singularity and unavailable when $S$ is singular. With fixed positive scales or [positive-definite](../../../../../../positive-definite-bilinear-form.md) $S$, all three square-root expressions are genuine [metrics](../../../../../../metric.md) on the measurement space. Their different geometries encode different notions of which individuals should be considered similar.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
