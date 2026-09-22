<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The Euclidean matrix [norm](../../../../../../norm.md) is the induced [operator norm](../../../../../../operator-norm.md) $\|C\|_2=\sup_{\|x\|_2=1}\|Cx\|_2$. By the [spectral theorem](../../../../../../spectral-theorem.md), a real [symmetric matrix](../../../../../../symmetric-matrix.md) has $A=Q\Lambda Q^T$ with $Q$ orthogonal and $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_m)$. Hence

$$
e^{tA}=Q\operatorname{diag}(e^{t\lambda_1},\ldots,e^{t\lambda_m})Q^T.
$$

Orthogonal transformations preserve the Euclidean [norm](../../../../../../norm.md), and the induced [norm](../../../../../../norm.md) of a real diagonal matrix is the maximum absolute diagonal entry. Therefore, for $t\geq0$,

$$
\boxed{\|e^{tA}\|_2=\max_j e^{t\lambda_j}=e^{t\mu(A)}.}
$$

This gives the requested inequality with equality. If an exponent $\beta<\mu(A)$ were to work with prefactor one for every $t$, choose a unit [eigenvector](../../../../../../eigenvector.md) for $\mu(A)$. Its image has length $e^{t\mu(A)}>e^{t\beta}$ for every $t>0$, a contradiction. Thus **$\mu(A)$ is the smallest possible exponent**.

For [symmetric matrices](../../../../../../symmetric-matrix.md) the [spectral abscissa](../../../../../../spectral-abscissa.md) equals the [Euclidean logarithmic norm](../../../../../../euclidean-logarithmic-norm.md). Symmetry is essential to this particular exact [norm](../../../../../../norm.md) formula; a general non-normal matrix can have transient growth not controlled with prefactor one by its spectral abscissa.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
