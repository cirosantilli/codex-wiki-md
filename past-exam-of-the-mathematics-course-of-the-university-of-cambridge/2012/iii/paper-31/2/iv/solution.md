<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $D=|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle|$. Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to the average of the nonnegative [eigenvalue](../../../../../../eigenvalue.md) differences, and then the [Hoffman–Wielandt inequality](../../../../../../hoffman-wielandt-inequality.md):

$$
D^2\leq\left(\frac1N\sum_i|\lambda_i-\widehat\lambda_i|\right)^2\leq\frac1N\sum_i|\lambda_i-\widehat\lambda_i|^2\leq\frac1N\operatorname{Tr}[(X_N-\widehat X_N)^2].
$$

Taking nonnegative square roots gives the [spectral Lipschitz bound from Frobenius distance](../../../../../../spectral-lipschitz-bound-from-frobenius-distance.md)

$$
\boxed{D\leq\left(\frac1N\operatorname{Tr}[(X_N-\widehat X_N)^2]\right)^{1/2}=\frac{\|X_N-\widehat X_N\|_F}{\sqrt N}.}
$$

The factor $N^{-1/2}$ is essential: the [empirical spectral measure](../../../../../../empirical-spectral-measure.md) has total mass $1$, not $N$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
