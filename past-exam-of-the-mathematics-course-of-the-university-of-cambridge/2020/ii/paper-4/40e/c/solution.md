<h1 id="40e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the only nonzero coefficients of $a$ are

$$
\widehat a_{0,0}=5,
\qquad
\widehat a_{1,0}=\widehat a_{-1,0}
=\widehat a_{0,1}=\widehat a_{0,-1}=1.
$$

Therefore, for each $(m,n)\in\Lambda_N$, the truncated system is

$$
\begin{aligned}
\pi^2\{&5(m^2+n^2)\widehat u_{m,n}
+[m(m-1)+n^2]\widehat u_{m-1,n}\\
&+[m(m+1)+n^2]\widehat u_{m+1,n}
+[m^2+n(n-1)]\widehat u_{m,n-1}\\
&+[m^2+n(n+1)]\widehat u_{m,n+1}\}
=-\widehat f_{m,n},
\end{aligned}
$$

where a coefficient is omitted when its index is outside $\Lambda_N$ or equals $(0,0)$.

For wavevectors $\mathbf k=(m,n)$ and $\boldsymbol\ell=(p,q)$, the matrix entry is

$$
A_{\mathbf k,\boldsymbol\ell}
=\pi^2(\mathbf k\mathbin\cdot\boldsymbol\ell)\widehat a_{\mathbf k-\boldsymbol\ell}.
$$

Because $\widehat a_{\mathbf r}=\widehat a_{-\mathbf r}$, $A_{\mathbf k,\boldsymbol\ell}=A_{\boldsymbol\ell,\mathbf k}$, so the matrix is [symmetric](../../../../../../symmetric-matrix.md). Its diagonal entry is $5\pi^2|\mathbf k|^2$. The sum of absolute off-diagonal entries is at most

$$
\pi^2\sum_{j=1}^2\left(
|\mathbf k|^2+k_j+|\mathbf k|^2-k_j\right)
=4\pi^2|\mathbf k|^2,
$$

because $|\mathbf k|^2\pm k_j\geq0$ for nonzero integer $\mathbf k$; truncation can only reduce the sum. Hence $A$ is [strictly diagonally dominant](../../../../../../strictly-diagonally-dominant-matrix.md) with positive diagonal. The [Gershgorin circle theorem](../../../../../../gershgorin-circle-theorem.md) places every eigenvalue in the positive interval

$$
[\pi^2|\mathbf k|^2,9\pi^2|\mathbf k|^2]
$$

for at least one row. Since the symmetric matrix has only real eigenvalues, all are positive, and $A$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md). Any one-dimensional ordering merely conjugates $A$ by a [permutation matrix](../../../../../../permutation-matrix.md), preserving symmetry and positive definiteness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
