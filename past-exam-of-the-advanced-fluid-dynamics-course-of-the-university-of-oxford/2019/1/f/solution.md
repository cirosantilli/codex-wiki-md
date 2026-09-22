<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The common part of the [magnetohydrodynamic-viscoelastic analogy](../../../../magnetohydrodynamic-viscoelastic-analogy.md) is stretching and advection of a line element. With the component-first [velocity gradient](../../../../velocity-gradient.md) $L_{ij}=\partial_j u_i$, the ideal tensor equation is

$$
D_tM-LM-ML^T=0.
$$

Its left side is an [upper-convected derivative](../../../../upper-convected-derivative.md), the same deformation law that appears for a [polymer](../../../../polymer-split.md) [conformation tensor](../../../../conformation-tensor.md) when its relaxation is neglected.

There are two important physical differences. First, the [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md) prevents a [magnetic field line](../../../../magnetic-field-line.md) from having an isolated source or sink inside the fluid. A [polymer](../../../../polymer-split.md) strand can have molecular endpoints, so there is no corresponding no-endpoint constraint on the strands. Second, a stretched [polymer](../../../../polymer-split.md) has a preferred relaxed distribution of configurations and a finite [polymer relaxation time](../../../../polymer-relaxation-time.md); it can recoil relative to the solvent through molecular drag and thermal motion. An ideal [magnetic field](../../../../magnetic-field-split.md) has no analogous local tendency to return to a prescribed coil size. Real [polymers](../../../../polymer-split.md) also have a finite contour length, a limitation absent from the ideal field-stretching law.

For example, a normalized [Hookean dumbbell conformation equation](../../../../hookean-dumbbell-conformation-equation.md) has the dissipative extension

$$
\boxed{D_tC-LC-CL^T=-\frac1\tau(C-I).}
$$

This is local relaxation toward an isotropic thermal configuration. It remains nonzero for a spatially uniform stretched $C$. By contrast, constant [magnetic diffusivity](../../../../magnetic-diffusivity.md) $\eta_m$ adds $\eta_m\nabla^2\mathbf B$ to the [resistive induction equation](../../../../resistive-induction-equation.md). The product rule gives the [resistive evolution of the magnetic second-moment tensor](../../../../resistive-evolution-of-the-magnetic-second-moment-tensor.md):

$$
\boxed{D_tM_{ij}-L_{in}M_{nj}-M_{in}L_{jn}
=\eta_m\nabla^2M_{ij}
-2\eta_m(\partial_nB_i)(\partial_nB_j).}
$$

The magnetic correction involves spatial gradients, vanishes for a uniform [magnetic field](../../../../magnetic-field-split.md), and does not create field-line endpoints: $\partial_t(\nabla\cdot\mathbf B)=\eta_m\nabla^2(\nabla\cdot\mathbf B)$. It permits slippage and [magnetic reconnection](../../../../magnetic-reconnection.md) while preserving the no-monopole constraint. After averaging, its gradient-product term generally needs additional information beyond the averaged $M$. One cannot replace it indiscriminately by the local [polymer](../../../../polymer-split.md) relaxation term, or even by $\eta_m\nabla^2M$ alone.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
