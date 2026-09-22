<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [real scalar field](../../../../real-scalar-field.md) suffices to describe one neutral species of bosonic [quasiparticle](../../../../quasiparticle.md). Let $\pi(\mathbf x)$ be its [canonical momentum](../../../../canonical-momentum.md). In three spatial dimensions, choose the positive classical [Hamiltonian](../../../../hamiltonian.md)

$$
\boxed{H[\phi,\pi]=\frac12\int d^3x\left[\pi^2+\kappa^2(\nabla^2\phi)^2+m^2\phi^2\right].}
$$

The same construction works in any number of spatial dimensions by replacing $d^3x$ appropriately. Under a spatial [Fourier transform](../../../../fourier-transform-split.md), $\nabla^2\phi$ becomes $-|\mathbf p|^2\widetilde\phi$, so the [Hamiltonian](../../../../hamiltonian.md) is a collection of independent [quantum harmonic oscillators](../../../../quantum-harmonic-oscillator-split.md) with squared [angular frequency](../../../../angular-frequency.md) $\omega_{\mathbf p}^2=\kappa^2|\mathbf p|^4+m^2$. The usual reality condition pairs opposite [momenta](../../../../momentum-split.md); it does not introduce a second species.

The canonical [action](../../../../action.md) is $S=\int dt\,[\int d^3x\,\pi\dot\phi-H]$. Varying $\pi$ gives $\pi=\dot\phi$; eliminating it by the [Legendre transform](../../../../convex-conjugate.md) gives

$$
\boxed{S[\phi]=\frac12\int dt\,d^3x\left[(\partial_t\phi)^2-\kappa^2(\nabla^2\phi)^2-m^2\phi^2\right].}
$$

This [Lagrangian density](../../../../lagrangian-density.md) is local: only the field and finitely many derivatives at the same point occur. It contains second spatial derivatives but only first time derivatives, so no extra canonical time data are needed. A square root of a differential operator in the classical [Hamiltonian](../../../../hamiltonian.md) is unnecessary. The fourth-order spatial term breaks [Lorentz invariance](../../../../lorentz-invariance.md) while preserving spatial rotations and translations. This is a [free scalar field with quartic spatial dispersion](../../../../free-scalar-field-with-quartic-spatial-dispersion.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
