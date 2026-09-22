<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [empirical spectral measures](../../../../../../empirical-spectral-measure.md) of the two real [symmetric matrices](../../../../../../symmetric-matrix.md) are

$$
L_N=\frac1N\sum_{i=1}^N\delta_{\lambda_i},\qquad \widehat L_N=\frac1N\sum_{i=1}^N\delta_{\widehat\lambda_i},
$$

where $\delta_t$ is the [Dirac measure](../../../../../../dirac-measure.md) at $t$. Thus $\langle L_N,f\rangle=N^{-1}\sum_i f(\lambda_i)$. Pair the [eigenvalues](../../../../../../eigenvalue.md) in the specified increasing order and apply the [triangle inequality](../../../../../../triangle-inequality.md) followed by [Lipschitz continuity](../../../../../../lipschitz-continuity.md) with bound $1$:

$$
\boxed{\left|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle\right|\leq\frac1N\sum_{i=1}^N|f(\lambda_i)-f(\widehat\lambda_i)|\leq\frac1N\sum_{i=1}^N|\lambda_i-\widehat\lambda_i|.}
$$

This deterministic estimate uses only the [Lipschitz bound](../../../../../../lipschitz-bound.md); no entry independence or distributional hypothesis is needed here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
