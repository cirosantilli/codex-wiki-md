<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [long-wavelength approximation in cosmology](../../../../../../long-wavelength-approximation-in-cosmology.md) organizes equations in powers of $\epsilon\sim k/(aH)\ll1$, while allowing finite perturbation amplitudes. For fields and lapse varying on the same large spatial scale, a spatial derivative is of order $\epsilon$ relative to a temporal expansion scale. Intrinsic spatial curvature, scalar gradient energy, and second spatial derivatives of the lapse are therefore second order and can be neglected at leading order. First-gradient constraints must still be retained: they relate neighboring locally homogeneous patches. During [cosmic inflation](../../../../../../cosmic-inflation-split.md), physical wavelengths stretch while the Hubble scale changes slowly, improving this expansion. Sharp spatial features or independently large anisotropic expansion require additional care.

Set the shift to zero, let $S^i{}_j=\widetilde K^i{}_j$, $S^2=S^i{}_jS^j{}_i$, and keep the lapse explicit. The normal scalar momentum is $\Pi=\dot\phi/N$, and the [shear-inclusive long-wavelength scalar equations](../../../../../../shear-inclusive-long-wavelength-scalar-equations.md) obtained from the given Einstein and scalar equations are

$$
\boxed{\begin{aligned}
\dot a&=NaH,&\dot\phi&=N\Pi,\\
\dot\Pi&=-N(3H\Pi+V_{,\phi}),&3H^2&=8\pi G(\Pi^2/2+V)+\tfrac12S^2,\\
\dot H&=-4\pi GN\Pi^2-\tfrac12NS^2,&\dot S^i{}_j&=-3NH S^i{}_j,\\
D_iH&=-4\pi G\Pi D_i\phi-\tfrac12D_jS^j{}_i.
\end{aligned}}
$$

Terms with two spatial gradients have been omitted in the time equations; the last equation is the retained first-gradient [momentum constraint](../../../../../../momentum-constraint.md). The Friedmann-type equation is the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md). To check the Hubble evolution, the trace equation gives $\dot H=-3NH^2+8\pi GNV$; inserting the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) gives the displayed kinetic and [cosmological shear](../../../../../../cosmological-shear.md) terms. Shear energy is not a spatial-gradient correction and cannot be discarded merely because the wavelength is large.

The trace-free evolution integrates immediately:

$$
\frac{d}{dt}(a^3S^i{}_j)=a^3(\dot S^i{}_j+3NH S^i{}_j)=0,\qquad\boxed{\widetilde K^i{}_j=C^i{}_j(\mathbf x)a^{-3}.}
$$

The arbitrary spatial integration tensor is trace free and must obey the initial constraints. This [inflationary shear damping](../../../../../../inflationary-shear-damping.md) suppresses anisotropic expansion exponentially during sustained inflation; its contribution $S^2$ falls as $a^{-6}$. It does not force the spatial conformal metric to be exactly flat: a frozen anisotropic shape or tensor perturbation can survive with negligible time-dependent [cosmological shear](../../../../../../cosmological-shear.md).

After this decaying [cosmological shear](../../../../../../cosmological-shear.md) mode and its first-gradient contribution become negligible, the equations simplify to $3H^2=8\pi G(\Pi^2/2+V)$ and $D_iH=-4\pi G\Pi D_i\phi$. Spatially differentiating the first relation gives

$$
6H D_iH=8\pi G(\Pi D_i\Pi+V_{,\phi}D_i\phi).
$$

Substitute the [momentum constraint](../../../../../../momentum-constraint.md) and divide by $\Pi\ne0$ to obtain $D_i\Pi=-(3H+V_{,\phi}/\Pi)D_i\phi$. The time scalar equation, together with $\dot\phi=N\Pi$, similarly becomes $\dot\Pi=-(3H+V_{,\phi}/\Pi)\dot\phi$. Finally $\dot H=-4\pi G\Pi\dot\phi$. Thus the requested single-clock relations are

$$
\boxed{\begin{aligned}
\dot\Pi&=-\left(3H+\frac{V_{,\phi}}\Pi\right)\dot\phi,&D_i\Pi&=-\left(3H+\frac{V_{,\phi}}\Pi\right)D_i\phi,\\
\dot H&=-4\pi G\Pi\dot\phi,&D_iH&=-4\pi G\Pi D_i\phi.
\end{aligned}}
$$

These retain arbitrary lapse and reduce to proper-time expressions when $N=1$. The division assumes the scalar is a valid local clock; turning points with $\Pi=0$ need another regular variable or a limiting treatment. The shear-neglect step, rather than the long-wavelength expansion alone, is what permits these single-clock spatial relations.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
