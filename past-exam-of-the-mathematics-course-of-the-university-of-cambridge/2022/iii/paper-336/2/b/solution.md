<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For constant width, [separation of variables](../../../../../../separation-of-variables.md) with $\phi=X(x)\sin(n\pi y/h_0)$ gives

$$
X''+k_n^2X=0,
\qquad
\boxed{k_n^2=k_0^2-\frac{n^2\pi^2}{h_0^2}.}
$$

Hence $X=A_ne^{ik_nx}+B_ne^{-ik_nx}$, with imaginary $k_n$ representing an evanescent mode.

For $X=\epsilon x$ and varying width,

$$
k_n(X)^2=k_0^2-\frac{n^2\pi^2}{h(X)^2},
\qquad
\Theta_n=\frac1\epsilon\int_0^Xk_n(\xi)d\xi.
$$

Projection of the next-order equation onto $\sin(n\pi y/h)$, whose squared norm is proportional to $h$, gives

$$
\boxed{2k_nA_n'+\left(k_n'+k_n\frac{h'}h\right)A_n=0,
\qquad
2k_nB_n'+\left(k_n'+k_n\frac{h'}h\right)B_n=0.}
$$

Thus the [WKB amplitude in a slowly varying duct](../../../../../../wkb-amplitude-in-a-slowly-varying-duct.md) is

$$
\boxed{
A_n(X)=A_n(0)\left[\frac{k_n(0)h(0)}{k_n(X)h(X)}\right]^{1/2},
\quad
B_n(X)=B_n(0)\left[\frac{k_n(0)h(0)}{k_n(X)h(X)}\right]^{1/2}.}
$$

This applies for $n\geq1$ away from turning points $k_n=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
