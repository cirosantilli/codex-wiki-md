<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the mutually orthogonal eigenvectors so that $(x_j)$ is an [orthonormal sequence](../../../../../../orthonormal-sequence.md). If $\lambda_j$ did not tend to zero, some subsequence would satisfy $|\lambda_j|\geq\varepsilon>0$. For distinct indices in this subsequence, orthogonality gives

$$
\lVert Tx_j-Tx_k\rVert^2
=\lVert\lambda_jx_j-\lambda_kx_k\rVert^2
=|\lambda_j|^2+|\lambda_k|^2
\geq2\varepsilon^2.
$$

Thus $(Tx_j)$ would have no Cauchy subsequence, contradicting compactness of $T$. Therefore the [orthogonal eigenvectors of a compact operator](../../../../../../orthogonal-eigenvectors-of-a-compact-operator.md) satisfy

$$
\boxed{\lambda_j\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22F](../../22f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
