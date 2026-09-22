<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For real $\lambda_1,\lambda_2$, compute

$$
LL^T-L^TL=\begin{pmatrix}-1&\lambda_1-\lambda_2\\\lambda_1-\lambda_2&1\end{pmatrix}\ne0.
$$

Thus $L$ is a [non-normal matrix](../../../../../../non-normal-matrix.md). For distinct [eigenvalues](../../../../../../eigenvalue.md), take

$$
v_1=\begin{pmatrix}\lambda_1-\lambda_2\\1\end{pmatrix},\qquad v_2=\begin{pmatrix}0\\1\end{pmatrix}.
$$

These satisfy $Lv_j=\lambda_jv_j$ but have [inner product](../../../../../../inner-product.md) $v_1^Tv_2=1$. The [eigenvectors](../../../../../../eigenvector.md) are therefore [nonorthogonal](../../../../../../nonorthogonal-vectors.md). When the eigenvalues coincide, only the direction $v_2$ remains as an [eigenvector](../../../../../../eigenvector.md); $L$ is a defective [Jordan block](../../../../../../jordan-block.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
