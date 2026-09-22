<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $B=A_1^TA_1$. It is a [symmetric matrix](../../../../../symmetric-matrix.md) and a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), while $A_2^TA_2=I_n-B$ is also a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md). By the [spectral theorem](../../../../../spectral-theorem.md), choose an [orthogonal matrix](../../../../../orthogonal-matrix.md) $V=[v_1,\ldots,v_n]$ such that

$$
V^TBV=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),\qquad 0\leq\lambda_j\leq1.
$$

The bounds follow directly from $z^TBz=\|A_1z\|_2^2\in[0,\|z\|_2^2]$. Define the [diagonal matrices](../../../../../diagonal-matrix.md)

$$
\Sigma_1=\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n}),\qquad
\Sigma_2=\operatorname{diag}(\sqrt{1-\lambda_1},\ldots,\sqrt{1-\lambda_n}).
$$

The columns of $A_1V$ are mutually [orthogonal](../../../../../orthogonal-vectors.md), since $(A_1v_i)^T(A_1v_j)=\lambda_j\delta_{ij}$. For each $\lambda_j>0$, set $u_{1j}=A_1v_j/\sqrt{\lambda_j}$. These columns are [orthonormal](../../../../../orthonormal-set.md). At a zero $\lambda_j$, one has $A_1v_j=0$; choose $u_{1j}$ by completing the already prescribed columns to an [orthonormal set](../../../../../orthonormal-set.md) of $n$ columns in $\mathbb R^k$. Such a completion exists because $k\geq n$. This gives $A_1V=U_1\Sigma_1$, including the zero columns.

Likewise, the [Gram matrix](../../../../../gram-matrix.md) of $A_2V$ is $\operatorname{diag}(1-\lambda_j)$. Normalize its nonzero columns and complete at its zero columns in $\mathbb R^{m-k}$, using $m-k\geq n$. The resulting $U_2$ has [orthonormal](../../../../../orthonormal-set.md) columns and $A_2V=U_2\Sigma_2$. Combining the identities gives

$$
\boxed{A=\begin{pmatrix}U_1&0\\0&U_2\end{pmatrix}
\begin{pmatrix}\Sigma_1\\\Sigma_2\end{pmatrix}V^T}.
$$

This is a form of the [cosine-sine decomposition](../../../../../cosine-sine-decomposition.md). Completing the zero columns is essential: neither block was assumed to have [full column rank](../../../../../full-column-rank.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
