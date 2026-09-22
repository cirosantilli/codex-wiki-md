<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose an orthonormal basis $(e_n)$ of $H_0^1(D)$ and write the GFF formally as $h=\sum_n\xi_ne_n$, where the $\xi_n$ are independent standard normal variables. The [Green-kernel expansion in the Dirichlet space](../../../../../../green-kernel-expansion-in-the-dirichlet-space.md) gives

$$
\sum_{n\geq1}\left(\int_De_n(x)\rho(dx)\right)^2
=\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy)<\infty.
$$

Consequently the series

$$
(h,\rho):=\sum_{n\geq1}\xi_n\int_De_n(x)\rho(dx)
$$

converges in $L^2$. Its partial sums are centered Gaussian and their variances converge to the displayed [Green energy](../../../../../../green-energy.md). The $L^2$ limit is therefore Gaussian with mean zero and variance

$$
\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy).
$$

This constructs the [Finite-Green-energy measure pairing with a Gaussian free field](../../../../../../finite-green-energy-measure-pairing-with-a-gaussian-free-field.md) independently of the chosen orthonormal basis.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
