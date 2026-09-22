# Zero-pivot failure of tridiagonal elimination

↑ **Parent:** [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)

An [invertible matrix](invertible-matrix.md) need not admit the unpivoted [Thomas algorithm](tridiagonal-matrix-algorithm.md). For example,

$$
A=\begin{pmatrix}0&1\\1&1\end{pmatrix},\qquad d=\begin{pmatrix}2\\3\end{pmatrix},\qquad x=\begin{pmatrix}1\\2\end{pmatrix}.
$$

Here $\det A=-1$ and $Ax=d$, but $p_1=0$ makes $m_2=1/0$ undefined. Interchanging the two equations instead gives the upper [triangular matrix](triangular-matrix.md) system $x_1+x_2=3$, $x_2=2$, solved immediately by [back substitution](back-substitution.md). Even a nonzero first diagonal does not guarantee all later [pivot elements](pivot-element.md): $\begin{pmatrix}1&1&0\\1&1&1\\0&1&1\end{pmatrix}$ has [determinant](determinant.md) $-1$, yet $p_2=1-1=0$.

For a general [tridiagonal matrix](tridiagonal-matrix.md), use a solver with [partial pivoting](columnwise-partial-pivoting.md) when these structural guarantees are unavailable or a dangerously small [pivot element](pivot-element.md) occurs. Adjacent row interchanges can introduce a second upper diagonal, so a pivoted solver must track that additional [fill-in](fill-in.md); it cannot blindly continue the unpivoted [recurrence relations](recurrence-relation.md). LAPACK's `DGTSV` explicitly performs [partial pivoting](columnwise-partial-pivoting.md), stores this extra upper diagonal, and includes it in [back substitution](back-substitution.md). Its fixed-width storage and bounded work per row retain $O(n)$ time for one right-hand side and $O(n)$ storage.[DGTSV, Purpose lines 34–39; DL argument lines 63–69; adjacent interchange lines 188–199; back solve lines 295–305](dgtsv-lapack-3-12-1-by-lapack-project.md)

## ↑ Ancestors (6)

1. [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
