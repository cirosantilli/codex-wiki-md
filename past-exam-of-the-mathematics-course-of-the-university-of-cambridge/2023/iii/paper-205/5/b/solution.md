<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $j\in A$ and write

$$
R=\lambda I+X_{A\setminus\{j\}}X_{A\setminus\{j\}}^T,
\qquad a=X_j^TR^{-1}X_j\geq0.
$$

The matrix $R$ is [positive definite](../../../../../../positive-definite-matrix.md). Applying the [Sherman–Morrison formula](../../../../../../sherman-morrison-formula.md) to $R+X_jX_j^T$ yields

$$
\boxed{X_j^T(X_AX_A^T+\lambda I)^{-1}X_j
=a-\frac{a^2}{1+a}=\frac a{1+a}<1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
