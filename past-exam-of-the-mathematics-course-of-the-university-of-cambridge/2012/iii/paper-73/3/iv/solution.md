<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $u^2=\langle u_x^2\rangle$ for the one-component [variance](../../../../../../variance-split.md) and $Q_{LL}=u^2f(r)$. Isotropy gives $Q_{ij}=u^2[(f-g)n_in_j+g\delta_{ij}]$, and incompressibility gives $g=f+rf'/2$. Taking the trace yields

$$
C(r)=u^2[3f+rf']=\frac{u^2}{r^2}\frac{d}{dr}[r^3f(r)].
$$

Therefore, with a regular correlation at the origin,

$$
\boxed{L=4\pi u^2\lim_{r\to\infty}r^3f(r)}.
$$

For $L>0$, the [longitudinal velocity correlation](../../../../../../longitudinal-velocity-correlation.md) has the tail $u^2f(r)\sim L/(4\pi r^3)$. Its physical source is the velocity induced far from a localized eddy with nonzero [hydrodynamic impulse](../../../../../../hydrodynamic-impulse.md). The [hydrodynamic Biot-Savart kernel](../../../../../../hydrodynamic-biot-savart-kernel.md) gives the dipolar far field

$$
\mathbf u_{\rm far}(\mathbf x)=\frac{3\mathbf n(\mathbf I\cdot\mathbf n)-\mathbf I}{4\pi r^3}+\text{higher multipoles}.
$$

The absence of a [vorticity](../../../../../../vorticity.md) monopole and the surviving [impulse](../../../../../../impulse.md) dipole give the $r^{-3}$ power. Random eddy [impulses](../../../../../../impulse.md) thus produce long-range velocity correlations despite the [vorticity](../../../../../../vorticity.md) itself being concentrated in localized structures. Incompressibility also explains how a distant [pressure](../../../../../../pressure.md) response can redistribute velocity without transporting local [vorticity](../../../../../../vorticity.md) there.

There is no inconsistency with integrability of the trace correlation. At leading order, $g\sim-f/2$, so

$$
Q_{ij}(r)\sim\frac{L}{8\pi r^3}(3n_in_j-\delta_{ij}),\qquad
Q_{ii}(r)=0\quad\hbox{at this leading order}.
$$

The longitudinal and transverse dipolar tails cancel in the trace. The scalar [Saffman integral](../../../../../../saffman-integral.md) can remain finite even though individual tensor components have long-range, direction-dependent tails.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
