# Quantum harmonic oscillator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_harmonic_oscillator)

The [quantum harmonic oscillator](quantum-harmonic-oscillator.md) describes a particle of [mass](classical-mechanics.md#mass) $m>0$ in a quadratic [potential energy](energy.md#potential-energy) with [angular frequency](lagrangian-mechanics.md#angular-frequency) $\omega>0$. In the position representation its [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) is

$$
H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+\frac{m\omega^2x^2}2.
$$

The model is useful far beyond a literal spring: a [Taylor series](calculus.md#taylor-series) about a stable equilibrium with positive potential curvature has this quadratic term as its leading nonconstant approximation. The pure [quartic oscillator](classical-mechanics.md#quartic-oscillator) has zero curvature at its minimum, so that particular approximation does not apply. [Allan Adams, MIT 8.04 Lecture 8, Quantum Harmonic Oscillator, pp. 3–4](https://ocw.mit.edu/courses/8-04-quantum-physics-i-spring-2013/808334d09369e3a726f6f20d82315c20_MIT8_04S13_Lec08.pdf).

In units with $\hbar=1$, [creation and annihilation operators](#creation-and-annihilation-operators) give

$$
H=\omega\left(N+\frac12\right),
\qquad N=A^\dagger A.
$$

Here $N$ is the [number operator](#number-operator). Restoring the reduced [Planck constant](quantum-mechanics.md#planck-constant), the [energy eigenvalues](energy-eigenvalue.md) are $E_n=\hbar\omega(n+1/2)$ for $n=0,1,2,\ldots$: neighboring levels are separated by $\hbar\omega$, and the [ground-state energy](quantum-mechanics.md#ground-state-energy) is the [zero-point energy](#zero-point-energy) $\hbar\omega/2$.

With length scale $\ell=\sqrt{\hbar/(m\omega)}$ and dimensionless coordinate $u=x/\ell$, the [ground state](quantum-mechanics.md#ground-state) is the normalized [Gaussian wave packet](wave-function.md#gaussian-wave-packet)

$$
\phi_0(x)=\frac1{\pi^{1/4}\sqrt\ell}e^{-u^2/2},\qquad \langle x^2\rangle_0=\frac{\ell^2}2.
$$

For $\hbar=m=\omega=1$, this is precisely the $a=1$ trial [wavefunction](wave-function.md) in the [quantum variational principle](quantum-mechanics.md#quantum-variational-principle). The balance of [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy) therefore recovers the exact [ground-state energy](quantum-mechanics.md#ground-state-energy) using only [Gaussian integrals](integral.md#gaussian-integral).

**Table of contents**

- [Oscillator ground-state density in a comparison wavelength](#oscillator-ground-state-density-in-a-comparison-wavelength)
- [Harmonic-oscillator wavefunction inflections](#harmonic-oscillator-wavefunction-inflections)
- [Oscillator uncertainty and allocation of classical energy](#oscillator-uncertainty-and-allocation-of-classical-energy)
- [Anisotropic quantum harmonic oscillator](#anisotropic-quantum-harmonic-oscillator)
  - [Capacity of an isotropic oscillator shell](#capacity-of-an-isotropic-oscillator-shell)
- [Quantum occupation scale of a classical oscillator](#quantum-occupation-scale-of-a-classical-oscillator)
- [Euclidean oscillator diagonal kernel](#euclidean-oscillator-diagonal-kernel)
- [Canonical oscillator coordinate variance](#canonical-oscillator-coordinate-variance)
- [Ground-state oscillator probability beyond the turning points](#ground-state-oscillator-probability-beyond-the-turning-points)
- [Exact ground state of two coordinate-coupled oscillators](#exact-ground-state-of-two-coordinate-coupled-oscillators)
- [Electric-field displacement of a quantum harmonic oscillator](#electric-field-displacement-of-a-quantum-harmonic-oscillator)
  - [Normalized two-state truncation of a displaced oscillator](#normalized-two-state-truncation-of-a-displaced-oscillator)
- [Uncertainty product of oscillator number states](#uncertainty-product-of-oscillator-number-states)
- [Harmonic oscillator eigenfunction](#harmonic-oscillator-eigenfunction)
- [Sudden oscillator frequency quench](#sudden-oscillator-frequency-quench)
- [Harmonic-oscillator forbidden-region probability](#harmonic-oscillator-forbidden-region-probability)
- [Gaussian variational bound for a radial harmonic oscillator](#gaussian-variational-bound-for-a-radial-harmonic-oscillator)
- [Half-harmonic oscillator](#half-harmonic-oscillator)
  - [Exponential trial state for a half-harmonic oscillator](#exponential-trial-state-for-a-half-harmonic-oscillator)
  - [Removal of a half-oscillator wall](#removal-of-a-half-oscillator-wall)
- [Cartesian and spherical bases of the first oscillator shell](#cartesian-and-spherical-bases-of-the-first-oscillator-shell)
- [Harmonic-oscillator number-state second moments](#harmonic-oscillator-number-state-second-moments)
- [Oscillator length](#oscillator-length)
- [Stability of monomial ladder-operator perturbations](#stability-of-monomial-ladder-operator-perturbations)
- [Harmonic oscillator transition kernel](#harmonic-oscillator-transition-kernel)
- [Minimum-energy normalized oscillator mode](#minimum-energy-normalized-oscillator-mode)
- [One-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain)
  - [Graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator)
    - [Resolvent of the shifted harmonic oscillator](#resolvent-of-the-shifted-harmonic-oscillator)
- [Thermal partition function of a quantum harmonic oscillator](#thermal-partition-function-of-a-quantum-harmonic-oscillator)
  - [Quantum-oscillator energy and heat capacity](#quantum-oscillator-energy-and-heat-capacity)
- [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)
  - [Shaken harmonic trap](#shaken-harmonic-trap)
    - [Weak resonant driving](#weak-resonant-driving)
    - [First-order selection rule for a linearly driven oscillator](#first-order-selection-rule-for-a-linearly-driven-oscillator)
  - [Exponential switch-on of a driven quantum oscillator](#exponential-switch-on-of-a-driven-quantum-oscillator)
  - [Ground-state overlap after sudden oscillator displacement](#ground-state-overlap-after-sudden-oscillator-displacement)
- [Zero-point energy](#zero-point-energy)
  - [Zero-point motion](#zero-point-motion)
- [Squeezed coherent state](#squeezed-coherent-state)
- [Creation and annihilation operators](#creation-and-annihilation-operators)
  - [Annihilation operator](#annihilation-operator)
  - [Creation operator](#creation-operator)
  - [Bosonic creation operator](#bosonic-creation-operator)
  - [Bosonic annihilation operator](#bosonic-annihilation-operator)
  - [Single-mode squeeze operator](#single-mode-squeeze-operator)
    - [Squeezed vacuum state](#squeezed-vacuum-state)
      - [Breathing Gaussian state in a harmonic oscillator](#breathing-gaussian-state-in-a-harmonic-oscillator)
      - [Squeezed one-photon state](#squeezed-one-photon-state)
      - [Optical squeezed vacuum](#optical-squeezed-vacuum)
        - [Photon statistics of a squeezed vacuum](#photon-statistics-of-a-squeezed-vacuum)
          - [Squeezed-vacuum photon-number moments](#squeezed-vacuum-photon-number-moments)
      - [Multimode squeezed vacuum](#multimode-squeezed-vacuum)
        - [Two-mode squeezed vacuum](#two-mode-squeezed-vacuum)
          - [Thermal reduction of a two-mode squeezed vacuum](#thermal-reduction-of-a-two-mode-squeezed-vacuum)
        - [Particle-antiparticle two-mode squeezed vacuum](#particle-antiparticle-two-mode-squeezed-vacuum)
          - [Geometric pair-number distribution](#geometric-pair-number-distribution)
  - [Number operator](#number-operator)
    - [Number-difference shift identity](#number-difference-shift-identity)
    - [Photon number](#photon-number)
    - [Number state](#number-state)
    - [Integer spectrum of the number operator](#integer-spectrum-of-the-number-operator)
- [Two commensurate quantum harmonic oscillators](#two-commensurate-quantum-harmonic-oscillators)

## Oscillator ground-state density in a comparison wavelength

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

A free particle whose [kinetic energy](energy.md#kinetic-energy) equals the ground-state total [energy](energy.md) $\hbar\omega/2$ has [momentum](momentum.md) $\hbar/a$ and [de Broglie wavelength](wave-function.md#de-broglie-wavelength) $\lambda=2\pi a$, where $a=\sqrt{\hbar/(m\omega)}$. Substitution into the normalized bound-state [Gaussian](probability-distribution.md#normal-distribution) yields the title density. The comparison [wavelength](wave-equation.md#wavelength) is a useful [length](physics.md#length) scale; it is not a claim that the [bound state](quantum-system.md#bound-state) has a single free [momentum](momentum.md) or spatially uniform [probability density](wave-function.md#probability-density).

## Harmonic-oscillator wavefunction inflections

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a one-dimensional [quantum harmonic oscillator](quantum-harmonic-oscillator.md), let $b=\sqrt{\hbar/(m\omega)}$ and $\xi=x/b$. The stationary [Schrödinger equation](mathematical-physics.md#schrodinger-equation) gives the displayed curvature relation. Inflections occur at [classical turning points](analysis.md#classical-turning-point) $\xi=\pm\sqrt{2n+1}$ and at simple [wavefunction](wave-function.md) [wavefunction nodes](wave-equation.md#wavefunction-node), provided the curvature changes sign. Thus the first excited state has an inflection at its central [wavefunction node](wave-equation.md#wavefunction-node) as well as at both turning points. Restricting attention to where $V=E$ misses [wavefunction node](wave-equation.md#wavefunction-node) inflections.

## Oscillator uncertainty and allocation of classical energy

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a one-dimensional oscillator eigenstate, [parity](quantum-mechanics.md#parity) gives $\langle x\rangle=0$ and its coordinate [variance](variance.md) is the displayed expression. A classical oscillator with that coordinate [energy](energy.md) has turning amplitude $A=\sqrt{2E_x/(m\omega^2)}$, so $\Delta x=A/\sqrt2$. In several dimensions the total [energy](energy.md) does not specify a given coordinate's classical amplitude until its [energy](energy.md) allocation is fixed. [zero-point energies](#zero-point-energy) in the other quantum coordinates must not silently be assigned to that one classical mode.

## Anisotropic quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a positive diagonal quadratic potential $V=m\sum_i\omega_i^2x_i^2/2$, coordinate [Hamiltonians](hamiltonian-mechanics.md#hamiltonian) commute and [wavefunctions](wave-function.md) separate into one-dimensional oscillator factors. Equality of two squared [frequencies](wave.md#frequency) gives [rotation](riemannian-geometry.md#rotation-mathematics) [symmetry](physics.md#symmetry-physics) in their plane; equality of all three gives full [rotation](riemannian-geometry.md#rotation-mathematics) [symmetry](physics.md#symmetry-physics). Equalities create [energy](energy.md) degeneracies and extra conserved [angular momentum](momentum.md#angular-momentum). Merely finding an accidental equality between particular level energies does not establish a global [rotational symmetry](linear-algebra.md#rotational-symmetry).

### Capacity of an isotropic oscillator shell

↑ **Parent:** [Anisotropic quantum harmonic oscillator](#anisotropic-quantum-harmonic-oscillator)

The number of nonnegative triples with $n_x+n_y+n_z=N$ is the stars-and-bars count $\binom{N+2}{2}$. Including a two-state [electron](physics.md#electron) [spin](angular-momentum-operator.md#spin) gives capacity $(N+1)(N+2)$. Filling non-interacting shells therefore uses capacities $2,6,12,\ldots$, with shell [energy](energy.md) $(N+3/2)\hbar\omega$ per [electron](physics.md#electron). A partly filled shell has degenerate many-body [ground states](quantum-mechanics.md#ground-state); rearranging its occupants is not a positive excitation [energy](energy.md).

## Quantum occupation scale of a classical oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

A classical oscillator of amplitude $A$ has [energy](energy.md) $m\omega^2A^2/2$. Comparing with the oscillator spacing $\hbar\omega$ gives the large-occupation scale displayed. A [coherent state](quantum-theory.md#coherent-state) with this classical amplitude has exactly this [mean](expected-value.md) excitation occupation and a Poisson number distribution; its total [mean](expected-value.md) [energy](energy.md) also includes the zero-point term. An observed macroscopic amplitude does not, by itself, establish a pure [coherent state](quantum-theory.md#coherent-state).

## Euclidean oscillator diagonal kernel

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

At imaginary duration $\beta\hbar$, $K_E(q,q)=\sqrt{m\omega/[2\pi\hbar\sinh x]}\exp[-m\omega q^2\tanh(x/2)/\hbar]$, $x=\beta\hbar\omega$. Integrating the common endpoint yields $[2\sinh(x/2)]^{-1}$.

## Canonical oscillator coordinate variance

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

A canonical [quantum harmonic oscillator](quantum-harmonic-oscillator.md) has geometric number probabilities and mean occupation $(e^{\beta\hbar\omega}-1)^{-1}$. The position operator then gives the displayed variance. It interpolates between zero-point fluctuations $\hbar/(2m\omega)$ and the classical variance $k_BT/(m\omega^2)$. The kinetic and potential [energies](energy.md) are equal at every [temperature](temperature.md), although classical equipartition describes their values only at high [temperature](temperature.md).

## Ground-state oscillator probability beyond the turning points

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

The ground-state turning points are $\pm\sqrt{\hbar/(m\omega)}$. In dimensionless position $y=x\sqrt{m\omega/\hbar}$, the [probability](probability-theory.md#probability) outside them is $(2/\sqrt\pi)\int_1^\infty e^{-y^2}\,dy=\operatorname{erfc}(1)\simeq0.15730$. This tail demonstrates that a bound quantum state need not be confined to its classically allowed region.

## Exact ground state of two coordinate-coupled oscillators

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For identical [masses](classical-mechanics.md#mass) and bare [frequencies](wave.md#frequency) with coupling $kxy$, coordinates $(x\pm y)/\sqrt2$ diagonalize the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). A stable normalizable [ground state](quantum-mechanics.md#ground-state) requires $|k|<m\omega^2$. Its wave function is the product of Gaussians of [frequencies](wave.md#frequency) $\omega_\pm$ in these [normal coordinates](general-relativity.md#normal-coordinates); a two-mode squeeze of the original bare oscillators alone is generally insufficient.

## Electric-field displacement of a quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For $H=p^2/(2m)+kx^2/2-qEx$, completing the square translates the well by $x_0=qE/k$ and shifts every [energy](energy.md) by $-q^2E^2/(2k)$. The [wavefunction](wave-function.md) of the [ground state](quantum-mechanics.md#ground-state) is translated without changing its width. Consequently the induced [electric dipole moment](electrostatics.md#electric-dipole-moment) is exactly linear in $E$, even when a low-order perturbative approximation to the state is inaccurate.

### Normalized two-state truncation of a displaced oscillator

↑ **Parent:** [Electric-field displacement of a quantum harmonic oscillator](#electric-field-displacement-of-a-quantum-harmonic-oscillator)

Let $x_{\rm zp}=\sqrt{\hbar/(2m\omega)}$ and $\eta=x_0/(2x_{\rm zp})$. The normalized first-order truncation is $(|0\rangle+\eta|1\rangle)/\sqrt{1+\eta^2}$. Its mean displacement is $2\eta x_{\rm zp}/(1+\eta^2)$, agreeing with $x_0$ only at small $|\eta|$. The exact translated [ground state](quantum-mechanics.md#ground-state) is a [coherent state](quantum-theory.md#coherent-state) whose expansion contains all [number states](#number-state) and has mean occupation $\eta^2$. Correct linear response does not justify extrapolating a truncated state to large fields.

## Uncertainty product of oscillator number states

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

An [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) has $\langle x\rangle=\langle p\rangle=0$, $\langle x^2\rangle=\hbar(n+1/2)/(m\omega)$ and $\langle p^2\rangle=m\hbar\omega(n+1/2)$. Thus $\Delta x\Delta p=\hbar(n+1/2)$; only the ground state in this sequence minimizes the [Heisenberg uncertainty principle](quantum-theory.md#heisenberg-uncertainty-relation).

## Harmonic oscillator eigenfunction

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

With oscillator length $\ell=\sqrt{\hbar/(m\omega)}$, the eigenfunctions are proportional to $H_n(x/\ell)e^{-x^2/(2\ell^2)}$. They have $n$ real nodes, [parity](quantum-mechanics.md#parity) $(-1)^n$, and energy $\hbar\omega(n+1/2)$.

## Sudden oscillator frequency quench

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

A jump from [positive frequency](quantum-field-theory.md#positive-frequency-solution) $\omega$ to $\Omega$ keeps an oscillator mode and its first derivative continuous. A normalized positive-frequency incident solution has outgoing coefficients $\alpha=(\Omega+\omega)/(2\sqrt{\Omega\omega})$ and $\beta=(\Omega-\omega)/(2\sqrt{\Omega\omega})$, satisfying $\alpha^2-\beta^2=1$. This temporal matching is not a sum-one spatial-scattering [probability](probability-theory.md#probability) rule.

## Harmonic-oscillator forbidden-region probability

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For the normalized ground state of a reduced [quantum harmonic oscillator](quantum-harmonic-oscillator.md), $\phi_0(q)=\pi^{-1/4}e^{-q^2/2}$ and $E_0=1/2$. Its [classical turning points](analysis.md#classical-turning-point) are $q=\pm1$. The [Born rule](wave-function.md#born-rule) assigns [probability](probability-theory.md#probability) $P=2\pi^{-1/2}\int_1^\infty e^{-q^2}\,dq=\operatorname{erfc}(1)\simeq0.157299$ to the [classically forbidden region](mathematical-physics.md#classically-forbidden-region). This is a stationary [probability](probability-theory.md#probability) of detection outside the classical interval. It is not a transmitted flux or an escape rate: the real stationary [wavefunction](wave-function.md) has zero [probability current](wave-function.md#probability-current).

## Gaussian variational bound for a radial harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

Consider $-y''-(n-1)y'/x+x^2y=\lambda y$ for a positive [integer](integer.md) $n$, with regular radial data at zero and square-integrable decay at infinity in the measure $x^{n-1}dx$. Its [Sturm-Liouville form](sturm-liouville-theory.md#sturm-liouville-form) has $p=w=x^{n-1}$ and $q=x^{n+1}$. For the Gaussian trial $y=e^{ax^2}$, $a<0$, the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is

$$
\Lambda(a)=(4a^2+1)\frac{\int_0^\infty x^{n+1}e^{2ax^2}dx}{\int_0^\infty x^{n-1}e^{2ax^2}dx}=-n\left(a+\frac1{4a}\right).
$$

The [Gamma function recurrence](complex-analysis.md#gamma-function-recurrence) evaluates the ratio, and the minimum is $n$ at $a=-1/2$. It is the exact lowest [eigenvalue](linear-operator-theory.md#eigenvalue): after the endpoint term $[x^ny^2]_0^\infty$ vanishes, [integration by parts](calculus.md#integration-by-parts) gives

$$
\int_0^\infty\left[x^{n-1}(y')^2+x^{n+1}y^2\right]dx-n\int_0^\infty x^{n-1}y^2dx=\int_0^\infty x^{n-1}(y'+xy)^2dx\geq0.
$$

Equality gives the displayed positive Gaussian [eigenfunction](linear-operator-theory.md#eigenfunction). For $n=1$, the radial regularity condition is the [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) at zero, not a vanishing value there. Changing the boundary condition changes the lowest [eigenvalue](linear-operator-theory.md#eigenvalue) and whether this trial is admissible.

## Half-harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

A [half-harmonic oscillator](#half-harmonic-oscillator) has $V=m\omega^2x^2/2$ on $x>0$ and an infinite wall at $x=0$. Its [wavefunction](wave-function.md) vanishes at the wall. Only the odd full-oscillator [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) satisfy this condition; restricting them to the positive half-line and multiplying by $\sqrt2$ restores normalization. Thus $E_r=\hbar\omega(2r+3/2)$ for $r=0,1,\ldots$. With $\ell=\sqrt{\hbar/(m\omega)}$, its normalized [ground state](quantum-mechanics.md#ground-state) is

$$
\psi_h(x)=\frac{2x}{\pi^{1/4}\ell^{3/2}}e^{-x^2/(2\ell^2)}\quad(x>0),\qquad \psi_h(x)=0\quad(x<0).
$$

It has no interior node on its allowed half-line, and energy $3\hbar\omega/2$.

### Exponential trial state for a half-harmonic oscillator

↑ **Parent:** [Half-harmonic oscillator](#half-harmonic-oscillator)

For the dimensionless [half-harmonic oscillator](#half-harmonic-oscillator) $-\psi''+x^2\psi=\lambda\psi$ on $x>0$ with $\psi(0)=0$, the trial family $xe^{-\alpha x}$, $\alpha>0$, is admissible for the [Rayleigh-Ritz variational principle](linear-operator-theory.md#rayleigh-ritz-variational-principle). The moments $\int_0^\infty x^ne^{-2\alpha x}dx=n!/(2\alpha)^{n+1}$ give norm squared $1/(4\alpha^3)$, derivative energy $1/(4\alpha)$, and potential energy $3/(4\alpha^5)$. Its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is $\alpha^2+3/\alpha^2$, minimized at $\alpha=3^{1/4}$. The resulting upper bound $2\sqrt3$ exceeds the exact lowest eigenvalue three; the exact ground-state shape is $xe^{-x^2/2}$.

### Removal of a half-oscillator wall

↑ **Parent:** [Half-harmonic oscillator](#half-harmonic-oscillator)

Suddenly remove the wall of a [half-harmonic oscillator](#half-harmonic-oscillator) in its ground state, leaving the same harmonic potential on the whole line. The [sudden approximation](quantum-mechanics.md#sudden-approximation) keeps its wavefunction unchanged during removal. The new normalized ground state is $\psi_0=\pi^{-1/4}\ell^{-1/2}e^{-x^2/(2\ell^2)}$, so

$$
\langle0|\psi_h\rangle=\frac{2}{\sqrt\pi\ell^2}\int_0^\infty xe^{-x^2/\ell^2}\,dx=\frac1{\sqrt\pi},\qquad \boxed{P_0=\frac1\pi.}
$$

The integration is over the initially occupied half-line. The final first excited state instead has probability $1/2$, since the initial half-line state equals $\sqrt2$ times its positive-half restriction. This also checks that removing the wall does not simply create the full oscillator's odd state.

## Cartesian and spherical bases of the first oscillator shell

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

In the isotropic three-dimensional [quantum harmonic oscillator](quantum-harmonic-oscillator.md), the first excited Cartesian [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) are proportional to $x,y,z$ times the common Gaussian $e^{-r^2/(2a_0^2)}$. If $\phi_x,\phi_y,\phi_z$ are normalized with the same real phase convention, their combinations in the title are normalized [angular momentum eigenstates](angular-momentum-operator.md#angular-momentum-eigenstate) with $l=1$ and $m=1,0,-1$.

Indeed, $z=r\cos\theta$ and $x\pm iy=r\sin\theta e^{\pm i\varphi}$ identify a common radial factor times the [spherical harmonics](analysis.md#spherical-harmonic) $Y_{10},Y_{1,\pm1}$. The transformation is unitary, so it changes the basis rather than the threefold orbital degeneracy.

## Harmonic-oscillator number-state second moments

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a [number operator](#number-operator) [eigenstate](energy-eigenvalue.md#eigenstate) $|n\rangle$, the [annihilation operator](#annihilation-operator) and [creation operator](#creation-operator) satisfy $\langle a\rangle=\langle a^\dagger\rangle=\langle a^2\rangle=\langle(a^\dagger)^2\rangle=0$, $\langle a^\dagger a\rangle=n$ and $\langle aa^\dagger\rangle=n+1$. Inserting $x=\sqrt{\hbar/(2m\omega)}(a+a^\dagger)$ and $p=i\sqrt{m\hbar\omega/2}(a^\dagger-a)$ gives the displayed second moments and zero means.

Thus the [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy) each have mean $\hbar\omega(n+1/2)/2$, and the uncertainty product is $\Delta x\Delta p=\hbar(n+1/2)$. Among number states only the ground state saturates the [Heisenberg uncertainty relation](quantum-theory.md#heisenberg-uncertainty-relation). A [quantum superposition](quantum-system.md#quantum-superposition) can have nonzero position and momentum means despite each constituent number state's zero means.

## Oscillator length

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

The oscillator length fixes the spatial scale of a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) of mass $m$ and angular frequency $\omega$. Its normalized ground [wavefunction](wave-function.md) is $\varphi_0(x)=\pi^{-1/4}\ell^{-1/2}\exp[-x^2/(2\ell^2)]$, so $|\varphi_0(0)|^2=1/(\sqrt\pi\ell)$ and $\langle x^2\rangle=\ell^2/2$. The definition of $\ell$ is distinct from the root-mean-square displacement $\ell/\sqrt2$.

## Stability of monomial ladder-operator perturbations

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

The perturbation $\lambda\hbar\omega(a^r+(a^\dagger)^r)$ couples the oscillator vacuum only to $|r\rangle$ at first order. Its squared coupling is $(\hbar\omega)^2r!$ and the [energy](energy.md) denominator is $-r\hbar\omega$, giving the displayed formal second-order coefficient. For $r>2$ and nonzero real $\lambda$, coherent-state expectations contain $R^2+2\lambda R^r\cos r\theta$; choosing its phase negative proves the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) is unbounded below. The formal vacuum branch must therefore not be called an exact ground state. For $r=2$ boundedness requires $|\lambda|<1/2$, while the displaced $r=1$ oscillator is stable for every real strength.

## Harmonic oscillator transition kernel

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For [action](lagrangian-mechanics.md#action) $\frac m2\int(\dot q^2-\omega^2q^2)dt$, the kernel is $\sqrt{m\omega/(2\pi i\sin\omega T)}\exp\{im\omega[(q_f^2+q_i^2)\cos\omega T-2q_fq_i]/(2\sin\omega T)\}$. The [Dirichlet oscillator determinant ratio](quantum-field-theory.md#dirichlet-oscillator-determinant-ratio) supplies its prefactor, while the classical boundary [action](lagrangian-mechanics.md#action) supplies its exponent. The [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription) specifies its continuation through caustics.

## Minimum-energy normalized oscillator mode

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) with $\omega>0$, a complex mode satisfying the [Wronskian normalization](quantum-field-theory.md#wronskian-normalization) $q\dot q^*-\dot q q^*=i$ can be written $q=re^{is}$ with $\dot s=-1/(2r^2)$. Its [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) is $\dot r^2/2+1/(8r^2)+\omega^2r^2/2$. This is at least $\omega/2$, with equality exactly when $\dot r=0$ and $r^2=1/(2\omega)$. The same argument fixes the subhorizon positive-frequency normalization in the [Bunch-Davies vacuum](cosmic-inflation.md#bunch-davies-vacuum) of a canonical cosmological mode.

## One-dimensional harmonic oscillator form domain

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

This [Hilbert space](hilbert-space.md) has norm $\|u\|_X^2=\|u\|_2^2+\|u'\|_2^2+\|xu\|_2^2$. Completeness follows from completeness of [H1 space](sobolev-space.md#h1-space) and closedness of the [multiplication operator](vector-space.md#multiplication-operator) $u\mapsto xu$. Smooth cutoffs followed by convolution with a [mollifier](distribution-theory.md#mollifier) show that smooth compactly supported functions are dense. The space is the natural energy domain of the dimensionless [quantum harmonic oscillator](quantum-harmonic-oscillator.md), whereas the operator domain additionally requires $u''$ and $x^2u$ to lie in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space).

### Graph estimate for the harmonic oscillator

↑ **Parent:** [One-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain)

For $c>0$ and smooth compactly supported $u$, [integration by parts](calculus.md#integration-by-parts) gives

$$
\|-u''+(c+x^2)u\|_2^2
=\|u''\|_2^2+\|(c+x^2)u\|_2^2+2\int(c+x^2)|u'|^2\,dx-2\|u\|_2^2.
$$

Dropping the nonnegative weighted derivative term proves the displayed bound. For a weak resolvent solution in the [one-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain), apply the bound to $\chi_Ru$, where $\chi_R$ is a smooth cutoff. The cutoff error $-2\chi_R'u'-\chi_R''u$ is bounded in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) and tends to zero. The [Fatou lemma](measure-theory.md#fatou-s-lemma) then shows that $u''$ and $x^2u$ belong to [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), identifying the strong operator domain.

#### Resolvent of the shifted harmonic oscillator

↑ **Parent:** [Graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator)

For $Au=u''-(1+x^2)u$ on $D(A)=\{u\in H^2(\mathbb R):x^2u\in L^2\}$, the form $a_\lambda(u,v)=\int u'\overline{v'}+(1+\lambda+x^2)u\bar v$ is coercive on the [one-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain) when $\lambda>0$. The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique weak solution of $(\lambda-A)u=g$. The [graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator) puts it in $D(A)$, and $a_\lambda(u,u)\geq(1+\lambda)\|u\|_2^2$ gives the displayed [resolvent](functional-analysis.md#resolvent-of-an-operator) bound. The domain is dense and the bounded resolvent proves closedness, so the [Hille-Yosida theorem](functional-analysis.md#hille-yosida-theorem) gives a [contraction semigroup](functional-analysis.md#contraction-semigroup). An [exponentially shifted semigroup](functional-analysis.md#exponentially-shifted-semigroup) with generator $A+I$ solves the heat equation with oscillator potential.

## Thermal partition function of a quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) with $\hbar=1$, $\omega>0$ and [inverse temperature](temperature.md#inverse-temperature) $\beta>0$, the [canonical partition function](canonical-ensemble.md#canonical-partition-function) is $\sum_{r\ge0}e^{-\beta\omega(r+1/2)}$. The [geometric series](sequence-and-series.md#geometric-series) gives the displayed formula. Keeping the [zero-point energy](#zero-point-energy) is essential to its prefactor.

### Quantum-oscillator energy and heat capacity

↑ **Parent:** [Thermal partition function of a quantum harmonic oscillator](#thermal-partition-function-of-a-quantum-harmonic-oscillator)

For one [quantum harmonic oscillator](quantum-harmonic-oscillator.md) of [frequency](wave.md#frequency) $\Omega$, $Z=e^{-x/2}/(1-e^{-x})$ with $x=\hbar\Omega/(k_BT)$. Differentiating $\ln Z$ gives $U=\hbar\Omega[1/2+1/(e^x-1)]$ and $C_V=k_Bx^2e^x/(e^x-1)^2$. [Zero-point energy](#zero-point-energy) leaves $U\to\hbar\Omega/2$ as $T\to0$ but contributes no [heat capacity](heat.md#heat-capacity). Excitation freeze-out makes $C_V$ exponentially small, while high [temperature](temperature.md) gives $U\sim k_BT$ and $C_V\to k_B$.

## Displaced quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

Adding $-Fx$ to the [quantum harmonic oscillator](quantum-harmonic-oscillator.md) potential gives $\frac12m\omega^2(x-d)^2-F^2/(2m\omega^2)$, where $d=F/(m\omega^2)$. Translation preserves the oscillator spectrum, apart from the displayed constant shift. Eigenfunctions are translated by $d$ and the energy spacing is unchanged.

### Shaken harmonic trap

↑ **Parent:** [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)

Displacing a one-dimensional [quantum harmonic oscillator](quantum-harmonic-oscillator.md) produces a linear force term and a scalar shift relative to the unshifted [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). The scalar adds only a common phase. The linear term couples [number states](#number-state) separated by one excitation. Arbitrary linear driving of the [ground state](quantum-mechanics.md#ground-state) creates a [coherent state](quantum-theory.md#coherent-state); a first-order expansion of that state contains only the vacuum and first excited state.[§4.4.2, printed pp.132–133: a forcing term creates coherent states](physics-bibliography.md#topics-in-quantum-mechanics-by-david-tong)

#### Weak resonant driving

↑ **Parent:** [Shaken harmonic trap](#shaken-harmonic-trap)

A sinusoidal trap displacement with amplitude $\varepsilon$ and duration $T$ produces a resonant first-order excitation amplitude proportional to $\varepsilon\omega T/a_0$, where $a_0$ is the [oscillator length](#oscillator-length). Keeping its square much smaller than one is the long-time condition for weak excitation. The small-displacement condition $\varepsilon/a_0\ll1$ alone does not ensure uniform validity as $T$ grows. Exact linear driving remains solvable as a [coherent state](quantum-theory.md#coherent-state) after this first-order approximation fails.

#### First-order selection rule for a linearly driven oscillator

↑ **Parent:** [Shaken harmonic trap](#shaken-harmonic-trap)

The ladder identity $x=\sqrt{\hbar/(2m\omega)}(a+a^\dagger)$ proves the matrix element in the title. In [time-dependent perturbation theory](quantum-mechanics.md#time-dependent-perturbation-theory), a linear force excites only $n=1$ directly from $n=0$. [Parity](quantum-mechanics.md#parity) alone rules out even excited states; the ladder identity also rules out odd $n>1$. Higher-order evolution can reach other levels, so the driven oscillator is not an exact [two-level system](canonical-ensemble.md#two-level-system).

### Exponential switch-on of a driven quantum oscillator

↑ **Parent:** [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)

For $H(t)=\hbar\omega(a^\dagger a+1/2)-Fx e^{t/\tau}$ on $t\leq0$, start in the unforced [ground state](quantum-mechanics.md#ground-state) at $t=-\infty$. Define $x_{01}=\sqrt{\hbar/(2m\omega)}$ and $\eta=Fx_{01}/(\hbar\omega)$. [Time-dependent perturbation theory](quantum-mechanics.md#time-dependent-perturbation-theory) gives

$$
c_1(0)=\frac{iFx_{01}}\hbar\int_{-\infty}^0 e^{(1/\tau+i\omega)t}\,dt=\frac{i\eta\omega\tau}{1+i\omega\tau}.
$$

Thus the first excited-state probability in the original oscillator basis tends to zero for a rapid turn-on and to $\eta^2$ for slow turn-on, within the weak-force approximation $|\eta|\ll1$.

This finite adiabatic limit is not a failure of the [adiabatic theorem](quantum-theory.md#adiabatic-theorem): the instantaneous [ground state](quantum-mechanics.md#ground-state) is displaced and has a nonzero projection onto the original excited states. In fact a linear force preserves a [coherent state](quantum-theory.md#coherent-state), whose exact original-basis displacement at $t=0$ is $\alpha=i\eta\omega\tau/(1+i\omega\tau)$. It follows either from $\dot\alpha=-i\omega\alpha+iFx_{01}e^{t/\tau}/\hbar$ or from the forced oscillator equations. Consequently the exact original-basis probability is $P_1^{(0)}=|\alpha|^2e^{-|\alpha|^2}$. The instantaneous oscillator basis has displacement $\eta$, so its mean excitation is instead $|\alpha-\eta|^2=\eta^2/[1+(\omega\tau)^2]$, which vanishes adiabatically.

### Ground-state overlap after sudden oscillator displacement

↑ **Parent:** [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)

In the [sudden approximation](quantum-mechanics.md#sudden-approximation), an initial oscillator [ground state](quantum-mechanics.md#ground-state) overlaps the displaced ground state by $\exp[-m\omega d^2/(4\hbar)]$. Completing the square in the product of the two normalized Gaussian wavefunctions and using the [Gaussian integral](integral.md#gaussian-integral) proves this amplitude. Squaring it gives the displayed probability. Only an irrelevant overall phase evolves before the sudden switch.

## Zero-point energy

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero-point_energy)

Zero-point energy is the nonzero ground-state energy left by quantum fluctuations. One harmonic oscillator contributes $\omega/2$ before any regularization or normal-ordering subtraction.

### Zero-point motion

↑ **Parent:** [Zero-point energy](#zero-point-energy)

[Zero-point motion](#zero-point-motion) is the nonzero quantum fluctuation of position and momentum in a system's [ground state](quantum-mechanics.md#ground-state). For a [quantum harmonic oscillator](quantum-harmonic-oscillator.md), the [ground state](quantum-mechanics.md#ground-state) has [energy](energy.md) $\hbar\omega/2$ and nonzero position and momentum variances even at zero [temperature](temperature.md). It does not represent a thermal mixture and need not carry [entropy](entropy.md). The large [zero-point motion](#zero-point-motion) of light [helium](chemical-substance.md#helium) atoms helps explain why [helium](chemical-substance.md#helium) can remain a [liquid](thermodynamics.md#liquid) at low [pressure](pressure.md) even as [temperature](temperature.md) approaches [absolute zero](temperature.md#absolute-zero).

## Squeezed coherent state

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squeezed_coherent_state)

A [squeezed coherent state](#squeezed-coherent-state) is obtained from the vacuum by a squeeze operator and a displacement operator. Its quadrature variances can differ while saturating the uncertainty product. With zero displacement it is a [squeezed vacuum state](#squeezed-vacuum-state).

## Creation and annihilation operators

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Creation_and_annihilation_operators)

The bosonic ladder operators satisfy

$$
[A,A^\dagger]=1,
\qquad
A|n\rangle=\sqrt n\,|n-1\rangle,
\qquad
A^\dagger|n\rangle=\sqrt{n+1}\,|n+1\rangle.
$$

### Annihilation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

An annihilation operator lowers the occupation [number operator](#number-operator) eigenvalue by one and annihilates the [Fock vacuum](quantum-field-theory.md#fock-vacuum).

### Creation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

A creation operator raises the occupation [number operator](#number-operator) eigenvalue of a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) by one. Repeated application builds [Fock states](quantum-field-theory.md#fock-state).

### Bosonic creation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

### Bosonic annihilation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

### Single-mode squeeze operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

For a real squeezing parameter $\gamma$, the single-mode squeeze operator is

$$
S(\gamma)=\exp\left[-\frac\gamma2\left(A^{\dagger2}-A^2\right)\right].
$$

Its exponent is [skew-adjoint](functional-analysis.md#skew-adjoint-generator), so $S(\gamma)$ is a [unitary operator](vector-space.md#unitary-operator), and it implements the [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation)

$$
S^\dagger AS=A\cosh\gamma-A^\dagger\sinh\gamma.
$$

#### Squeezed vacuum state

↑ **Parent:** [Single-mode squeeze operator](#single-mode-squeeze-operator)

The squeezed vacuum is the zero-displacement [squeezed coherent state](#squeezed-coherent-state) $|\gamma\rangle=S(\gamma)|0\rangle$. Its position and momentum variances are rescaled in opposite directions,

$$
(\Delta X)^2=\frac{\hbar}{2m\omega}e^{-2\gamma},
\qquad
(\Delta P)^2=\frac{m\hbar\omega}{2}e^{2\gamma},
$$

so it remains an [minimum-uncertainty state](quantum-theory.md#equality-case-of-the-heisenberg-uncertainty-relation) with $\Delta X\Delta P=\hbar/2$.

##### Breathing Gaussian state in a harmonic oscillator

↑ **Parent:** [Squeezed vacuum state](#squeezed-vacuum-state)

A real centered [Gaussian wave packet](wave-function.md#gaussian-wave-packet) with initial [position](classical-mechanics.md#position) [variance](variance.md) $1/(2\alpha)$ and [momentum](momentum.md) [variance](variance.md) $\hbar^2\alpha/2$ evolves under a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) by

$$
M(t)=\begin{pmatrix}\cos\omega t&\sin\omega t/(m\omega)\\
-m\omega\sin\omega t&\cos\omega t\end{pmatrix}.
$$

The [covariance matrix](variance.md#covariance-matrix) obeys $\Sigma(t)=M\Sigma(0)M^{\mathsf T}$ and $\det\Sigma=\hbar^2/4$. Thus the [Robertson-Schrödinger uncertainty relation](quantum-theory.md#robertson-schrodinger-uncertainty-relation) stays saturated, although the position-momentum [variance](variance.md) product can exceed $\hbar^2/4$ because of nonzero [quantum covariance](quantum-theory.md#quantum-covariance). The widths are stationary only for $\alpha=m\omega/\hbar$; otherwise they breathe with [frequency](wave.md#frequency) $2\omega$.

##### Squeezed one-photon state

↑ **Parent:** [Squeezed vacuum state](#squeezed-vacuum-state)

[photon addition](quantum-optics.md#photon-addition) to an [optical squeezed vacuum](#optical-squeezed-vacuum) gives $a^\dagger S|0\rangle=\cosh r\,S|1\rangle$; subtraction gives $aS|0\rangle=-\sinh r\,S|1\rangle$. After successful-event normalization these are the same state up to phase, with mean occupation $1+3\sinh^2r$ and odd [photon](quantum-mechanics.md#photon) parity. At zero squeezing subtraction never succeeds; the normalized limiting state is not an output at that exact parameter value.

##### Optical squeezed vacuum

↑ **Parent:** [Squeezed vacuum state](#squeezed-vacuum-state)

A single optical mode in a [squeezed vacuum state](#squeezed-vacuum-state). In principal [optical quadratures](quantum-optics.md#optical-quadrature), its variances are $e^{-2r}/4$ and $e^{2r}/4$, while its mean [photon](quantum-mechanics.md#photon) number is $\sinh^2r$. Its mean field vanishes. A degenerate [optical parametric amplifier](optics.md#optical-parametric-amplifier) generates the state by pair creation with phase fixed by the pump. Loss admixes unsqueezed vacuum and limits the measured variance reduction.

###### Photon statistics of a squeezed vacuum

↑ **Parent:** [Optical squeezed vacuum](#optical-squeezed-vacuum)

The [single-mode squeeze operator](#single-mode-squeeze-operator) changes occupation in pairs. Consequently an [optical squeezed vacuum](#optical-squeezed-vacuum) has only even [photon numbers](#photon-number), with mean $s=\sinh^2r$ and [variance](variance.md) $2s(s+1)$. Its large number fluctuations are compatible with [quadrature squeezing](quantum-optics.md#quadrature-squeezing): they concern different observables.

###### Squeezed-vacuum photon-number moments

↑ **Parent:** [Photon statistics of a squeezed vacuum](#photon-statistics-of-a-squeezed-vacuum)

Here $s=\sinh^2r$. The pair moment is $\langle N(N-1)\rangle=3s^2+s$. These expressions follow from the single-mode [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation) or by differentiating the even-occupation [probability](probability-theory.md#probability) generating function $G(t)=[\cosh r\sqrt{1-t^2\tanh^2r}]^{-1}$.

##### Multimode squeezed vacuum

↑ **Parent:** [Squeezed vacuum state](#squeezed-vacuum-state)

For an invertible finite-mode [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation) $a=Aa'+Ba'{}^\dagger$, the symmetric squeezing matrix is $M=-A^{-1}B$. The [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) make its singular values strictly less than one. The normalized state has $|C|=\det(I-MM^\dagger)^{1/4}$. Infinitely many modes additionally require [bosonic mode mixing implementability](quantum-field-theory.md#bosonic-mode-mixing-implementability).

###### Two-mode squeezed vacuum

↑ **Parent:** [Multimode squeezed vacuum](#multimode-squeezed-vacuum)

Pair creation in two bosonic modes gives the normalized state displayed. The two occupations coincide in each term, while either mode alone has a geometric number distribution. At small $r$, the leading nonvacuum term is a single pair. This optical construction does not require particle-antiparticle modes.

###### Thermal reduction of a two-mode squeezed vacuum

↑ **Parent:** [Two-mode squeezed vacuum](#two-mode-squeezed-vacuum)

Tracing out one mode leaves geometric occupation [probabilities](probability-theory.md#probability) with $q=|\lambda|^2$. In an oscillator basis of [frequency](wave.md#frequency) $\omega$, they are [Boltzmann weights](canonical-ensemble.md#boltzmann-factor) with $k_BT=\hbar\omega/\ln(1/q)$. The joint state can be pure while each reduced state is mixed.

###### Particle-antiparticle two-mode squeezed vacuum

↑ **Parent:** [Multimode squeezed vacuum](#multimode-squeezed-vacuum)

For a pair of distinct bosonic [particle](physics.md#particle-physics) and [antiparticle](relativistic-quantum-field.md#antiparticle) modes, the normalized state obeying $(a+qb^\dagger)|\psi\rangle=(b+qa^\dagger)|\psi\rangle=0$ is $\sqrt{1-|q|^2}\sum_{n\geq0}(-q)^n|n,n\rangle$, for $|q|<1$. It contains equal occupations and is generated by a pair-creation exponential. Infinite products require a separate implementability or regulator check.

###### Geometric pair-number distribution

↑ **Parent:** [Particle-antiparticle two-mode squeezed vacuum](#particle-antiparticle-two-mode-squeezed-vacuum)

The pair count of a two-mode squeezed [vacuum](physics.md#vacuum) has $P(n)=(1-r)r^n$, where $r=|q|^2<1$. Its mean is $r/(1-r)$ and its [variance](variance.md) is $r/(1-r)^2$. Equal mode occupations follow from pair creation, not from independent [particle](physics.md#particle-physics) and [antiparticle](relativistic-quantum-field.md#antiparticle) draws.

### Number operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Number_operator)

The number operator $N=A^\dagger A$ satisfies

$$
[N,A]=-A,
\qquad
[N,A^\dagger]=A^\dagger.
$$

It is self-adjoint and positive semidefinite.

#### Number-difference shift identity

↑ **Parent:** [Number operator](#number-operator)

For a hopping operator $X$ with $[\Delta,X]=2X$, spectral functions obey $Xf(\Delta)=f(\Delta-2)X$. The coefficient on the left of the hop is evaluated on the final state. This ordering determines the shifted energy denominator in virtual-hopping calculations.

#### Photon number

↑ **Parent:** [Number operator](#number-operator)

For a single [electromagnetic field](electromagnetism.md#electromagnetic-field) mode, the [eigenvalues](linear-operator-theory.md#eigenvalue) of the [number operator](#number-operator) count its [photons](quantum-mechanics.md#photon).

#### Number state

↑ **Parent:** [Number operator](#number-operator)

A number state is a normalized [eigenstate](energy-eigenvalue.md#eigenstate) of the [number operator](#number-operator):

$$
N|n\rangle=n|n\rangle,
\qquad n\in\mathbb Z_{\geq0}.
$$

For a single [quantum harmonic oscillator](quantum-harmonic-oscillator.md), it is also an [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) with energy $\hbar\omega(n+1/2)$.

#### Integer spectrum of the number operator

↑ **Parent:** [Number operator](#number-operator)

If $N|\nu\rangle=\nu|\nu\rangle$, then $A$ lowers the eigenvalue by one and $\|A|\nu\rangle\|^2=\nu\|\nu\rangle\|^2$. Positivity forces the lowering ladder to terminate at eigenvalue zero, so every eigenvalue is a nonnegative integer.

## Two commensurate quantum harmonic oscillators

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)

For independent frequencies $1$ and $2$,

$$
H_0=N_A+2N_B+\frac32,
$$

so the eigenspace at energy $k+3/2$ has one basis state $|n,m\rangle$ for each nonnegative solution of $n+2m=k$.

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (145)

- [Bond potential-well depth](chemical-bond.md#bond-potential-well-depth)
- [Bose condensation in a three-dimensional harmonic trap](quantum-ideal-gas-statistics.md#bose-condensation-in-a-three-dimensional-harmonic-trap)
- [Breathing Gaussian state in a harmonic oscillator](#breathing-gaussian-state-in-a-harmonic-oscillator)
- [Canonical oscillator coordinate variance](#canonical-oscillator-coordinate-variance)
- [Cartesian and spherical bases of the first oscillator shell](#cartesian-and-spherical-bases-of-the-first-oscillator-shell)
- [Classical grand potential in a harmonic trap](ideal-gas.md#classical-grand-potential-in-a-harmonic-trap)
- [Coherent state after shifting an oscillator equilibrium](quantum-theory.md#coherent-state-after-shifting-an-oscillator-equilibrium)
- [Coherent-state oscillator expectation values](quantum-theory.md#coherent-state-oscillator-expectation-values)
- [Compact cosine trial bound for the quantum harmonic oscillator](linear-operator-theory.md#compact-cosine-trial-bound-for-the-quantum-harmonic-oscillator)
- [Compact parabolic trial bound for the quantum harmonic oscillator](linear-operator-theory.md#compact-parabolic-trial-bound-for-the-quantum-harmonic-oscillator)
- [Contact shifts of two spin-one-half fermions in a harmonic trap](tensor-product-of-quantum-systems.md#contact-shifts-of-two-spin-one-half-fermions-in-a-harmonic-trap)
- [Cosine-potential gap in a quantum ring](topological-quantum-matter.md#cosine-potential-gap-in-a-quantum-ring)
- [Creation operator](#creation-operator)
- [Crossover from Gaussian to Thomas–Fermi condensate](quantum-ideal-gas-statistics.md#crossover-from-gaussian-to-thomas-fermi-condensate)
- [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)
- [Dynamic electric polarizability](electrostatics.md#dynamic-electric-polarizability)
- [Einstein solid](heat.md#einstein-solid)
- [Electric dipole transition](quantum-mechanics.md#electric-dipole-transition)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Finite oscillator commutator boundary defect](quantum-mechanics.md#finite-oscillator-commutator-boundary-defect)
- [First-order ground state of the quartic oscillator](quantum-mechanics.md#first-order-ground-state-of-the-quartic-oscillator)
- [From Heisenberg arrays to Born-Jordan commutation](quantum-mechanics.md#from-heisenberg-arrays-to-born-jordan-commutation)
- [Gaussian covariance in a harmonic potential](wave-function.md#gaussian-covariance-in-a-harmonic-potential)
- [Gaussian variational energy for the harmonic oscillator](quantum-theory.md#gaussian-variational-energy-for-the-harmonic-oscillator)
- [Ground state](quantum-mechanics.md#ground-state)
- [Ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy)
- [Harmonic-oscillator dipole response to switched radiation](electrostatics.md#harmonic-oscillator-dipole-response-to-switched-radiation)
- [Harmonic-oscillator forbidden-region probability](#harmonic-oscillator-forbidden-region-probability)
- [Harmonic-oscillator wavefunction inflections](#harmonic-oscillator-wavefunction-inflections)
- [Harmonic vibrational energy levels](molecule.md#harmonic-vibrational-energy-levels)
- [HCl and DCl harmonic stretch comparison](molecule.md#hcl-and-dcl-harmonic-stretch-comparison)
- [Heisenberg uncertainty relation](quantum-theory.md#heisenberg-uncertainty-relation)
- [Hermite function](orthogonal-polynomial.md#hermite-function)
- [Internal energy of an ideal gas](ideal-gas.md#internal-energy-of-an-ideal-gas)
- [Isotope scaling of diatomic vibration](classical-mechanics.md#isotope-scaling-of-diatomic-vibration)
- [Lamb-Mössbauer factor](mossbauer-effect.md#lamb-mossbauer-factor)
- [Matrix mechanics](quantum-mechanics.md#matrix-mechanics)
- [Minimum-energy normalized oscillator mode](#minimum-energy-normalized-oscillator-mode)
- [Minimum uncertainty state](quantum-theory.md#minimum-uncertainty-state)
- [Morse potential](quantum-system.md#morse-potential)
- [Normal and Weyl symbols of a harmonic oscillator](perturbative-quantum-field-theory.md#normal-and-weyl-symbols-of-a-harmonic-oscillator)
- [Nuclear quadrupole vibration](atomic-nucleus.md#nuclear-quadrupole-vibration)
- [Number state](#number-state)
- [One-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain)
- [Oscillator length](#oscillator-length)
- [Parity-twisted oscillator thermal trace](canonical-ensemble.md#parity-twisted-oscillator-thermal-trace)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2014/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#2/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#2/c/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018.md#section-b/b2/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019.md#section-b/5/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021.md#section-a/1/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/4/e/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#1/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-1.md#a1/b/iv/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-1.md#a2/b/iii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1.md#a2/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2.md#a6/b/i/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2.md#a6/c/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b.md#section-a/25/a/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b.md#section-a/25/b/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b.md#section-b/33/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1.md#18a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#19d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3.md#7b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#32d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#33c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#33d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#33c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-47.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#6a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#30a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#17b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#17b/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2.md#17b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2.md#17b/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-304.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#33d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-310.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1.md#15b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#34b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#34a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4.md#15c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#15b/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1.md#14b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#34a/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#34b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#34d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#10/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#10/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1.md#section-a/2/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1.md#section-c/c11/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-c/c11/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-b/b7/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-c/c11/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-c/c11/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1.md#section-b/b6/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2.md#section-d/d9/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1.md#section-d/d9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c11/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c9/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b6/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2018.md#4/a/solution)
- [Quadratic fluctuation Hamiltonian](perturbative-quantum-field-theory.md#quadratic-fluctuation-hamiltonian)
- [Quantized phase levels in a Josephson junction](superconductivity.md#quantized-phase-levels-in-a-josephson-junction)
- [Quantum harmonic chain](classical-mechanics.md#quantum-harmonic-chain)
- [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)
- [Quantum-oscillator energy and heat capacity](#quantum-oscillator-energy-and-heat-capacity)
- [Quantum variational principle](quantum-mechanics.md#quantum-variational-principle)
- [Raman vibrational activity](optics.md#raman-vibrational-activity)
- [Shaken harmonic trap](#shaken-harmonic-trap)
- [Spin-boson model](tensor-product-of-quantum-systems.md#spin-boson-model)
- [Spin-orbit shifts of an isotropic harmonic oscillator](atomic-physics.md#spin-orbit-shifts-of-an-isotropic-harmonic-oscillator)
- [Stokes Raman scattering](optics.md#stokes-raman-scattering)
- [Thermal light](quantum-optics.md#thermal-light)
- [Thermal partition function of a quantum harmonic oscillator](#thermal-partition-function-of-a-quantum-harmonic-oscillator)
- [Tilted Josephson washboard potential](superconductivity.md#tilted-josephson-washboard-potential)
- [Tilted Ornstein-Uhlenbeck oscillator transformation](gaussian-process.md#tilted-ornstein-uhlenbeck-oscillator-transformation)
- [Trapped-ion internal and motional states](atomic-physics.md#trapped-ion-internal-and-motional-states)
- [Trapped-ion quantum control](atomic-physics.md#trapped-ion-quantum-control)
- [Trapped-ion sideband pulse model](atomic-physics.md#trapped-ion-sideband-pulse-model)
- [Two-electron states in the first two shells of an isotropic oscillator](tensor-product-of-quantum-systems.md#two-electron-states-in-the-first-two-shells-of-an-isotropic-oscillator)
- [Vacuum energy sign of a fermionic oscillator](perturbative-quantum-field-theory.md#vacuum-energy-sign-of-a-fermionic-oscillator)
- [Variational method](quantum-theory.md#variational-method)
- [Vibrational heat capacity of a diatomic gas](molecule.md#vibrational-heat-capacity-of-a-diatomic-gas)
- [Vibrational partition function](canonical-ensemble.md#vibrational-partition-function)
- [Zero-point motion](#zero-point-motion)
