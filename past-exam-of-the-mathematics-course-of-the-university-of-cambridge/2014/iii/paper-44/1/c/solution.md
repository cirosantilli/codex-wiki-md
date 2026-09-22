<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The off-diagonal auxiliary integrations impose $M^i{}_j=0$ for $i\ne j$, by the Fourier representation of a [Dirac delta function](../../../../../../dirac-delta-function.md). After this constraint, $M=\operatorname{diag}(\lambda_1,\ldots,\lambda_N)$ and

$$
[M,C]^i{}_j=(\lambda_i-\lambda_j)C^i{}_j,\qquad
\operatorname{tr}(B[M,C])=\sum_{i\ne j}B^j{}_i(\lambda_i-\lambda_j)C^i{}_j.
$$

The [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) over each off-diagonal pair gives its coefficient. Consequently the ghost determinant is

$$
\det{}'\operatorname{ad}_M=\prod_{i\ne j}(\lambda_i-\lambda_j)
=(-1)^{N(N-1)/2}\prod_{i<j}(\lambda_i-\lambda_j)^2.
$$

The prime omits the diagonal directions, which were excluded from the outset. The constant sign depends on the [Berezin integral](../../../../../../berezin-integral.md) ordering and can be absorbed in normalization. Thus the [Vandermonde determinant](../../../../../../vandermonde-determinant.md) squared is the eigenvalue measure factor in this [matrix diagonalization ghost determinant](../../../../../../matrix-diagonalization-ghost-determinant.md).

Up to an eigenvalue-independent constant, the remaining integral is $\int\prod_i d\lambda_i\,e^{-S_{\rm eig}}$, where

$$
\boxed{S_{\rm eig}=N\sum_i\left(\frac{\lambda_i^2}{2}+\frac g4\lambda_i^4\right)
-2\sum_{i<j}\log|\lambda_i-\lambda_j|.}
$$

**The determinant supplies logarithmic eigenvalue repulsion**. An ordering restriction on the [eigenvalues](../../../../../../eigenvalue.md) changes only a constant factorial; no remaining eigenvalue integral needs to be performed. The off-diagonal bosonic contours and the displayed normalization are understood in the usual Fourier-delta prescription.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
