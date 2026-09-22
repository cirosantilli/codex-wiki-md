<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Boltzmann distribution](../../../../../boltzmann-distribution.md) for two atomic levels at thermodynamic equilibrium is

$$
\boxed{\frac{N_a}{N_b}=\frac{\omega_a}{\omega_b}
\exp\left[-\frac{E_a-E_b}{kT}\right],}
$$

where $\omega$ is the [statistical weight of an atomic level](../../../../../statistical-weight-of-an-atomic-level.md). For a resolved level of total angular momentum $J$, $\omega=2J+1$ when magnetic substates are unresolved.

To extend this counting to the continuum, assume an ideal, nondegenerate [plasma](../../../../../plasma-physics.md) with classical free [Electrons](../../../../../electron.md) and neglect the small difference between the translational masses of the two heavy ionic species. Let $z_e=e^{\mu_e/kT}$ be the [electron fugacity in the Saha equation](../../../../../electron-fugacity-in-the-saha-equation.md), with the [Electron](../../../../../electron.md) [chemical potential](../../../../../chemical-potential.md) measured relative to its rest energy. The two [Electron](../../../../../electron.md) spin states and the phase-space cell volume $h^3$ give

$$
N_e=\frac{2z_e}{h^3}\int_{\mathbb R^3}e^{-p^2/(2mkT)}\,d^3p
=2z_e\left(\frac{2\pi mkT}{h^2}\right)^{3/2}.
$$

Chemical equilibrium for capture equates the bound species' [chemical potential](../../../../../chemical-potential.md) to the sum for its parent [ion](../../../../../ion.md) and free [Electron](../../../../../electron.md). Thus applying [Boltzmann factors](../../../../../boltzmann-factor.md) to a bound level at energy $-I_n$ gives $N_n/N_+=(\omega_n/\omega_+)z_e e^{I_n/kT}$. Eliminating the [Electron](../../../../../electron.md) fugacity proves the level-specific [Saha ionization equation](../../../../../saha-ionization-equation.md):

$$
\boxed{\frac{N_n}{N_eN_+}
=\frac{\omega_n}{2\omega_+}
\left(\frac{h^2}{2\pi mkT}\right)^{3/2}e^{I_n/kT}.}
$$

The factor two is the [Electron](../../../../../electron.md) spin multiplicity; the factor with power $3/2$ is the inverse free-electron translational state density. A total-ionization Saha equation sums the bound states into an internal partition function, whereas this expression refers to one specified level.

For [dielectronic recombination](../../../../../dielectronic-recombination.md), write the entrance [ion](../../../../../ion.md) as $X^{(z+1)+}$ in ground state $i$, and the intermediate state of $X^{z+}$ as $d=(j,n\ell)$. Capture excites the core from $i$ to $j$ while binding the incident [Electron](../../../../../electron.md). The resonance energy relative to the entrance continuum is $\bar E=E_{ij}-I_{n\ell}>0$. The doubly excited state can eject the [Electron](../../../../../electron.md) by [autoionization](../../../../../autoionization.md), or undergo [radiative stabilization](../../../../../radiative-stabilization.md) to a bound state.

Let $A^a_{di}$ be the partial [autoionization](../../../../../autoionization.md) rate back to the entrance [ion](../../../../../ion.md), $A_a$ the total [autoionization](../../../../../autoionization.md) rate, $A_r$ the total radiative decay rate, and $A_s$ the rate of radiative decays that stabilize into bound levels. For an isolated narrow resonance, the Saha-Boltzmann equilibrium ratio has the bound-state energy replaced by the positive resonance energy:

$$
\frac{N_d^{\rm eq}}{N_eN_i}
=\frac{g_d}{2g_i}\left(\frac{h^2}{2\pi mkT}\right)^{3/2}e^{-\bar E/kT}.
$$

At equilibrium, inverse [dielectronic capture](../../../../../dielectronic-capture.md) and [autoionization](../../../../../autoionization.md) fluxes balance: $N_eN_iC_d=N_d^{\rm eq}A^a_{di}$. This establishes the capture coefficient even when the actual [plasma](../../../../../plasma-physics.md) is not in local thermodynamic equilibrium. In the low-density, weak-radiation recombining [plasma](../../../../../plasma-physics.md), the intermediate level instead has the stationary balance

$$
N_eN_iC_d=N_d(A_a+A_r).
$$

Multiplying its population by the successful stabilization rate gives the actual recombination coefficient

$$
\boxed{\alpha_d(d)=\frac{g_d}{2g_i}
\left(\frac{h^2}{2\pi mkT}\right)^{3/2}
e^{-\bar E/kT}\frac{A^a_{di}A_s}{A_a+A_r}.}
$$

