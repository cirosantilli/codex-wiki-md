<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $h=\Delta x$ and sample a sufficiently smooth periodic exact solution. The [central finite differences](../../../../../../central-finite-difference.md) have expansions

$$
\frac{u(x-h)-2u(x)+u(x+h)}{h^2}
=u_{xx}+\frac{h^2}{12}u_{xxxx}+O(h^4),
$$

and

$$
\frac{u(x+h)-u(x-h)}{2h}
=u_x+\frac{h^2}{6}u_{xxx}+O(h^4).
$$

The semidiscrete right side therefore equals $u_{xx}+\alpha u_x+h^2(u_{xxxx}/12+\alpha u_{xxx}/6)+O(h^4)$. The spatial [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) is **second order**, for each fixed $\alpha$. There is no time discretization in the stated ordinary differential system, so no separate temporal approximation order is being assigned. The Taylor statement concerns smooth solutions; [L2-compatible initialization of grid data](../../../../../../l2-compatible-initialization-of-grid-data.md) handles nonsmooth initial data without undefined point sampling.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [3](../../3.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
