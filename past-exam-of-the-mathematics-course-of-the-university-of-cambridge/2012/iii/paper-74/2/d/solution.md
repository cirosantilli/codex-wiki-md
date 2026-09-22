<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [functional derivative](../../../../../../functional-derivative.md) is $\delta\mathcal E/\delta h=Ah^{(4)}$, so the [overdamped filament bending equation](../../../../../../small-slope-elastohydrodynamic-filament-equation.md) is $\zeta h_t=-Ah^{(4)}$ with the free-end conditions from (a). Expand the initial shape in the complete [orthonormal basis](../../../../../../orthonormal-basis.md):

$$
c_j=\int_0^L W_j(x)H(x)\,dx.
$$

The [overdamped relaxation of a free filament](../../../../../../overdamped-relaxation-of-a-free-filament.md) is

$$
\boxed{h(x,t)=c_{\rm tr}W_{\rm tr}(x)+c_{\rm tilt}W_{\rm tilt}(x)
+\sum_{n\geq1}c_nW_n(x)e^{-Ak_n^4t/\zeta}.}
$$

Each bending mode relaxes on time $\tau_n=\zeta/(Ak_n^4)$; the two zero modes remain constant. Consequently the long-time shape is the affine projection of $H$,

$$
h_\infty(x)=\frac1L\int_0^L H(s)ds
+\frac{12(x-L/2)}{L^3}\int_0^L(s-L/2)H(s)ds.
$$

The total displacement and its first moment are conserved: integrate $h_t$ and $(x-L/2)h_t$, using $h''=h^{(3)}=0$ at the ends. This also checks why the final affine part cannot generally be set to zero. The series defines the $L^2$ solution for arbitrary square-integrable initial data; a classical solution at time zero additionally requires compatible boundary values.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
