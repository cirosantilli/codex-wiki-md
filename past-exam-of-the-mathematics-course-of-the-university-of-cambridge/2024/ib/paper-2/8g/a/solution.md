<h1 id="8g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The characteristic [polynomial](../../../../../../polynomial-split.md) is

$$
\chi_A(t)=\det(tI-A).
$$

To prove triangularizability, use induction on $n$. The result is immediate for $n=1$. Over $\mathbb C$, $\chi_A$ has a root $\lambda$, so $A$ has an [eigenvector](../../../../../../eigenvector.md) $v_1$. Extend it to a [basis](../../../../../../basis.md). In this [basis](../../../../../../basis.md),

$$
[A]=\begin{pmatrix}\lambda&*\\0&B\end{pmatrix}.
$$

By induction, a change among the remaining $n-1$ [basis](../../../../../../basis.md) [vectors](../../../../../../vector.md) makes $B$ upper triangular. Thus the [triangularization over an algebraically closed field](../../../../../../triangularization-over-an-algebraically-closed-field.md) gives

$$
\boxed{A\text{ is similar to an upper-triangular matrix}}.
$$

The minimal [polynomial](../../../../../../polynomial-split.md) $m_A$ is the monic [polynomial](../../../../../../polynomial-split.md) of least degree satisfying $m_A(A)=0$. To establish existence without quoting the Cayley-Hamilton theorem, let $T$ be an upper-triangular [matrix](../../../../../../matrix.md) similar to $A$, with diagonal entries $\lambda_1,\ldots,\lambda_n$, and put

$$
V_k=\operatorname{span}\{e_1,\ldots,e_k\}.
$$

Then

$$
(T-\lambda_kI)V_k\subseteq V_{k-1}.
$$

The factors $T-\lambda_kI$ commute, so applying all of them successively lowers the invariant flag to zero:

$$
\prod_{k=1}^n(T-\lambda_kI)=0.
$$

Similarity gives the same [polynomial](../../../../../../polynomial-split.md) identity for $A$. Hence a nonzero monic annihilating [polynomial](../../../../../../polynomial-split.md) of degree $n$ exists, and a least-degree one exists.

If $m$ and $\widetilde m$ were two monic annihilating [polynomials](../../../../../../polynomial-split.md) of the same least degree, then $m-\widetilde m$ would be an annihilating [polynomial](../../../../../../polynomial-split.md) of smaller degree unless it were zero. Thus the minimal [polynomial](../../../../../../polynomial-split.md) is unique, and the [minimal polynomial bound from a triangular invariant flag](../../../../../../minimal-polynomial-bound-from-a-triangular-invariant-flag.md) gives

$$
\boxed{\deg m_A\leq n}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8G](../../8g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
