<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $K=k(z)$, where $z$ is an indeterminate, and form the [right Artinian triangular ring that is not left Noetherian](../../../../../right-artinian-triangular-ring-that-is-not-left-noetherian.md)

$$
\boxed{T=\begin{pmatrix}k&K\\0&K\end{pmatrix}.}
$$

Multiplication uses the natural $k$–$K$ bimodule structure on the upper-right entry. With the two diagonal [idempotents](../../../../../idempotent.md) $e_1,e_2$, the right regular [module](../../../../../module-mathematics.md) is $e_1T\oplus e_2T$. The off-diagonal submodule of $e_1T$ is one-dimensional over the bottom-right [field](../../../../../field.md) $K$, hence simple. Its quotient is one-dimensional over the top-left [field](../../../../../field.md) $k$, hence simple. Also $e_2T$ is a simple right [module](../../../../../module-mathematics.md) over $K$. Thus $T_T$ has a composition series of length three, and in particular $T$ is right [Artinian](../../../../../artinian-ring.md).

On the left, multiplication of an off-diagonal matrix gives

$$
\begin{pmatrix}a&m\\0&b\end{pmatrix}
\begin{pmatrix}0&u\\0&0\end{pmatrix}
=\begin{pmatrix}0&au\\0&0\end{pmatrix}.
$$

Every $k$-subspace $U\subseteq K$ therefore yields a [left ideal](../../../../../left-ideal.md) of off-diagonal matrices with entries in $U$. The subspaces $U_m=\operatorname{span}_k\{1,z,\ldots,z^m\}$ are strictly increasing because $z$ is transcendental. Their associated [left ideals](../../../../../left-ideal.md) violate the [ascending chain condition](../../../../../ascending-chain-condition.md). Hence **$T$ is not left Noetherian**, even though it is right Artinian and right Noetherian.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 85](../../paper-85-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
