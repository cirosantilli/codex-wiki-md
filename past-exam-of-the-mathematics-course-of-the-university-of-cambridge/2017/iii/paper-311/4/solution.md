<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work first in units $G=c=\hbar=k_B=1$. [Black-hole thermodynamics](../../../../../black-hole-thermodynamics.md) starts with the [laws of black-hole mechanics](../../../../../laws-of-black-hole-mechanics.md). For a [connected](../../../../../connected-space.md) stationary regular [Killing horizon](../../../../../killing-horizon.md), the [Zeroth law of black-hole mechanics](../../../../../zeroth-law-of-black-hole-mechanics.md) makes its [surface gravity](../../../../../surface-gravity.md) $\kappa$ constant when the [Einstein field equations](../../../../../einstein-field-equations.md) and [dominant energy condition](../../../../../dominant-energy-condition.md) hold. This parallels uniform equilibrium [temperature](../../../../../temperature.md). For neighboring stationary asymptotically flat four-dimensional Einstein-Maxwell [black holes](../../../../../black-hole.md), the [First law of black-hole mechanics](../../../../../first-law-of-black-hole-mechanics.md) is

$$
\delta M=\frac\kappa{8\pi}\delta A+\Omega_H\delta J+\Phi_H\delta Q,
$$

where $\Omega_H$ is the horizon [angular velocity](../../../../../angular-velocity.md) and $\Phi_H$ its [electric potential](../../../../../electric-potential.md) relative to infinity. The last terms are rotational and electromagnetic work, analogous to the work terms in $\delta E=T\delta S+\text{work}$. The [second law of black-hole mechanics](../../../../../second-law-of-black-hole-mechanics.md), expressed by [Hawking's area theorem](../../../../../hawking-s-area-theorem.md), makes the total future horizon area nondecreasing for classical matter obeying the [null energy condition](../../../../../null-energy-condition.md) and global assumptions such as [strong asymptotic predictability](../../../../../strong-asymptotic-predictability.md). The [third law of black-hole mechanics](../../../../../third-law-of-black-hole-mechanics.md) is an unattainability statement: subject to the usual regularity assumptions, the [weak energy condition](../../../../../weak-energy-condition.md), and a bounded [stress-energy tensor](../../../../../stress-energy-tensor.md), no finite physical process reduces the [surface gravity](../../../../../surface-gravity.md) of a regular horizon to zero. It does not assert that [extremal black holes](../../../../../extremal-black-hole.md) have zero area or zero [entropy](../../../../../entropy.md).

Classical geometry alone fixes an analogy, not a nonzero physical [temperature](../../../../../temperature.md). [Quantum field theory](../../../../../quantum-field-theory-split.md) supplies [Hawking temperature](../../../../../hawking-temperature.md) $T_H=\kappa/(2\pi)$. Comparing the area term of the first law with $T_H\delta S$ gives $\delta S=\delta A/4$ for nonextremal holes, and hence the standard [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md). Restoring physical constants,

$$
\boxed{T_H=\frac{\hbar\kappa}{2\pi c k_B},\qquad
S_{\mathrm{BH}}=\frac{k_Bc^3A}{4G\hbar}=\frac{k_BA}{4\ell_P^2}.}
$$

Here restored $\kappa$ is the physical acceleration [surface gravity](../../../../../surface-gravity.md) and $\ell_P^2=G\hbar/c^3$ is the squared [Planck length](../../../../../planck-length.md). The first-law comparison determines the area coefficient, leaving an additive [entropy](../../../../../entropy.md) constant unspecified; the displayed formula is the usual convention. Its area scaling, rather than ordinary volume scaling, signals that the available thermodynamic degrees of freedom of a gravitating system are constrained by the horizon geometry.

Particle production explains the quantum input. For a [real scalar field](../../../../../real-scalar-field.md) obeying the massless covariant [wave equation](../../../../../wave-equation-split.md), the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) on solutions is

$$
(u,v)=i\int_\Sigma d\Sigma^a\left(u^*\nabla_av-v\nabla_au^*\right).
$$

The [wave equation](../../../../../wave-equation-split.md) makes its current divergence-free, so the product is independent of a [Cauchy hypersurface](../../../../../cauchy-surface.md) when the boundary flux vanishes. Use suitably normalized [wave packets](../../../../../wave-packet.md) or the appropriate continuum distributions. Asymptotic past and future [Minkowski spacetimes](../../../../../minkowski-spacetime.md) give preferred [positive-frequency solution](../../../../../positive-frequency-solution.md) mode bases $u_j^{\mathrm{in}}$ and $u_i^{\mathrm{out}}$, normalized by $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and $(u_i,u_j^*)=0$. Between those regions, a nonstationary geometry generally has no preferred positive-frequency splitting.

The mode bases are related by a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md),

$$
u_i^{\mathrm{out}}=\sum_j\left(\alpha_{ij}u_j^{\mathrm{in}}+\beta_{ij}u_j^{\mathrm{in}*}\right),
\qquad
\alpha\alpha^\dagger-\beta\beta^\dagger=I,\quad
\alpha\beta^T=\beta\alpha^T.
$$

The last identities follow from conservation of the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) and are the [canonical identities for a bosonic Bogoliubov transformation](../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md). Expanding the field in either complete basis and extracting its positive-frequency coefficient gives

$$
a_i^{\mathrm{out}}=\sum_j\left(\alpha_{ij}^*a_j^{\mathrm{in}}-\beta_{ij}^*a_j^{\mathrm{in}\dagger}\right).
$$

Thus the state annihilated by every $a_j^{\mathrm{in}}$ has

