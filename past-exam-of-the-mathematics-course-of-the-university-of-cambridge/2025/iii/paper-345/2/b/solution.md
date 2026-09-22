<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [reduced gravity](../../../../../../reduced-gravity-split.md)

$$
g'=g\frac{\rho_1-\rho_2}{\rho_2},
$$

and use the Boussinesq limit $\rho_1\simeq\rho_2$ except in buoyancy. The balances become

$$
g'_t+ug'_x=-g'\frac{w_e}{h},
$$



$$
h_t+uh_x+hu_x=w_e-w_d,
$$



$$
u_t+uu_x+g'h_x+\frac h2g'_x=-u\frac{w_e}{h}.
$$

Thus, for $\mathbf q=(g',h,u)^T$,

$$
\boxed{
\mathbf q_t+
\begin{pmatrix}
u&0&0\\
0&u&h\\
h/2&g'&u
\end{pmatrix}\mathbf q_x
=
\begin{pmatrix}
-g'w_e/h\\
w_e-w_d\\
-uw_e/h
\end{pmatrix}},
$$

which is the required [entraining shallow-water layer](../../../../../../entraining-shallow-water-layer.md) system.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
