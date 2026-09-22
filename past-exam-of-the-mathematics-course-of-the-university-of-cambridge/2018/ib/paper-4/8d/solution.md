<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

[Gaussian elimination](../../../../../gaussian-elimination.md) without pivoting gives

$$
A=LU,
\quad
L=\begin{pmatrix}1&0&0&0\\2&1&0&0\\1&3&1&0\\2&2&2&1\end{pmatrix},
\quad
U=\begin{pmatrix}1&2&1&2\\0&1&3&2\\0&0&3&6\\0&0&0&\lambda-20\end{pmatrix}.
$$

Thus $\det A=3(\lambda-20)$ and the solution is unique exactly when **$\lambda\ne20$**.

For $\lambda=20$, [forward substitution in a triangular system](../../../../../forward-substitution-in-a-triangular-system.md) in $Ly=b$ gives $y=(1,1,3,\mu-10)^T$. Consistency of $Ux=y$ requires $\boxed{\mu=10}$. [backward substitution in a triangular system](../../../../../backward-substitution-in-a-triangular-system.md) then gives

$$
\boxed{x=(4-8t,\ 4t-2,\ 1-2t,\ t)^T,\qquad t\in\mathbb R.}
$$

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