$$
\boxed{\langle0_{\mathrm{in}}|N_i^{\mathrm{out}}|0_{\mathrm{in}}\rangle
=\sum_j|\beta_{ij}|^2.}
$$

This [particle number from Bogoliubov coefficients](../../../../../particle-number-from-bogoliubov-coefficients.md) is nonzero when time evolution mixes positive and negative frequencies. It describes one state as vacuum in the early particle basis and populated in the late basis; it does not require an arbitrary choice of a vacuum at each intermediate time. For a finite implementable transformation the state remains a squeezed [pure quantum state](../../../../../pure-state.md). In infinitely many modes, a common unitary [bosonic Fock space](../../../../../bosonic-fock-space.md) implementation requires additional conditions, such as the beta map being a [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md); finite [wave packet](../../../../../wave-packet.md) observables need not share every global divergence of an ideal continuum calculation.

For gravitational collapse, the future is not globally Minkowski: it contains a [black hole](../../../../../black-hole.md). The relevant late out-basis includes modes reaching [future null infinity](../../../../../future-null-infinity.md) together with modes entering the future [event horizon](../../../../../event-horizon.md). Modes on infinity alone are not a complete Cauchy basis. Nevertheless the same mode-mixing calculation determines the outgoing particle flux. Near a nonextremal horizon, the logarithm in the [tortoise coordinate](../../../../../tortoise-coordinate.md) converts regular early null coordinates into the [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md)

$$
U_H-U=Ae^{-\kappa u},\qquad A>0,
$$

where $U$ is the early affine null coordinate and $u$ is late retarded time at infinity. Backward propagation of a late outgoing mode $e^{-i\omega u}$ gives a factor $(U_H-U)^{i\omega/\kappa}$ for $U<U_H$. Its positive- and negative-frequency Fourier [integrals](../../../../../integral.md) differ by [analytic continuation](../../../../../analytic-continuation.md) around the logarithmic branch. With a convergence regulator they reduce to

$$
\int_0^\infty x^{ia}e^{-(\epsilon\pm i\omega')x}\,dx
=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia},\qquad a=\frac\omega\kappa.
$$

Taking $\epsilon\downarrow0$ gives the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md), $|\beta|^2/|\alpha|^2=e^{-2\pi\omega/\kappa}$. Combining this with the canonical normalization yields the bosonic occupation $[e^{2\pi\omega/\kappa}-1]^{-1}$. Late-time [wave packets](../../../../../wave-packet.md) turn formal continuum coefficients into a finite number flux.

A [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md) has $\kappa=1/(4M)$, so this spectrum has $T_H=1/(8\pi M)$. The exterior curvature potential partly reflects the outgoing modes. Its transmission [probabilities](../../../../../probability.md) are the [greybody factors](../../../../../greybody-factor.md), giving, for one massless scalar species in the stationary late-time approximation,

$$
\frac{d^2N}{du\,d\omega}=\frac1{2\pi}
\sum_{\ell=0}^{\infty}(2\ell+1)
\frac{\Gamma_\ell(\omega)}{e^{8\pi M\omega}-1}.
$$

Thus the horizon [temperature](../../../../../temperature.md) is universal, while the spectrum received at infinity is not a perfect featureless [blackbody radiation](../../../../../black-body-radiation.md) spectrum. The derivation assumes the near-horizon [quantum state](../../../../../quantum-state.md) inherited from a regular collapse vacuum and ignores rapid backreaction over the timescale of the packets. Exponentially blueshifted precursor frequencies indicate the usual short-distance assumption in the semiclassical calculation, not an independently demonstrated quantum-gravity description of the endpoint.

The outgoing positive [energy](../../../../../energy.md) flux drives [black-hole evaporation](../../../../../black-hole-evaporation.md). At leading order for a large isolated [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md), area scales as $M^2$ and [temperature](../../../../../temperature.md) as $M^{-1}$, giving $dM/du\sim-\gamma/M^2$ and a lifetime of order $M^3$, with the coefficient depending on species and transmission factors. Its [negative heat capacity of a Schwarzschild black hole](../../../../../negative-heat-capacity-of-a-schwarzschild-black-hole.md), $dM/dT_H=-8\pi M^2$, means that it heats up as it loses [mass](../../../../../mass.md) and cannot be in stable canonical equilibrium with an unlimited thermal reservoir. The approximation fails when quantum-gravitational scales are reached and does not fix whether the endpoint is complete evaporation, a remnant, or something else.

Area loss does not contradict the classical area theorem, because the quantum [stress-energy tensor](../../../../../stress-energy-tensor.md) need not obey the classical [null energy condition](../../../../../null-energy-condition.md); negative horizon [energy](../../../../../energy.md) accompanies the positive outgoing flux. The appropriate thermodynamic statement is the [generalized second law](../../../../../generalized-second-law.md), involving $S_{\mathrm{BH}}+S_{\mathrm{outside}}$. Finally, [Hawking radiation](../../../../../hawking-radiation.md) raises the [black hole information paradox](../../../../../black-hole-information-paradox.md): if a [pure quantum state](../../../../../pure-state.md) completely evaporates into an exactly thermal [mixed quantum state](../../../../../mixed-state.md) and its partners disappear, the result conflicts with ordinary [unitary time evolution](../../../../../unitary-time-evolution.md). Early outgoing radiation can be mixed simply because of its [entanglement](../../../../../entangled-state.md) with interior modes while the complete state remains a [pure quantum state](../../../../../pure-state.md); that fact alone is not information loss. Resolving the fate of all correlations through the evaporation endpoint requires more than the leading semiclassical flux calculation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 311](../../paper-311-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
