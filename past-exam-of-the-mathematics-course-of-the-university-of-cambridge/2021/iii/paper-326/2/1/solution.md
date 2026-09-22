<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $u\in L^1(\Omega)$, its [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) is

$$
\operatorname{TV}(u)
=\sup\left\{
\int_\Omega u\,\operatorname{div}\varphi\,dx:
\varphi\in C_c^1(\Omega;\mathbb R^n),\ 
\|\varphi\|_\infty\leq1
\right\}.
$$

The corresponding [bounded-variation space](../../../../../../function-of-bounded-variation-on-a-domain.md) and its zero-mean subspace are

$$
BV(\Omega)=\{u\in L^1(\Omega):\operatorname{TV}(u)<\infty\},
\qquad
BV_0(\Omega)=\left\{u\in BV(\Omega):\int_\Omega u\,dx=0\right\}.
$$

If $u_\Omega=|\Omega|^{-1}\int_\Omega u\,dx$, the [Poincaré inequality for total variation](../../../../../../poincare-inequality-for-total-variation.md) is

$$
\boxed{\|u-u_\Omega\|_{L^1(\Omega)}\leq C_\Omega\operatorname{TV}(u)}.
$$

In particular, $\|u\|_{L^1}\leq C_\Omega\operatorname{TV}(u)$ for $u\in BV_0(\Omega)$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
