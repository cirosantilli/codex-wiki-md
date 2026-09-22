<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define

$$
\left(\sum_i a_iX^i\right)\left(\sum_jm_jX^j\right)
=\sum_n\left(\sum_{i+j=n}a_im_j\right)X^n.
$$

This makes $M[X]$ an $R[X]$-module.

Let $N\subseteq M[X]$ be an $R[X]$-submodule. For $n\geq0$, let $L_n\subseteq M$ consist of zero and the leading coefficients of elements of $N$ of degree $n$. Each $L_n$ is an $R$-submodule, and multiplication by $X$ gives

$$
L_0\subseteq L_1\subseteq\cdots.
$$

Because $M$ is Noetherian, this chain stabilizes at some $n_0$, and each $L_n$ for $n\leq n_0$ is finitely generated. Choose finitely many polynomials $f_{nj}\in N$ of degree $n$ whose leading coefficients generate $L_n$.

For $f\in N$ of degree $d$, if $d\leq n_0$, subtract an $R$-linear combination of the $f_{dj}$ to lower its degree. If $d>n_0$, use $L_d=L_{n_0}$ and subtract a combination of $X^{d-n_0}f_{n_0j}$. Induction on degree expresses $f$ in terms of the finite collection $\{f_{nj}\}$. Therefore every submodule $N$ is finitely generated and

$$
\boxed{M[X]\text{ is a Noetherian }R[X]\text{-module}.}
$$

This is the module form of the [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
