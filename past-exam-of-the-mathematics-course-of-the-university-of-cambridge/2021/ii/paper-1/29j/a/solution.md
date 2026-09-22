<h1 id="29j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
\ell_n(\theta)=\log f_\theta(X_1,\ldots,X_n)
$$

be the [log-likelihood](../../../../../../log-likelihood.md). The [score function](../../../../../../informant-function.md) and scalar [Fisher information](../../../../../../fisher-information-matrix.md) are

$$
S_n(\theta)=\frac{\partial}{\partial\theta}\ell_n(\theta),
\qquad
\boxed{I_n(\theta)=\mathbb E_\theta[S_n(\theta)^2]}.
$$

Under the usual regularity conditions the score has mean zero, so this is also its [variance](../../../../../../variance-split.md).

The information tensorizes when it is additive over observations. For identically distributed observations,

$$
\boxed{I_n(\theta)=nI_1(\theta)}.
$$

For an independent sample the joint score is the sum of the individual scores, and the [mean-zero score identity](../../../../../../mean-zero-score-identity.md) makes all cross covariances vanish. This is the [Tensorization of Fisher information](../../../../../../tensorization-of-fisher-information.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
