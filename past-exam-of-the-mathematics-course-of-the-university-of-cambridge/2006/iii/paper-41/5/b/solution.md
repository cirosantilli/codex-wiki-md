<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $A=\sum_{i=1}^3S_{i1}$, $B=\sum_{i=1}^3S_{i2}$ and $d=\lambda_1-\lambda_2$. [Independence](../../../../../../independent-random-variables.md) of the pairs makes their likelihood contributions multiply. The three fully observed pairs contribute $(\lambda_1\lambda_2)^3e^{-\lambda_1A-\lambda_2B}$; each remaining pair contributes its [hypoexponential distribution](../../../../../../hypoexponential-distribution.md) density. Thus the observed-data [log-likelihood](../../../../../../log-likelihood.md) is

$$
\boxed{\ell(\lambda_1,\lambda_2)=8\log\lambda_1+8\log\lambda_2
-\lambda_1A-\lambda_2B-5\log d
+\sum_{j=4}^8\log(e^{-\lambda_2T_j}-e^{-\lambda_1T_j}).}
$$

An equivalent expression, convenient for calculations, is

$$
\ell=8\log\lambda_1+8\log\lambda_2-5\log d
-\lambda_1A-\lambda_2\left(B+\sum_{j=4}^8T_j\right)
+\sum_{j=4}^8\log(1-e^{-dT_j}).
$$

The apparent singularity as $d\downarrow0$ cancels between the last sum and $-5\log d$. The resulting equal-rate limit is finite for positive observed times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
