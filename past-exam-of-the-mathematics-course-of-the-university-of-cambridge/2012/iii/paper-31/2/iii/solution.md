<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Hoffman–Wielandt inequality](../../../../../../hoffman-wielandt-inequality.md) says that for [normal matrices](../../../../../../normal-matrix.md) $A,B$ with [eigenvalues](../../../../../../eigenvalue.md) $\alpha_i,\beta_i$, there is a [permutation](../../../../../../permutation.md) $\pi$ such that

$$
\sum_{i=1}^N|\alpha_i-\beta_{\pi(i)}|^2\leq\|A-B\|_F^2=\operatorname{Tr}[(A-B)^*(A-B)],
$$

where $\|\cdot\|_F$ is the [Frobenius norm](../../../../../../frobenius-norm.md) and $*$ denotes the [conjugate transpose](../../../../../../conjugate-transpose.md). For [Hermitian matrices](../../../../../../hermitian-operator.md), the increasingly ordered real [eigenvalues](../../../../../../eigenvalue.md) may be paired directly: this ordering minimizes the sum of squared distances over all [permutations](../../../../../../permutation.md), by removing crossed pairs. In particular, for the real [symmetric matrices](../../../../../../symmetric-matrix.md) in this question,

$$
\boxed{\sum_{i=1}^N|\lambda_i-\widehat\lambda_i|^2\leq\operatorname{Tr}[(X_N-\widehat X_N)^2].}
$$

The square on the right is justified by symmetry. For arbitrary [matrices](../../../../../../matrix.md), the appropriate expression is the conjugate-transpose product, not the ordinary square.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
