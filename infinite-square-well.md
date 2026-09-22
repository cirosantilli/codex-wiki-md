# Infinite square well

↑ **Parent:** [Quantum mechanics](quantum-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Particle_in_a_box)

The [infinite square well](infinite-square-well.md) is an ideal confinement model with [potential energy](potential-energy.md) $V(x)=0$ for $0<x<L$ and infinite walls outside. The walls impose [Dirichlet boundary conditions](dirichlet-boundary-condition.md) $\phi(0)=\phi(L)=0$ and a vanishing exterior [wavefunction](wave-function.md). Inside, the time-independent [Schrödinger equation](schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\frac{d^2\phi}{dx^2}=E\phi,\qquad \phi_n(x)=\sqrt{\frac2L}\sin\frac{n\pi x}{L},\qquad E_n=\frac{n^2\pi^2\hbar^2}{2mL^2},\quad n=1,2,\ldots.
$$

The first wall removes the [cosine](cosine.md) term; the second requires $\sin(kL)=0$, hence $k=n\pi/L$. The $n=0$ solution is identically zero and cannot satisfy [wavefunction normalization](wavefunction-normalization.md). Each [energy eigenstate](energy-eigenstate.md) has $n-1$ interior [nodes of a standing wave](node-physics.md), at $x=jL/n$ for $j=1,\ldots,n-1$. More curvature costs more [kinetic energy](kinetic-energy.md), explaining the $n^2$ growth. The positive [ground-state energy](ground-state-energy.md) is a confinement effect: a constant zero-energy [wavefunction](wave-function.md) cannot satisfy both walls and remain normalized.

For an [Electron](electron.md) with mass $m_e=9.1093837139\times10^{-31}\,\mathrm{kg}$ in a box of length $L=1\,\mathrm{nm}$, use $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$ and $1\,\mathrm{eV}=1.602176634\times10^{-19}\,\mathrm J$. These constants are from the 2022 CODATA adjustment. [Fundamental Physical Constants — Complete Listing by National Institute of Standards and Technology and others](fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others.md). Substitution gives

$$
E_1=\frac{h^2}{8m_eL^2}=6.024667\times10^{-20}\,\mathrm J\approx0.376030\,\mathrm{eV},\qquad E_2=4E_1\approx1.504121\,\mathrm{eV}.
$$

Doubling $L$ quarters every [energy eigenvalue](energy-eigenvalue.md); doubling $m$ halves them. This scaling makes the [particle in a box](infinite-square-well.md) useful for estimating confinement energies before attempting a more realistic calculation. A [finite square well](finite-square-well.md) permits exterior tails for [bound states](bound-state.md) and has only finitely many bound [energy eigenstates](energy-eigenstate.md). For an [Electron](electron.md), the scalar box calculation assumes fixed [spin](spin.md) and no spin-dependent interactions.

For the [ground state](ground-state.md), the probability of finding the particle in the middle half of the box is fully computable:

$$
\Pr\left(\frac L4<x<\frac{3L}4\right)=\int_{L/4}^{3L/4}\frac2L\sin^2\frac{\pi x}{L}\,dx=\left[\frac xL-\frac{\sin(2\pi x/L)}{2\pi}\right]_{L/4}^{3L/4}=\frac12+\frac1\pi\approx0.818310.
$$

Thus half the available length contains about $81.8\%$ of the probability. The figure contrasts the signed [wavefunctions](wave-function.md) with their nonnegative [probability densities](probability-density.md): a negative lobe is an amplitude with opposite [quantum phase](quantum-phase.md), not negative probability.

<a id="image-ideal-infinite-square-well-normalized-modes-nodes-and-analytic-position-densities"></a>
![](quantum-box-eigenstates.png)

**[Figure 21](#image-ideal-infinite-square-well-normalized-modes-nodes-and-analytic-position-densities). Ideal infinite square well: normalized modes, nodes, and analytic position densities**.

An equal [quantum superposition](quantum-superposition.md) of the first two [energy eigenstates](energy-eigenstate.md) gives a simple example of moving density:

$$
\psi(x,t)=\frac{\phi_1(x)e^{-iE_1t/\hbar}+\phi_2(x)e^{-iE_2t/\hbar}}{\sqrt2},\qquad |\psi|^2=\frac{\phi_1^2+\phi_2^2}{2}+\phi_1\phi_2\cos\frac{(E_2-E_1)t}{\hbar}.
$$

Its density period is $T=h/(E_2-E_1)\approx3.66608\,\mathrm{fs}$ for the [Electron](electron.md) box above. At $t=0$ the cross term enhances the left side; at $T/4$ it vanishes; at $T/2$ it enhances the right side. More quantitatively,

$$
\Pr(0<x<L/2)=\frac12+\frac4{3\pi}\cos\frac{2\pi t}{T},
$$

which takes the values $0.924413$, $0.5$, and $0.075587$ at those times. [Orthogonality](orthogonal-vectors.md) keeps the total probability one throughout. An [energy measurement](energy-measurement.md) still returns $E_1$ or $E_2$ with equal probabilities: changing position density arises from relative [quantum phase](quantum-phase.md), not changing populations. A [mixed state](mixed-state.md) describing a statistical mixture with those populations has the constant [probability density](probability-density.md) $(\phi_1^2+\phi_2^2)/2$; it lacks this [matter-wave interference](matter-wave-interference.md) term.

<a id="image-ideal-box-superposition-relative-phase-changes-analytic-density-while-total-probability-stays-one"></a>
![](quantum-box-superposition.png)

**[Figure 22](#image-ideal-box-superposition-relative-phase-changes-analytic-density-while-total-probability-stays-one). Ideal box superposition: relative phase changes analytic density while total probability stays one**.

**Table of contents**

- [Energy form of a half-well sine state](energy-form-of-a-half-well-sine-state.md)
- [Ramp-state expansion in a symmetric infinite well](ramp-state-expansion-in-a-symmetric-infinite-well.md)
- [Particle in a rectangular box](particle-in-a-rectangular-box.md)

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Energy eigenspace](energy-eigenspace.md)
- [Energy eigenstate](energy-eigenstate.md)
- [Energy eigenvalue](energy-eigenvalue.md)
- [Energy form of a half-well sine state](energy-form-of-a-half-well-sine-state.md)
- [Excited state](excited-state.md)
- [Ground-state overlap after sudden expansion of a square well](ground-state-overlap-after-sudden-expansion-of-a-square-well.md)
- [Infinite square well](infinite-square-well.md)
- [Particle in a rectangular box](particle-in-a-rectangular-box.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/18f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/15g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/15a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/15b/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/8b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/15a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/15b/a/solution.md)
- [Quantum mechanics](quantum-mechanics-split.md)
- [Unfolding a reflected interval trajectory](unfolding-a-reflected-interval-trajectory.md)
- [Wave function](wave-function.md)
- [Wavefunction normalization](wavefunction-normalization.md)
