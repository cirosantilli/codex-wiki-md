<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x,y>0$, the [Laplace transform](../../../../../../laplace-transform.md) identity

$$
\frac1{x+y}=\int_0^\infty e^{-tx}e^{-ty}\,dt
$$

exhibits $k_1$ as an inner product of the [feature functions](../../../../../../feature-map.md) $t\mapsto e^{-tx}$ in $L^2(0,\infty)$. More explicitly, for any real $c_i$ and positive $x_i$,

$$
\sum_{i,j}c_ic_jk_1(x_i,x_j)
=\int_0^\infty\left(\sum_i c_i e^{-tx_i}\right)^2dt\geq0.
$$

**Therefore $k_1$ is a [positive-semidefinite kernel](../../../../../../positive-semidefinite-kernel.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
