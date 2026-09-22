<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Gaussian elimination](../../../../gaussian-elimination.md) uses [elementary row operations](../../../../elementary-row-operation.md) to remove entries below successive [pivot elements](../../../../pivot-element.md), reducing a [linear system](../../../../system-of-linear-equations.md) to one with an [upper triangular matrix](../../../../upper-triangular-matrix.md). [Back substitution](../../../../back-substitution.md) then solves that system. It also computes a reusable [matrix factorization](../../../../matrix-decomposition.md), so additional right-hand sides can be handled by [forward substitution](../../../../forward-substitution.md) and [back substitution](../../../../back-substitution.md) without repeating the elimination.

For elimination without row exchanges, let $A^{(1)}=A$. At step $k$, provided the [pivot element](../../../../pivot-element.md) $a_{kk}^{(k)}$ is nonzero, form the [elimination multipliers](../../../../elimination-multiplier.md)

$$
m_{ik}=\frac{a_{ik}^{(k)}}{a_{kk}^{(k)}},\qquad i=k+1,\ldots,n,
$$

and perform $\text{row}_i\leftarrow\text{row}_i-m_{ik}\text{row}_k$, applying the same operation to the right-hand side. More explicitly the resulting entries satisfy $a_{ij}^{(k+1)}=a_{ij}^{(k)}-m_{ik}a_{kj}^{(k)}$ for $i>k$, $j\geq k$.

Let $E_k=I-\sum_{i>k}m_{ik}e_i e_k^T$, where $e_i$ are the [standard basis](../../../../standard-basis.md) [vectors](../../../../vector.md). Then

$$
U=E_{n-1}\cdots E_1A,\qquad
A=LU,\qquad L=E_1^{-1}\cdots E_{n-1}^{-1}.
$$

The [matrix](../../../../matrix.md) $L$ is a [unit lower triangular matrix](../../../../unit-lower-triangular-matrix.md) storing the [elimination multipliers](../../../../elimination-multiplier.md), while $U$ is an [upper triangular matrix](../../../../upper-triangular-matrix.md):

$$
L=\begin{pmatrix}
1&0&\cdots&0\\
m_{21}&1&\cdots&0\\
\vdots&\vdots&\ddots&\vdots\\
m_{n1}&m_{n2}&\cdots&1
\end{pmatrix},\qquad
U=\begin{pmatrix}
u_{11}&u_{12}&\cdots&u_{1n}\\
0&u_{22}&\cdots&u_{2n}\\
\vdots&\vdots&\ddots&\vdots\\
0&0&\cdots&u_{nn}
\end{pmatrix}.
$$

Solving $Ax=b$ becomes $Ly=b$ followed by $Ux=y$. If a required [pivot element](../../../../pivot-element.md) vanishes, an unpermuted [LU decomposition](../../../../lu-decomposition.md) can fail even for an [invertible matrix](../../../../invertible-matrix.md). Row exchanges, typically selected by [partial pivoting](../../../../columnwise-partial-pivoting.md), instead produce $PA=LU$ with a [permutation matrix](../../../../permutation-matrix.md) $P$; then solve $Ly=Pb$, $Ux=y$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
