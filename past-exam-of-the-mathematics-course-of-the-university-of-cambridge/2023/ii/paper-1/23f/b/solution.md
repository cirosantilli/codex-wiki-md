<h1 id="23f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $1\leq p<\infty$, choose nonzero $\phi\in C_c(\mathbb R^{n-1})$ and $\psi\in C_c(\mathbb R)$ with $\psi(0)=1$. Define

$$
u_k(x',x_n)=\phi(x')\psi(kx_n).
$$

These functions are continuous and belong to the [Lebesgue space](../../../../../../lp-space.md) $L^p(\mathbb R^n)$, while their restrictions to the hyperplane are all the same:

$$
u_k(x',0)=\phi(x').
$$

Changing variables in the normal coordinate gives

$$
\lVert u_k\rVert_{L^p(\mathbb R^n)}^p
=\frac1k\lVert\phi\rVert_{L^p(\mathbb R^{n-1})}^p
\lVert\psi\rVert_{L^p(\mathbb R)}^p
\longrightarrow0.
$$

If the claimed bounded $T$ existed, then

$$
0<\lVert\phi\rVert_p
=\lVert Tu_k\rVert_p
\leq\lVert T\rVert\,\lVert u_k\rVert_p
\longrightarrow0,
$$

a contradiction. This scaling argument is the [failure of an Lp hyperplane trace](../../../../../../failure-of-an-lp-hyperplane-trace.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
