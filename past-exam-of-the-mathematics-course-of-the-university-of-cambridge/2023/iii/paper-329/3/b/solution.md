<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With no $y$ dependence, integrate the dimensionless equation once. The upstream condition fixes the constant:

$$
h^3-h^3h_x=1,
\qquad
\boxed{h_x=1-h^{-3}}.
$$

Write $h=1+\eta$ upstream. Linearization gives $\eta_x=3\eta$, so

$$
\boxed{h\sim1+Ae^{3x}},
\qquad k=3.
$$

For $A>0$, the thickness increases monotonically. At large $h$,

$$
\frac{dx}{dh}=\frac1{1-h^{-3}}
=1+h^{-3}+O(h^{-6}).
$$

Integration gives $x-x_0=h-	frac12h^{-2}+O(h^{-5})$, and inversion yields

$$
\boxed{h=x-x_0+O(x^{-2})}.
$$

In dimensional variables, $dh_{\rm dim}/dx_{\rm dim}\to\alpha$. The increasing thickness therefore cancels the plane's downward slope, so the free surface becomes asymptotically horizontal. The profile represents the upslope edge of a deep viscous pool or pond held back by an obstruction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
