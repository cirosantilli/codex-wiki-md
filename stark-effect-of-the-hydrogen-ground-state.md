# Stark effect of the hydrogen ground state

↑ **Parent:** [Stark effect](stark-effect.md)

The even, spherically symmetric [hydrogen atom](hydrogen-atom.md) ground state has no permanent [electric dipole](electric-dipole.md), so a uniform [electric field](electric-field-split.md) gives no first-order energy shift. The [electric-dipole selection rules for hydrogen](electric-dipole-selection-rules-for-hydrogen.md) allow odd-parity excited states to mix in at second order, yielding a negative shift quadratic in the field.

Here there is a [nondegenerate energy eigenvalue](nondegenerate-energy-eigenvalue.md), so [second-order nondegenerate perturbation theory](second-order-nondegenerate-perturbation-theory.md) applies. With $H'=e\mathcal E z$, it gives

$$
\Delta E_{1s}^{(2)}
=e^2\mathcal E^2\sum_{k\ne1s}
\frac{|\langle k|z|1s\rangle|^2}{E_1-E_k}
=-\frac12\alpha_{1s}\mathcal E^2,
\qquad
\alpha_{1s}=\frac92\,4\pi\epsilon_0a_0^3.
$$

The notation includes integration over the [continuous spectrum](continuous-spectrum.md), as well as a sum over discrete [energy eigenstates](energy-eigenstate.md). All denominators are negative because $1s$ is the [ground state](ground-state.md). The positive [electric polarizability](electric-polarizability.md) $\alpha_{1s}$ therefore lowers its [energy](energy-split.md).[Quantum Mechanics by Richard Fitzpatrick; Fitzpatrick, Quadratic Stark Effect, equations (7.57) and (7.65): quadratic convention and exact polarizability](quantum-mechanics-by-richard-fitzpatrick/quadratic-stark-effect.md)

An independent way to see the coefficient avoids truncating that sum. Define $E_{\rm h}=e^2/(4\pi\epsilon_0a_0)$ and $f=ea_0\mathcal E/E_{\rm h}$. In coordinates $\boldsymbol\rho=\mathbf r/a_0$, the dimensionless unperturbed [Hamiltonian operator](hamiltonian-quantum-mechanics.md) and normalized [wavefunction](wave-function-split.md) are $h_0=-\nabla_\rho^2/2-1/\rho$ and $\psi_0=\pi^{-1/2}e^{-\rho}$, with [energy eigenvalue](energy-eigenvalue-split.md) $-1/2$. Writing the first-order [wavefunction](wave-function-split.md) correction as $f\chi$, substitution into the [time-independent Schrödinger equation](time-independent-schrodinger-equation.md) gives

$$
(h_0+1/2)\chi=-\rho\cos\theta\,\psi_0,
\qquad
\chi=-\tfrac12\rho(\rho+2)\cos\theta\,\psi_0.
$$

The second equality can be checked by differentiation. Its [parity](parity.md) makes $\chi$ orthogonal to $\psi_0$. The resulting [integral](integral-split.md) is

$$
\frac{\Delta E_{1s}^{(2)}}{E_{\rm h}}
=f^2\langle\psi_0|\rho\cos\theta|\chi\rangle
=-\frac{f^2}{6}\bigl(\langle\rho^3\rangle_0+2\langle\rho^2\rangle_0\bigr)
=-\frac94 f^2,
$$

since the normalized radial [probability density](probability-density.md) is $4\rho^2e^{-2\rho}$, giving $\langle\rho^2\rangle_0=3$ and $\langle\rho^3\rangle_0=15/2$. Converting back to [SI](international-system-of-units.md) units gives the stated [electric polarizability](electric-polarizability.md). The induced [electric dipole moment](electric-dipole-moment.md) is $-\partial\Delta E/\partial\mathcal E=\alpha_{1s}\mathcal E$ and tends to zero with the [electric field](electric-field-split.md), unlike the selected degenerate branches' leading dipoles. Both calculations describe weak-field level shifts; a spatially uniform static [electric field](electric-field-split.md) also allows eventual [quantum tunnelling](quantum-tunnelling.md) and [ionization](ionization.md), which these real [energy](energy-split.md) corrections do not calculate.

## ↑ Ancestors (4)

1. [Stark effect](stark-effect.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/33a/c/solution.md)
