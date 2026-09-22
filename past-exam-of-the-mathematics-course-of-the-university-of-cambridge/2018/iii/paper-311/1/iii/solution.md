<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose the asymptotic time translation: $N=1+O(r^{-1})$, $N^i=O(r^{-1})$, with their derivatives $O(r^{-2})$, in asymptotically Cartesian coordinates. Use the usual differentiable falloff $h_{ij}=\delta_{ij}+O(r^{-1})$, $\partial_kh_{ij}=O(r^{-2})$, $\pi^{ij}=O(r^{-2})$, and analogous falloff for allowed variations; impose the standard additional conditions needed for finite bulk integrals. These variations need not fix the [Arnowitt-Deser-Misner energy](../../../../../../arnowitt-deser-misner-energy.md).

Only the spatial curvature term produces the leading nonvanishing surface variation. Applying the variation of the [Ricci scalar](../../../../../../ricci-scalar.md) and applying [integration by parts](../../../../../../integration-by-parts.md) to its two derivative terms yields

$$
\delta H_{\rm bulk}
=\int d^3x\left(\mathcal F^{ij}\delta h_{ij}+\mathcal G_{ij}\delta\pi^{ij}\right)
-\lim_{r\to\infty}\int_{S_r}dA\,n^i(\partial_j\delta h_{ij}-\partial_i\delta h_{jj}).
$$

The terms involving derivatives of the asymptotic [lapse function](../../../../../../lapse-function.md), and the shift boundary terms, vanish under these falloff conditions. The displayed surface integral need not vanish: its integrand is $O(r^{-2})$ and the area is $O(r^2)$.

[Hamilton's equations](../../../../../../hamilton-s-equations.md) require a [Hamiltonian](../../../../../../hamiltonian.md) with a variation expressed by the bulk [functional derivatives](../../../../../../functional-derivative.md) alone for the allowed variations. The unwanted term is exactly $-\delta E_{\rm ADM}$, so [differentiability of the gravitational Hamiltonian at spatial infinity](../../../../../../differentiability-of-the-gravitational-hamiltonian-at-spatial-infinity.md) requires

$$
\boxed{H_{\rm total}=H_{\rm bulk}+E_{\rm ADM}.}
$$

Its variation cancels the surface term. On the constraint surface, $H_{\rm total}=E_{\rm ADM}$. Restoring units inserts $1/(16\pi G)$ in the surface integral; the paper has set this factor to one. The original PDF has the standard equation $\partial_t h_{ij}=\delta H/\delta\pi^{ij}$; the extra $t$ in the extracted TeX is a transcription error.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
