<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

The [linear least-squares problem](../../../../../linear-least-squares-problem.md) is to choose $x\in\mathbb R^n$ minimizing the [Euclidean norm](../../../../../euclidean-norm.md) of the residual:

$$
\boxed{\min_x\|Ax-b\|_2}.
$$

For a [QR decomposition](../../../../../qr-decomposition.md) $A=QR$, orthogonality of $Q$ gives $\|Ax-b\|_2=\|Rx-Q^Tb\|_2$. If $A$ has full column rank and $R=\binom{R_1}{0}$ is in standard form with invertible upper-triangular $R_1\in\mathbb R^{n\times n}$, the minimizer solves $R_1x=(Q^Tb)_{1:n}$.

Applying the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to the columns of the given matrix yields

$$
Q=\frac12\begin{pmatrix}
1&1&1&1\\
1&-1&1&-1\\
1&1&-1&-1\\
1&-1&-1&1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
2&1&1\\
0&1&0\\
0&0&1\\
0&0&0
\end{pmatrix}.
$$

Indeed, $Q$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) and $A=QR$. Moreover,

$$
Q^Tb=(6,-2,-3,1)^T.
$$

Back substitution in the leading triangular system gives

$$
x_2=-2,
\qquad x_3=-3,
\qquad 2x_1+x_2+x_3=6,
$$

so the unique least-squares solution is

$$
\boxed{x=(11/2,-2,-3)^T}.
$$

The unused final transformed residual component is $1$, so the minimum residual norm is $1$.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
