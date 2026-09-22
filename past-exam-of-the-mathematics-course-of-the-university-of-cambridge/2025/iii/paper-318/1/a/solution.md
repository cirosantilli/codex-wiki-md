<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The trigonometric [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) says that $p_n^*\in\mathcal T_n$ is best exactly when its error has at least $2n+2$ cyclically ordered extrema of equal magnitude and alternating sign. Let $5^m\leq n<5^{m+1}$ and set $x_j=j\pi/5^{m+1}$. For every $k\geq m+1$,

$$
\cos(5^kx_j)=\cos(j\pi5^{k-m-1})=(-1)^j.
$$

Thus

$$
g(x_j)-\sum_{k=0}^mc_k\cos(5^kx_j)=(-1)^j\sum_{k=m+1}^\infty c_k.
$$

There are $2\cdot5^{m+1}\geq2n+2$ such extrema, while the [triangle inequality](../../../../../../triangle-inequality.md) bounds the tail by their common magnitude. Hence

$$
\boxed{p_n^*(x)=\sum_{k=0}^mc_k\cos(5^kx)},\qquad
\boxed{E_n(g)=\sum_{k=m+1}^\infty c_k}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
