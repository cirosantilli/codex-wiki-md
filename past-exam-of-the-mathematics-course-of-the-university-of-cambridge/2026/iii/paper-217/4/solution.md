<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $e_n(t)=\sqrt2\sin(n\pi t)$, let $(g_n)$ be independent standard normal variables, and choose $a_n=e^{-n^2}$. Define

$$
X(t)=\sum_{n=1}^\infty a_ng_ne_n(t).
$$

Finite collections of values are limits of centered Gaussian vectors, so this is a centered [Gaussian process](../../../../../gaussian-process.md).

The functions $(e_n)$ are an [orthonormal basis](../../../../../orthonormal-basis.md) of $H=L^2(0,1)$. Hence

$$
\mathbb E\lVert X\rVert_H^2=\sum_{n=1}^\infty a_n^2<\infty,
$$

which proves $\mu_X(H)=1$. For every integer $k\geq0$,

$$
\mathbb E\sum_{n=1}^\infty
|a_ng_n|\lVert e_n^{(k)}\rVert_\infty
\leq C_k\mathbb E|g_1|\sum_{n=1}^\infty e^{-n^2}n^k<\infty.
$$

Thus, almost surely and simultaneously for all $k$, the differentiated series converges uniformly on $(0,1)$. Termwise differentiation gives an almost surely infinitely differentiable version.

Finally, let $F\subset H$ be finite-dimensional. Choose a nonzero $h\in F^\perp$. Then

$$
\langle X,h\rangle_H
=\sum_{n=1}^\infty a_ng_n\langle e_n,h\rangle_H
$$

is a centered normal variable of variance

$$
\sum_{n=1}^\infty a_n^2|\langle e_n,h\rangle_H|^2>0,
$$

because every $a_n$ is positive and $(e_n)$ is complete. The event $\{X\in F\}$ is contained in $\{\langle X,h\rangle_H=0\}$, which has probability zero because a nondegenerate normal distribution has no atoms. Therefore $\mu_X(F)=0$ for every finite-dimensional linear subspace $F$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
