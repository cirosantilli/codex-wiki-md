<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the printed $A_0=0$ as the empty initial hull. Write $a(t)=\operatorname{hcap}(\widetilde A_t)$ and $F_t=\psi_t$. [Conformal maps](../../../../../../conformal-map.md) preserve inclusion and simple connectedness of the complementary domains, so the image sets form an increasing hull family. Boundedness of $\psi$ on bounded sets ensures that these image hulls are bounded. The [Loewner local growth property](../../../../../../loewner-local-growth-property.md) is preserved under conformal transport: after mapping out the hull at time $t$, the small new hull is transported by $F_t$ near its single boundary growth point. The [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md) extends $F_t$ analytically across that point, with real positive derivative. The image diameters therefore tend to zero as the original ones do. These statements use the usual hull closures and [prime ends](../../../../../../prime-end.md); the initial image hull is empty.

For completeness, the infinitesimal capacity rule underlying this argument is that a shrinking hull $J$ attached near $u$, transported by a map $F$ analytic there, has

$$
\operatorname{hcap}(F(J))=F'(u)^2\operatorname{hcap}(J)+o(\operatorname{hcap}(J)).
$$

One obtains this by rescaling at $u$: the transported map tends to its linear part, and [half-plane capacity](../../../../../../half-plane-capacity.md) scales by the square of the dilation. Uniform analytic distortion near the growth point controls the error. Applying it to the mapped-out increments gives local absolute continuity of $a$ and $a'(t)=2F_t'(U_t)^2$.

The coefficient can also be read directly from the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md). The image driver is $\widetilde U_t=F_t(U_t)$. Differentiate $F_t=\widetilde g_t\circ\psi\circ g_t^{-1}$, at a fixed point $w$, to obtain

$$
\partial_tF_t(w)=\frac{a'(t)}{F_t(w)-F_t(U_t)}-\frac{2F_t'(w)}{w-U_t}.
$$

The left side is regular at $w=U_t$. On the right, the coefficient of $(w-U_t)^{-1}$ is $a'(t)/F_t'(U_t)-2F_t'(U_t)$, so it must vanish. This proves the [conformal change of half-plane capacity](../../../../../../conformal-change-of-half-plane-capacity.md) rule and its integrated version:

$$
\boxed{\operatorname{hcap}(\widetilde A_t)=\int_0^t2\bigl(\psi_s'(U_s)\bigr)^2\,ds,\qquad\widetilde A_0=\varnothing.}
$$

If the derivative at the initial boundary point is singular, the formula is interpreted by integrating from a positive time and taking the lower limit to zero; finite image capacity and kernel continuity give this limit. The duplicated incomplete normalization sentence in the TeX is absent from the PDF.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
