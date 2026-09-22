<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A matrix is in [Jordan normal form](../../../../../jordan-normal-form.md) if it is block diagonal with [Jordan blocks](../../../../../jordan-block.md) $J_r(\lambda)=\lambda I+N$, where $N$ has ones immediately above the diagonal and zeros elsewhere. For a [Jordan normal form](../../../../../jordan-normal-form.md) matrix $J$, number its diagonal positions $1,\ldots,n$ and put

$$
J_m=J+\varepsilon_m\operatorname{diag}(1,\ldots,n).
$$

Choose positive $\varepsilon_m\to0$ avoiding the finitely many values solving $\lambda_i+i\varepsilon=\lambda_j+j\varepsilon$ for $i\ne j$. The matrix remains upper triangular and now has distinct [eigenvalues](../../../../../eigenvalue.md), so it is [diagonalizable](../../../../../diagonalizable-matrix.md). Its entries converge to those of $J$. For arbitrary $A=SJS^{-1}$, use $A_m=SJ_mS^{-1}$. This proves [density of diagonalizable complex matrices](../../../../../density-of-diagonalizable-complex-matrices.md).

If $A$ is diagonalizable with [eigenvalues](../../../../../eigenvalue.md) $\lambda_1,\lambda_2$, conjugating $B$ by the same basis change conjugates $T_A$ to $T_{\operatorname{diag}(\lambda_1,\lambda_2)}$. On the four matrix units $E_{ij}$, this acts by $(\lambda_i+\lambda_j)E_{ij}$. Thus, writing $s=\operatorname{tr}A$ and $d=\det A$, its [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\begin{aligned}
\chi_{T_A}(t)&=(t-2\lambda_1)(t-2\lambda_2)(t-\lambda_1-\lambda_2)^2\\
&=\boxed{(t-s)^2(t^2-2st+4d)}.
\end{aligned}
$$

The entries of $T_A$ depend linearly on those of $A$, and the coefficients of its [characteristic polynomial](../../../../../characteristic-polynomial.md) depend polynomially, hence continuously, on those entries. Apply the formula to the approximating $A_m$ and pass to the limit. The boxed formula therefore holds for every $A$, including non-diagonalizable matrices. This is the [two-by-two anticommutator characteristic polynomial](../../../../../two-by-two-anticommutator-characteristic-polynomial.md).

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
