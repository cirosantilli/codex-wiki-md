<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Let the unit normal point from layer 1 to layer 2. The electrostatic [electric field](../../../../../electric-field-split.md) boundary condition is $\mathbf n\times(\mathbf E_2-\mathbf E_1)=0$, while [Gauss's law](../../../../../gauss-s-law.md) for the [electric displacement field](../../../../../electric-displacement-field.md) gives $\mathbf n\cdot(\mathbf D_2-\mathbf D_1)=\sigma_f$. Here $\epsilon_i$ denotes absolute [permittivity](../../../../../permittivity-split.md); replace it by $\epsilon_0\epsilon_{ri}$ if dielectric constants are relative.

In the steady conducting state, [charge conservation](../../../../../charge-conservation.md) makes the normal [current density](../../../../../current-density.md) the same in both layers:

$$
J=\sigma_1E_1=\sigma_2E_2,\qquad V=E_1d_1+E_2d_2.
$$

Writing $\mathcal D=\sigma_2d_1+\sigma_1d_2$, the [steady fields in two leaky dielectric layers](../../../../../steady-fields-in-two-leaky-dielectric-layers.md) are

$$
\boxed{E_1=\frac{\sigma_2V}{\mathcal D},\qquad E_2=\frac{\sigma_1V}{\mathcal D},\qquad J=\frac{\sigma_1\sigma_2V}{\mathcal D}.}
$$

The signed interfacial free [surface charge density](../../../../../surface-charge-density.md) is the jump of $D_n$:

$$
\boxed{\sigma_f=\frac{(\epsilon_2\sigma_1-\epsilon_1\sigma_2)V}{\mathcal D}.}
$$

The total free-plus-bound sheet charge instead follows from the vacuum form of [Gauss's law](../../../../../gauss-s-law.md),

$$
\boxed{\sigma_{\rm total}=\epsilon_0(E_2-E_1)
=\frac{\epsilon_0(\sigma_1-\sigma_2)V}{\mathcal D}.}
$$

The bound contribution is $\sigma_{\rm total}-\sigma_f$. These are signed quantities for the chosen normal and voltage direction; their magnitudes are obtained by absolute values. They describe the long-time DC state, not the initial capacitive transient. Positive conductivities suffice for the derivation; if both vanish, conductivity alone does not determine the field division, which also depends on the initial free interfacial charge.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2A](../../../paper-2a-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](../../../paper-2b/section-b/b6/solution.md)
