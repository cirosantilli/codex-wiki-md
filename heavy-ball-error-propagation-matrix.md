# Heavy-ball error propagation matrix

↑ **Parent:** [Heavy-ball method](heavy-ball-method.md)

For $e_k=x^*-x_k$,

$$
\binom{e_{k+1}}{e_k}
=
\begin{pmatrix}
(1+\beta)I-\alpha A&-\beta I\\
I&0
\end{pmatrix}
\binom{e_k}{e_{k-1}}.
$$

If $A$ is diagonal with entries $\lambda_i$, a coordinate permutation turns this matrix into blocks

$$
\begin{pmatrix}1+\beta-\alpha\lambda_i&-\beta\\1&0\end{pmatrix}.
$$

**Table of contents**

- [Heavy-ball rate for a two-eigenvalue diagonal quadratic](heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic.md)

## ↑ Ancestors (7)

1. [Heavy-ball method](heavy-ball-method.md)
2. [Gradient descent](gradient-descent.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/40c/c/solution.md)
