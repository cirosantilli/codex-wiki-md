<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [International System of Units](../../../../international-system-of-units.md), with $c^{-2}=\mu_0\varepsilon_0$. The [Maxwell equations](../../../../maxwell-equations-split.md) with [charge density](../../../../charge-density.md) $\rho$ and [current density](../../../../current-density.md) $\mathbf J$ are

$$
\boxed{\nabla\cdot\mathbf E=\rho/\varepsilon_0,\qquad\nabla\cdot\mathbf B=0,\qquad\nabla\times\mathbf E=-\partial_t\mathbf B,\qquad\nabla\times\mathbf B=\mu_0\mathbf J+c^{-2}\partial_t\mathbf E.}
$$

Locally, or in a suitable contractible region, the zero [divergence](../../../../divergence.md) of $\mathbf B$ allows a [magnetic vector potential](../../../../magnetic-vector-potential.md) $\mathbf B=\nabla\times\mathbf A$. [Faraday's law](../../../../faraday-s-law-of-induction.md) then makes $\mathbf E+\partial_t\mathbf A$ [curl](../../../../curl.md)-free, so a [electric potential](../../../../electric-potential.md) can be chosen with

$$
\boxed{\mathbf E=-\nabla\Phi-\partial_t\mathbf A,\qquad\mathbf B=\nabla\times\mathbf A.}
$$

These formulas automatically satisfy the two homogeneous [Maxwell equations](../../../../maxwell-equations-split.md). The local topology assumption rules out obstructions to expressing a closed field as a [gradient](../../../../gradient.md) or [curl](../../../../curl.md).

For any sufficiently smooth scalar $\chi$, the [gauge transformation](../../../../gauge-transformation.md)

$$
\boxed{\mathbf A\mapsto\mathbf A+\nabla\chi,\qquad\Phi\mapsto\Phi-\partial_t\chi}
$$

leaves both physical fields unchanged, because [curl](../../../../curl.md) of a [gradient](../../../../gradient.md) is zero and spatial and time [derivatives](../../../../derivative.md) commute. In such a region this accounts for the freedom between potentials for the same fields.

The [Lorenz gauge](../../../../lorenz-gauge-condition.md) is $\nabla\cdot\mathbf A+c^{-2}\partial_t\Phi=0$. Substitution into the sourced [Maxwell equations](../../../../maxwell-equations-split.md), using $\nabla\times(\nabla\times\mathbf A)=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A$, gives the decoupled [wave equations](../../../../wave-equation-split.md)

$$
\boxed{(\nabla^2-c^{-2}\partial_t^2)\Phi=-\rho/\varepsilon_0,\qquad(\nabla^2-c^{-2}\partial_t^2)\mathbf A=-\mu_0\mathbf J.}
$$

For example, Gauss's law gives $-\nabla^2\Phi-\partial_t\nabla\cdot\mathbf A=\rho/\varepsilon_0$; the gauge condition turns this into the scalar equation. The remaining gauge freedom preserving the condition has $(\nabla^2-c^{-2}\partial_t^2)\chi=0$.

Put $\theta=\omega t-Kz$ for the given wave. Direct differentiation gives $\nabla\cdot\mathbf E=0$ and $\nabla\times\mathbf E=K\mathbf E$. Integrating [Faraday's law](../../../../faraday-s-law-of-induction.md) in time yields the wave's [magnetic field](../../../../magnetic-field-split.md)

$$
\boxed{\mathbf B=\frac K\omega\,\widehat{\mathbf z}\times\mathbf E=\frac{KE}{\omega}(-\sin\theta,\cos\theta,0).}
$$

One could superpose a time-independent [divergence](../../../../divergence.md)-free and [curl](../../../../curl.md)-free [magnetic field](../../../../magnetic-field-split.md); the expression displayed chooses no such extra background. It has zero [divergence](../../../../divergence.md) and $\partial_t\mathbf B=-K\mathbf E$, so the magnetic Gauss and Faraday equations hold. Moreover

$$
\nabla\times\mathbf B=\frac{K^2}{\omega^2}\partial_t\mathbf E.
$$

Since the time [derivative](../../../../derivative.md) is nonzero, the vacuum [Ampere-Maxwell law](../../../../ampere-s-circuital-law.md) holds precisely when

$$
\boxed{K^2=\omega^2/c^2.}
$$

This verifies all four source-free equations, including both [divergence](../../../../divergence.md) constraints. The sign of $\omega/K$ selects the direction of propagation.

A wave has [circular polarization](../../../../circular-polarization.md) when, at a fixed spatial point, its transverse electric [vector](../../../../vector.md) has constant nonzero magnitude and rotates uniformly through a circle. Here $E_x^2+E_y^2=E^2$ and the angle changes at rate $\omega$, so **the wave is circularly polarized**. Its magnetic [vector](../../../../vector.md) is perpendicular to the electric [vector](../../../../vector.md), has magnitude $|E|/c$ under the [dispersion relation](../../../../dispersion-relation-split.md), and rotates with it. A handedness label additionally requires a convention for the observer's viewing direction.

The [Lorenz-gauge potentials for a circularly polarized plane wave](../../../../lorenz-gauge-potentials-for-a-circularly-polarized-plane-wave.md) give a convenient choice. Take $\Phi=0$ and $\mathbf A=\omega^{-2}\partial_t\mathbf E$. Because $\partial_t^2\mathbf E=-\omega^2\mathbf E$,

$$
-\partial_t\mathbf A=\mathbf E,\qquad
\nabla\times\mathbf A=\omega^{-2}\partial_t(K\mathbf E)=\frac K\omega\widehat{\mathbf z}\times\mathbf E=\mathbf B.
$$

Also $\nabla\cdot\mathbf A=\omega^{-2}\partial_t\nabla\cdot\mathbf E=0$. Together with $\partial_t\Phi=0$, this proves **these potentials satisfy the [Lorenz gauge](../../../../lorenz-gauge-condition.md)**. They satisfy the source-free potential [wave equations](../../../../wave-equation-split.md) because every component has the same [dispersion relation](../../../../dispersion-relation-split.md) just obtained.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the quantum mechanics and electromagnetism course of the University of Oxford](../../../split.md)
5. [Quantum mechanics and electromagnetism course of the University of Oxford](../../../../quantum-mechanics-and-electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
