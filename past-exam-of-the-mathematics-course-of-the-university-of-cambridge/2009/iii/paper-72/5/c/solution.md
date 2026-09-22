<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S_1u$ be the sum of the four axial neighbors and $S_2u$ the sum of the four diagonal neighbors. The two PDF stencils define

$$
\Gamma_9u=\frac23S_1u+\frac16S_2u-\frac{10}3u,
\qquad M_hu=\frac23u+\frac1{12}S_1u.
$$

The reaction stencil has four axial weights $1/12$ and center weight $2/3$, so its weights sum to one. [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
h^{-2}\Gamma_9u=\Delta u+\frac{h^2}{12}\Delta^2u+O(h^4),\qquad
M_hu=u+\frac{h^2}{12}\Delta u+O(h^4).
$$

For example, the diagonal neighbors supply the $u_{xxyy}$ term needed to turn the fourth derivatives into the full squared [Laplacian](../../../../../../laplacian.md). Adding the reaction contribution produces

$$
h^{-2}\Gamma_9u+\lambda M_hu
=(\Delta+\lambda)u+\frac{h^2}{12}\Delta(\Delta+\lambda)u+O(h^4).
$$

On a smooth solution of the constant-coefficient equation, both displayed leading terms vanish. Thus the [compact fourth-order Helmholtz stencil](../../../../../../compact-fourth-order-helmholtz-stencil.md) has

$$
\boxed{\text{fourth-order normalized local accuracy,}\qquad
\Gamma_9u+\lambda h^2M_hu=O(h^6).}
$$

The cancellation uses the differential equation and constant $\lambda$; the [nine-point finite-difference stencil](../../../../../../nine-point-finite-difference-stencil.md) alone still has an $O(h^2)$ operator error on an arbitrary smooth function. It also does not establish a uniform global fourth-order error without an appropriate inverse bound and compatible treatment of boundaries and resonances.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
