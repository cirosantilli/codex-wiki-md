<h1 id="section-c/c11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a nonrelativistic spinless particle in a scalar potential, the [Time-dependent Schrödinger equation](../../../../../../time-dependent-schrodinger-equation.md) is

$$
\boxed{i\hbar\frac{\partial\psi}{\partial t}
=\left[-\frac{\hbar^2}{2m}\nabla^2+V(\mathbf r,t)\right]\psi}.
$$

An initial [wavefunction](../../../../../../wave-function-split.md) together with [boundary conditions](../../../../../../boundary-condition.md) specifies the evolution. The [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) must be self-adjoint on the appropriate domain for closed-system evolution to be unitary. The equation is linear, so a superposition of solutions is another solution. Its complex [wavefunction](../../../../../../wave-function-split.md) predicts [probability amplitudes](../../../../../../probability-amplitude.md); the [Born rule](../../../../../../born-rule.md) separately supplies the connection to measurement [probabilities](../../../../../../probability.md).

For a time-independent potential, separation $\psi(\mathbf r,t)=\phi(\mathbf r)e^{-iEt/\hbar}$ gives the [time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) $H\phi=E\phi$. Normalizability and [boundary conditions](../../../../../../boundary-condition.md) select the allowed [energies](../../../../../../energy-split.md) of [bound states](../../../../../../bound-state.md); [scattering states](../../../../../../scattering-state.md) instead use incoming and outgoing [boundary conditions](../../../../../../boundary-condition.md) and generalized normalization. A general state is a superposition of [energy eigenstates](../../../../../../energy-eigenstate.md), with a spectral integral as well if there is a [continuous spectrum](../../../../../../continuous-spectrum.md). Different [energies](../../../../../../energy-split.md) accumulate different phases, allowing time-dependent position densities and oscillatory [expectation values](../../../../../../expectation-value.md) even though a single [energy eigenstate](../../../../../../energy-eigenstate.md) has a stationary density.

For a real scalar potential, combining the equation with its [complex conjugate](../../../../../../complex-conjugate.md) yields [probability](../../../../../../probability.md) conservation:

$$
\partial_t|\psi|^2+\nabla\cdot\mathbf J=0,\qquad
\mathbf J=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi).
$$

With no current escaping the boundary, $\int|\psi|^2\,d^3r$ is constant. Matching conditions at a finite potential step follow from the differential equation and enforce the flux balance used in B6.

The [Schrödinger equation](../../../../../../schrodinger-equation.md) is a dynamical postulate of nonrelativistic [quantum mechanics](../../../../../../quantum-mechanics-split.md), not a consequence of [classical mechanics](../../../../../../classical-mechanics-split.md) alone. The substitutions $E\mapsto i\hbar\partial_t$ and $\mathbf p\mapsto-i\hbar\nabla$ motivate its free-particle form from the [dispersion relation](../../../../../../dispersion-relation-split.md), but do not derive the measurement postulates. The scalar equation omits intrinsic spin and relativistic particle creation. Spinful or relativistic problems require the corresponding extended theory. Nor does its deterministic unitary evolution, by itself, prescribe conditioning on a particular observed measurement outcome.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
