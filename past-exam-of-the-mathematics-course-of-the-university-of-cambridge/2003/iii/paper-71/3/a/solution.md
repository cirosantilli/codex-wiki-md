<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $B$ for the [filament bending modulus](../../../../../../filament-bending-modulus.md) and $C$ for the [filament torsional stiffness](../../../../../../filament-torsional-stiffness.md), so that the [energy](../../../../../../energy.md) per unit length is $(B\kappa^2+C\Omega^2)/2$. For one circular filament,

$$
B_1=EI_1=\frac{\pi Er^4}{4},\qquad C_1=G_sJ_1=\frac{\pi G_sr^4}{2},\qquad G_s=\frac{E}{2(1+\nu)},
$$

where $I_1$ is the [second moment of area](../../../../../../second-moment-of-area.md), $J_1$ the polar moment, $G_s$ the [shear modulus](../../../../../../shear-modulus.md), and $\nu$ [Poisson's ratio](../../../../../../poisson-s-ratio.md). Numerical twisting constants cannot be fixed by [Young's modulus](../../../../../../young-s-modulus.md) alone without specifying $\nu$.

For a filled sliding bundle, $N\sim(R/r)^2$. Filaments share the centerline curvature but slide instead of accumulating the additional axial strains of a bonded cross-section. Their bending energies add: **$B\sim NB_1\sim Er^2R^2$**. If end constraints impose the same material twist on every filament, their torsional energies also add: **$C\sim G_sr^2R^2$**.

For a bonded, one-filament-thick circular tube, the wall thickness $h$ is of order $r$. Its moments are $I\sim\pi R^3h$ and $J_p\sim2\pi R^3h$, giving **$B\sim ErR^3$ and $C\sim G_srR^3$**. For a bonded filled rod, $I\sim\pi R^4/4$ and $J_p\sim\pi R^4/2$, giving **$B\sim ER^4$ and $C\sim G_sR^4$**. Packing fractions and the convention for tube radius affect constants, not these powers.

There is an important qualification to [bending and torsion of filament bundles](../../../../../../bending-and-torsion-of-filament-bundles.md): free axial sliding does not specify whether each filament can also spin freely. If both spin and slip are unconstrained, the common-material-twist calculation is not forced by the geometry. A helix of small twist rate has centerline curvature of order $\rho\Omega^2$, so its bending [energy](../../../../../../energy.md) starts at $\Omega^4$, not $\Omega^2$. A nonzero linear collective torsional stiffness then requires additional end, contact, or spin constraints.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
