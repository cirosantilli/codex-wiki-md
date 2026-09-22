<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the orientation of the [Berezin integral](../../../../../../berezin-integral.md) so that

$$
D\eta\,D\bar\eta=d\eta_N\,d\bar\eta_N\cdots d\eta_1\,d\bar\eta_1,
\qquad\int D\eta\,D\bar\eta\prod_{i=1}^N(\bar\eta_i\eta_i)=1.
$$

Here the product has increasing $i$; this explicitly fixes the otherwise convention-dependent overall sign in the compact measure notation.

Since $A$ is a [diagonalizable matrix](../../../../../../diagonalizable-matrix.md), write $A=S\Lambda S^{-1}$ with $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_N)$. Make the independent changes $\eta=S\xi$ and $\bar\eta=\bar\xi S^{-1}$. The [Grassmann change-of-variables formula](../../../../../../grassmann-change-of-variables-formula.md) gives the two factors $(\det S)^{-1}$ and $\det S$, so the complete measure is unchanged. The exponent becomes $\sum_i\lambda_i\bar\xi_i\xi_i$. Each summand is even and squares to zero, and the different even summands commute. Consequently,

$$
e^{\bar\eta A\eta}=\prod_{i=1}^N(1+\lambda_i\bar\xi_i\xi_i).
$$

Only the term containing every generator survives the [Berezin integral](../../../../../../berezin-integral.md). Hence the [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) is

$$
\boxed{\int D\eta\,D\bar\eta\,e^{\bar\eta A\eta}
=\prod_{i=1}^N\lambda_i=\det A}.
$$

Zero eigenvalues give zero on both sides, so invertibility of $A$ is unnecessary. In fact the identity extends to all ordinary matrices: the top-degree coefficient of the exponential is the alternating [determinant](../../../../../../determinant.md) expansion. The assumption that $A$ is a [diagonalizable matrix](../../../../../../diagonalizable-matrix.md) makes the proof especially transparent.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
