<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [orthogonal diagonalization of a real symmetric matrix](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md), write $A=Q\operatorname{diag}(\lambda_1,\ldots,\lambda_d)Q^T$, with orthogonal $Q$. Its [matrix exponential](../../../../../../matrix-exponential.md) has the same eigenvectors and positive [eigenvalues](../../../../../../eigenvalue.md) $e^{t\lambda_j}$. Orthogonal invariance of the induced [Euclidean norm](../../../../../../euclidean-norm.md) gives the exact identity

$$
\boxed{\|e^{tA}\|_2=\max_j e^{t\lambda_j}
=e^{t\lambda_{\max}(A)},\qquad t\geq0.}
$$

This proves the requested inequality with equality. If a real number $\beta$ gave the bound for every $t\geq0$, evaluating on a unit eigenvector for $\lambda_{\max}(A)$ at any $t>0$ would give $e^{t\lambda_{\max}}\leq e^{t\beta}$, so $\beta\geq\lambda_{\max}$. Thus **the stated exponent is the smallest possible**. For a [symmetric matrix](../../../../../../symmetric-matrix.md) the [spectral abscissa](../../../../../../spectral-abscissa.md) and [Euclidean logarithmic norm](../../../../../../euclidean-logarithmic-norm.md) coincide, unlike the general nonsymmetric case in Question 1.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
