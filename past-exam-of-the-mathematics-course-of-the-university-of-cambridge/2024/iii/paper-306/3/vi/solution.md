<h1 id="3/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Extract a mode using

$$
G_m=\oint_0\frac{dz}{2\pi i}\,z^{m+1/2}G(z),
\qquad
L_k=\oint_0\frac{dw}{2\pi i}\,w^{k+1}T(w).
$$

In the radially ordered double contour for the anticommutator, the simple pole $2T(w)/(z-w)$ gives $2L_{m+n}$. Expanding $z^{m+1/2}$ about $w$, the third-order pole contributes one half of its second derivative,

$$
\frac12\left(m+\frac12\right)\left(m-\frac12\right)
w^{m-3/2}.
$$

The remaining contour is nonzero only for $m+n=0$. Restoring the general leading OPE coefficient $2c/3$ gives

$$
\boxed{
\{G_m,G_n\}=2L_{m+n}
+\frac c{12}(4m^2-1)\delta_{m,-n}}.
$$

This is the fermionic relation in the [N=1 super-Virasoro algebra](../../../../../../n-1-super-virasoro-algebra.md).

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [3](../../3.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
