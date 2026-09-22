<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let there be $J$ interior points. The [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has positive values

$$
\eta_j=4\sin^2\left(\frac{j\pi}{2(J+1)}\right)
$$

for the eigenvalues of its negative, and the amplification eigenvalues are $(1+\mu\eta_j)^{-1}$. Therefore the [Backward Euler diffusion stability on a finite Dirichlet interval](../../../../../../backward-euler-diffusion-stability-on-a-finite-dirichlet-interval.md) is

$$
\boxed{\mu\geq0
\quad\text{or}\quad
\mu\leq-\frac1{2\sin^2(\pi/(2(J+1)))}}.
$$

If, as usual, a Courant number is restricted to nonnegative values, this again reduces to all $\mu\geq0$. The additional negative branch is a finite-grid artefact and disappears to $-\infty$ as the mesh is refined.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
