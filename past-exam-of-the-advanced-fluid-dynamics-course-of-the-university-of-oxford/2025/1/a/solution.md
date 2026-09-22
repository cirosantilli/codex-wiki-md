<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

To first order in fluid [velocity](../../../../velocity.md) divided by the [speed of light](../../../../speed-of-light.md), the [Lorentz transformation of electromagnetic fields](../../../../lorentz-transformation-of-electromagnetic-fields.md) gives $\mathbf E'=\mathbf E+\mathbf u\times\mathbf B$. Applying [Ohm's law](../../../../ohm-s-law.md) in the local fluid frame gives $\mathbf E+\mathbf u\times\mathbf B=\eta\mathbf J$. Neglecting the [displacement current](../../../../displacement-current.md) in [Ampère's law](../../../../ampere-s-circuital-law.md), $\mathbf J=\nabla\times\mathbf B/\mu_0$. Substitution in [Faraday's law](../../../../faraday-s-law-of-induction.md) gives

$$
\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)-\frac\eta{\mu_0}\nabla\times(\nabla\times\mathbf B)
=\nabla\times(\mathbf u\times\mathbf B)+\eta_m\nabla^2\mathbf B,\qquad\eta_m=\frac\eta{\mu_0}.
$$

Here $\eta_m$ is the [magnetic diffusivity](../../../../magnetic-diffusivity.md); the paper's $\eta$ is [electrical resistivity](../../../../electrical-resistivity.md), rather than [magnetic diffusivity](../../../../magnetic-diffusivity.md). Expanding the curl with the [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md) gives the [resistive induction equation](../../../../resistive-induction-equation.md) in its compressible form:

$$
\boxed{\partial_t\mathbf B+(\mathbf u\cdot\nabla)\mathbf B=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\,\nabla\cdot\mathbf u+\frac\eta{\mu_0}\nabla^2\mathbf B.}
$$

The left side is the [material derivative](../../../../material-derivative.md) of the [magnetic field](../../../../magnetic-field-split.md). The three right-hand terms respectively describe field-line stretching and reorientation, amplification or dilution by compression or expansion, and [magnetic diffusion](../../../../magnetic-diffusion.md). In particular, compression has $\nabla\cdot\mathbf u<0$ and amplifies a field component perpendicular to the compression.

The assumptions are nonrelativistic bulk motion, the low-frequency approximation permitting omission of the [displacement current](../../../../displacement-current.md), a conducting-fluid continuum, isotropic local [Ohm's law](../../../../ohm-s-law.md) with spatially constant scalar [electrical resistivity](../../../../electrical-resistivity.md), constant [magnetic permeability](../../../../permeability-electromagnetism.md) $\mu_0$, and $\nabla\cdot\mathbf B=0$. Hall, electron-pressure and other non-Ohmic corrections to the generalized [Ohm's law](../../../../ohm-s-law.md) are excluded. [Incompressible flow](../../../../incompressible-flow.md) is not required: imposing it would remove the compression term.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