Here the equilibrium population was used only to determine the capture rate by detailed balance; it was not assumed to equal the intermediate population when [photons](../../../../../photon.md) escape. This is precisely why the competing decay probabilities appear.

Use the supplied core-transition relation between the [Einstein coefficients](../../../../../einstein-coefficients.md) and [atomic oscillator strength](../../../../../atomic-oscillator-strength.md),

$$
A_{ji}=\frac{\alpha^4c}{2a_0}\left(\frac{E_{ij}}{I_H}\right)^2\frac{g_i}{g_j}f_{ij},
\qquad \frac{h^2}{2\pi m}=4\pi a_0^2I_H.
$$

Here $\alpha$ is the [fine-structure constant](../../../../../fine-structure-constant.md) and $a_0$ the [Bohr radius](../../../../../bohr-radius.md), not a recombination coefficient. Factor out $A_{ji}$ and define

$$
\boxed{\beta_{j,n\ell}=\frac{g_d}{2g_j}\,
\frac{A^a_{di}A_s}{A_{ji}(A_a+A_r)}.}
$$

Substitution yields

$$
\begin{aligned}
\alpha_d(j,n\ell)
&=4\pi^{3/2}\alpha^4a_0^2c\,
\frac{E_{ij}^2}{I_H^{1/2}(kT)^{3/2}}
e^{-\bar E/kT}f_{ij}\beta_{j,n\ell}\\
&=\boxed{4\pi^{3/2}\alpha^4a_0^2c
\left(\frac{E_{ij}}{I_H}\right)^{1/2}
\left(\frac{E_{ij}}{kT}\right)^{3/2}
e^{-\bar E/kT}f_{ij}\beta_{j,n\ell}.}
\end{aligned}
$$

This definition accommodates several entrance and decay channels. In the common spectator-electron approximation with one [autoionization](../../../../../autoionization.md) channel and stabilization by the core transition, $A_s=A_r=A_{ji}$ and $A^a_{di}=A_a$. If all coupled substates of the captured $n\ell$ [Electron](../../../../../electron.md) are summed, $g_d=2(2\ell+1)g_j$, giving

$$
\boxed{\beta_{j,n\ell}=(2\ell+1)\frac{A_a}{A_a+A_{ji}}.}
$$

For an intermediate state resolved by [fine structure](../../../../../fine-structure.md), retain its actual $g_d$ instead of that summed weight. The stabilization probability itself is $A_s/(A_a+A_r)$; **the requested $\beta_{j,n\ell}$ is not just this branching probability, because the prefactor has already factored out the core radiative rate and [statistical weights of atomic levels](../../../../../statistical-weight-of-an-atomic-level.md).** Radiative transitions to another still-autoionizing state require that state's eventual survival probability, rather than automatically counting every emitted [photon](../../../../../photon.md) as stabilization.

The total [dielectronic recombination](../../../../../dielectronic-recombination.md) coefficient sums all accessible positive-energy resonances. In this isolated-resonance approximation it has the form

$$
\alpha_d(T)=T^{-3/2}\sum_d c_d e^{-\bar E_d/kT},\qquad c_d\geq0,
$$

with atomic factors included in $c_d$. The [resonance-temperature dependence of dielectronic recombination](../../../../../resonance-temperature-dependence-of-dielectronic-recombination.md) follows by differentiating a single term's logarithm:

$$
\frac{d}{dT}\log\alpha_d(d)=-\frac{3}{2T}+\frac{\bar E_d}{kT^2},
\qquad \boxed{kT_{\rm peak}=\frac23\bar E_d.}
$$

Thus low temperatures suppress a positive-energy resonance, although resonances very near threshold can still matter; at sufficiently high [temperature](../../../../../temperature.md) a fixed set of resonances falls as $T^{-3/2}$. Several core-excitation series can produce several peaks. When [autoionization](../../../../../autoionization.md) is much faster than radiation, the capture-and-survival product is limited by the stabilizing radiative rate; when capture is weak, [autoionization](../../../../../autoionization.md) is the limiting inverse-capture rate. For a fixed Rydberg angular channel, [autoionization](../../../../../autoionization.md) typically decreases at high principal quantum number while the core radiative rate changes little. Capture into very high levels is vulnerable to subsequent collisional or field ionization, so finite-density survival can suppress the total rate. **[dielectronic recombination](../../../../../dielectronic-recombination.md) is resonant and strongly temperature-selective; its magnitude can be important in coronal ionization balance.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
