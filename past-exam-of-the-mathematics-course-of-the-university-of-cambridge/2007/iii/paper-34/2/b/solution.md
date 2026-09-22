<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the spectral decomposition of the one-qubit [density operator](../../../../../../density-matrix.md) as $\pi=\sum_{j=0}^1\lambda_j|e_j\rangle\langle e_j|$. For a word $\mathbf j=(j_1,\ldots,j_n)$, the [tensor product](../../../../../../tensor-product.md) vector

$$
|e_{\mathbf j}\rangle=|e_{j_1}\rangle\otimes\cdots\otimes|e_{j_n}\rangle
$$

is an eigenvector of $\pi^{\otimes n}$, with eigenvalue

$$
\boxed{\lambda_{\mathbf j}=\lambda_{j_1}\cdots\lambda_{j_n}.}
$$

These product vectors form an orthonormal [eigenbasis](../../../../../../eigenbasis.md), allowing arbitrary orthonormal choices within degeneracies. Using $\sum_j\lambda_j=1$ and $0\log0=0$,

$$
\begin{aligned}
S(\pi^{\otimes n})
&=-\sum_{j_1,\ldots,j_n}\left(\prod_{s=1}^n\lambda_{j_s}\right)\sum_{s=1}^n\log_2\lambda_{j_s}\\
&=n\left(-\sum_j\lambda_j\log_2\lambda_j\right).
\end{aligned}
$$

Thus the [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is

$$
\boxed{S(\rho^{(n)})=nS(\pi).}
$$

This calculation uses the spectral ensemble of the [memoryless quantum information source](../../../../../../memoryless-quantum-information-source.md); the originally emitted vectors need not equal these eigenvectors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
