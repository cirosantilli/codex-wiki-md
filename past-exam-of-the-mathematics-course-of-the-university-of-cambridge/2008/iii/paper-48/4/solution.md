<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A symmetry of a [classical field theory](../../../../../classical-field-theory.md) maps solutions to solutions; for the [Noether theorem](../../../../../noether-theorem.md) we require a continuous variational symmetry of the action, allowing its density to change by a total divergence. This is stronger than simply observing an accidental symmetry of one solution. Consider first-derivative fields $\phi_a$ and define

$$
\Pi_a^\mu=\frac{\partial\mathcal L}{\partial(\partial_\mu\phi_a)},\qquad
E_a=\frac{\partial\mathcal L}{\partial\phi_a}-\partial_\mu\Pi_a^\mu.
$$

The [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) are $E_a=0$. For a fixed-coordinate variation $\delta_0\phi_a=\varepsilon Q_a$, the product rule gives the off-shell identity

$$
\frac{\delta_0\mathcal L}{\varepsilon}
=\sum_a E_aQ_a+\partial_\mu\!\left(\sum_a\Pi_a^\mu Q_a\right).
$$

This identity is the proof's essential integration-by-parts step.

For a general spacetime symmetry write $x'^\mu=x^\mu+\varepsilon\xi^\mu$ and $\phi'_a(x')=\phi_a(x)+\varepsilon\Delta_a$. At a fixed point $Q_a=\Delta_a-\xi^\nu\partial_\nu\phi_a$, while the volume-element variation contributes $\partial_\mu(\mathcal L\xi^\mu)$. Suppose action invariance takes the form

$$
\frac{\delta_0\mathcal L}{\varepsilon}+\partial_\mu(\mathcal L\xi^\mu)=\partial_\mu K^\mu.
$$

Combining with the preceding identity proves

$$
\boxed{j^\mu=\sum_a\Pi_a^\mu Q_a+\mathcal L\xi^\mu-K^\mu,
\qquad\partial_\mu j^\mu=-\sum_aE_aQ_a=0\ \text{on shell}.}
$$

This is the [Noether current for a spacetime symmetry](../../../../../noether-current-for-a-spacetime-symmetry.md). It also covers internal symmetries, for which $\xi=0$. A constant parameter corresponds to one [Noether current](../../../../../noether-current.md); several independent parameters give several currents. Integrating the continuity equation gives

$$
\frac{dQ}{dt}=-\int_{\partial\Sigma}\mathbf j\cdot d\mathbf S,
\qquad Q=\int_\Sigma j^0\,d^3x.
$$

Thus the [Noether charge](../../../../../noether-charge.md) is conserved when the fields have suitable falloff or no flux through the spatial boundary. These are classical identities; quantum symmetries may additionally require absence of an [quantum anomaly](../../../../../anomaly-physics.md).

**Translations conserve energy and momentum.** If the density has no explicit coordinate dependence, take the active fixed-coordinate variation $Q_a=\partial_\nu\phi_a$ for translation in direction $\nu$. Then $\delta_0\mathcal L/\varepsilon=\partial_\nu\mathcal L$, and the internal-form proof with $K^\mu=\delta^\mu{}_{\nu}\mathcal L$ gives the [canonical energy-momentum tensor](../../../../../canonical-stress-energy-tensor.md)

$$
T^\mu{}_{\nu}=\sum_a\Pi_a^\mu\partial_\nu\phi_a-\delta^\mu{}_{\nu}\mathcal L,
\qquad \partial_\mu T^\mu{}_{\nu}=0.
$$

Its four spatial integrals are the conserved energy and momentum. For a real [scalar field](../../../../../scalar-field.md) with density $\tfrac12(\partial\phi)^2-V(\phi)$ this becomes $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L$. Direct differentiation gives $\partial_\mu T^{\mu\nu}=(\Box\phi+V'(\phi))\partial^\nu\phi$, which vanishes by the field equation.

**Lorentz symmetry conserves angular momentum and boost charges.** For that scalar example, $T^{\mu\nu}$ is symmetric, so the [Lorentz transformation](../../../../../lorentz-transformation.md) currents can be written

$$
J^{\mu\rho\sigma}=x^\rho T^{\mu\sigma}-x^\sigma T^{\mu\rho}.
$$

Their divergence is $T^{\rho\sigma}-T^{\sigma\rho}=0$. Spatial pairs give [angular momentum](../../../../../angular-momentum.md), and time-space pairs give the conserved boost charges. For a [spinor field](../../../../../spinor-field.md) or a [vector field](../../../../../vector-field.md), the intrinsic field variation supplies an additional spin current; equivalently the [Belinfante-Rosenfeld stress-energy tensor](../../../../../belinfante-rosenfeld-stress-energy-tensor.md) combines spin and orbital pieces into a symmetric stress tensor. The nonunitarity of the finite component [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md) does not obstruct conservation of these physical spacetime charges.

**Global phase symmetry conserves particle charge.** For a complex [scalar field](../../../../../scalar-field.md) with density $\partial_\mu\Phi^*\partial^\mu\Phi-V(\Phi^*\Phi)$, the constant transformation $\Phi\mapsto e^{-i\alpha}\Phi$ leaves the density invariant. Using $Q_\Phi=-i\Phi$ and $Q_{\Phi^*}=i\Phi^*$ gives the [Noether current](../../../../../noether-current.md)

$$
j^\mu=i(\Phi^*\partial^\mu\Phi-\Phi\partial^\mu\Phi^*).
$$

For a [Dirac field](../../../../../dirac-field.md), the corresponding variations $Q_\psi=-i\psi$, $Q_{\bar\psi}=i\bar\psi$ yield instead $j^\mu=\bar\psi\gamma^\mu\psi$, the [Dirac current](../../../../../dirac-current.md). Its divergence vanishes by the [Dirac equation](../../../../../dirac-equation.md) and [adjoint Dirac equation](../../../../../adjoint-dirac-equation.md). The [Yukawa interaction](../../../../../yukawa-interaction.md) of part 2 also preserves this phase symmetry, because each bilinear has one $\psi$ and one $\bar\psi$. Thus it preserves fermion number and forbids annihilation of two fermions into a single scalar. These currents express charge or particle-minus-antiparticle-number conservation, rather than conservation of total particle count in arbitrary interacting processes.

A [global symmetry in field theory](../../../../../global-symmetry-in-field-theory.md) uses a spacetime-independent parameter and ordinarily relates physically distinct configurations. A [gauge symmetry](../../../../../gauge-invariance.md) instead has arbitrary local parameters and represents redundancy in the description. For example, the [Maxwell field](../../../../../electromagnetic-field.md) is unchanged physically by $A_\mu\mapsto A_\mu+\partial_\mu\alpha(x)$: its [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) is unchanged. For charged matter use $D_\mu=\partial_\mu+iqA_\mu$ together with $\psi\mapsto e^{-iq\alpha(x)}\psi$. Differentiating shows $D'_\mu\psi'=e^{-iq\alpha}D_\mu\psi$, so the coupled [Dirac action](../../../../../dirac-action.md) is locally gauge invariant. A local phase applied to free matter alone produces extra derivatives of $\alpha$ and is not an invariance; the compensating gauge field is necessary.

Local arbitrariness gives identities among field equations, rather than an independent physical charge for every function $\alpha$. In the pure [Maxwell field](../../../../../electromagnetic-field.md), action invariance under a compactly supported $\alpha$ implies

$$
0=\int d^4x\,E^\nu\partial_\nu\alpha
=-\int d^4x\,\alpha\partial_\nu E^\nu,
\qquad E^\nu=\partial_\mu F^{\mu\nu}.
$$

Thus $\partial_\nu E^\nu=0$ holds off shell, directly because $F^{\mu\nu}$ is antisymmetric. This exemplifies the [Noether second theorem](../../../../../noether-second-theorem.md). Gauge fixing and the [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md) remove redundant photon components; they do not remove a physical global charge. Gauge transformations that are nontrivial at a boundary can carry boundary charges, so the redundancy statement concerns transformations satisfying the chosen boundary conditions. Finally, discrete symmetries such as the sign reversal of a real scalar or [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) can be important without furnishing a continuous-parameter [Noether current](../../../../../noether-current.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
