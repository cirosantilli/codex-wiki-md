<h1 id="section-a-ii/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An **on-axis point illuminator increases spatial coherence**. It is not a point object, and it does not remove [diffraction](../../../../../../diffraction.md). For an ideal aberration-free pupil, [coherent imaging](../../../../../../coherent-imaging.md) is linear in field amplitude and has cutoff

$$
\boxed{\nu_c=\frac{\mathrm{NA}}{\lambda}}.
$$

For a real amplitude grating $U(x)=a[1+m\cos(2\pi\nu x)]$, with $0\leq m\leq1$ and all three field orders inside this pupil, the intensity contrast is $C=2m/(1+m^2)$. Flat coherent field transfer preserves this contrast; weak input modulation does not itself meet a high resist contrast threshold. Assume a sufficiently high-contrast amplitude mask: for example, $m=1$ gives $C=1$, exceeding both resist thresholds. Under this assumption, both resists have the same limiting equal-line/space width

$$
\boxed{w_c=\frac1{2\nu_c}=\frac{\lambda}{2\mathrm{NA}}
=241\,\mathrm{nm}},\qquad P_c=483\,\mathrm{nm}.
$$

This is an approach to the cutoff from below; finite dose latitude, aberrations and a real binary mask can make usable resolution worse. A general coherent intensity image cannot be obtained by applying an incoherent intensity MTF unchanged: $I=|h*U|^2$, rather than $I=|h|^2*|U|^2$.[coherent/incoherent comparison: field cutoff versus the twice-as-wide incoherent intensity cutoff](../../../../../../advanced-optical-imaging-incoherent-imaging-by-delft-university-of-technology.md)

With $\nu_0=2\mathrm{NA}/\lambda$, this coherent cutoff is $0.5\nu_0$: the low-contrast resist improves from roughly $302$ to $241\,\mathrm{nm}$, while the high-contrast resist worsens from roughly $201$ to $241\,\mathrm{nm}$. Coherence improves contrast within its passband but reduces the ultimate bandwidth relative to incoherent illumination.

With the literal Rayleigh-spacing normalization $\nu_0=1/R_R$, the same physical cutoff is instead $0.61\nu_0$, not $0.5\nu_0$. The corresponding widths from the preceding part would improve from roughly $368$ and $245\,\mathrm{nm}$ toward $241\,\mathrm{nm}$. **The cutoff in physical units is unambiguous under the stated ideal on-axis model; the claimed direction and size of a change inferred from the plotted normalized axis depend on its definition.** Off-axis illumination, partial coherence and arbitrary phase objects require a fuller imaging model.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Section A(ii)](../../../section-a-ii.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
