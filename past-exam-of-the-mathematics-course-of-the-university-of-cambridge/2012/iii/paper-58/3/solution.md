<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [laws of black-hole mechanics](../../../../../laws-of-black-hole-mechanics.md) establish the classical analogy with [thermodynamics](../../../../../thermodynamics-split.md). The [Zeroth law of black-hole mechanics](../../../../../zeroth-law-of-black-hole-mechanics.md) makes [surface gravity](../../../../../surface-gravity.md) constant on a connected equilibrium [Killing horizon](../../../../../killing-horizon.md), under its usual field-equation and energy hypotheses, paralleling constant temperature. For neighboring stationary Einstein–Maxwell solutions, the [First law of black-hole mechanics](../../../../../first-law-of-black-hole-mechanics.md) is

$$
\delta M=\frac{\kappa}{8\pi G}\delta A+\Omega_H\delta J+\Phi_H\delta Q.
$$

This parallels $\delta E=T\delta S$ plus work terms; $M$ denotes energy in $c=1$ units. The [second law of black-hole mechanics](../../../../../second-law-of-black-hole-mechanics.md) says area cannot decrease under the classical null-energy and global predictability assumptions. The [third law of black-hole mechanics](../../../../../third-law-of-black-hole-mechanics.md) is unattainability: regular finite physical processes satisfying its hypotheses cannot drive $\kappa$ to zero. It parallels unattainability of absolute zero, not a universal assertion of zero extremal entropy.

Classically a hole absorbs without emitting, so the analogy alone does not identify a measured temperature. Quantum [Hawking radiation](../../../../../hawking-radiation.md) supplies $T_H=\hbar\kappa/(2\pi)$, with $c=k_B=1$ and future-horizon normalization at infinity. Comparing the area terms in the first laws gives **the [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md)**

$$
\delta S_{\rm BH}=\frac{\delta A}{4G\hbar},\qquad\boxed{S_{\rm BH}=\frac{A}{4G\hbar}},
$$

up to a conventionally fixed additive constant. In ordinary units it is $k_Bc^3A/(4G\hbar)$. Entropy scales with area, not interior volume.

For the massless scalar in [quantum field theory in curved spacetime](../../../../../quantum-field-theory-in-curved-spacetime.md), [global hyperbolicity](../../../../../globally-hyperbolic-spacetime.md) ensures well-posed Cauchy evolution. The conserved [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) is

$$
(f,g)=i\int_\Sigma d\Sigma^\mu(f^*\nabla_\mu g-g\nabla_\mu f^*).
$$

Its current has zero divergence by the wave equation, making it slice-independent with appropriate boundary behavior. Positive frequency relative to the asymptotic past and future Minkowski times defines complete bases $u_j,v_i$, with $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and vanishing mixed products. Expand the field as

$$
\Phi=\sum_j(a_j^{\rm in}u_j+a_j^{{\rm in}\dagger}u_j^*)=\sum_i(a_i^{\rm out}v_i+a_i^{{\rm out}\dagger}v_i^*).
$$

Continuous labels replace sums by integrals; wave packets avoid artificial normalization infinities. [Particle creation by a nonstationary spacetime](../../../../../particle-creation-by-a-nonstationary-spacetime.md) occurs when evolution mixes frequency signs through a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md):

$$
v_i=\sum_j(\alpha_{ij}u_j+\beta_{ij}u_j^*),\qquad a_i^{\rm out}=\sum_j(\alpha_{ij}^*a_j^{\rm in}-\beta_{ij}^*a_j^{{\rm in}\dagger}).
$$

The inner product gives $\alpha\alpha^\dagger-\beta\beta^\dagger=I$ and $\alpha\beta^{\mathsf T}=\beta\alpha^{\mathsf T}$. For the initial vacuum annihilated by all $a_j^{\rm in}$, **$\boxed{\langle N_i^{\rm out}\rangle_{\rm in}=\sum_j|\beta_{ij}|^2}$.** Thus nonzero negative-frequency mixing makes the in-vacuum non-vacuum for final observers. The [vacuum state in a stationary spacetime](../../../../../vacuum-state-in-a-stationary-spacetime.md) depends on its positive-frequency splitting; this is not inconsistent with deterministic mode evolution. A unitary implementation on one fixed infinite-mode [Fock space](../../../../../fock-space.md) further needs the Hilbert–Schmidt condition on $\beta$.

For collapse forming a [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md), a late outgoing ray traced back to past null infinity obeys the [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md)

$$
U_H-U=C e^{-\kappa u},\qquad\kappa=1/(4GM).
$$

Pulling $e^{-i\omega u}$ back gives $(U_H-U)^{i\omega/\kappa}$ for $U<U_H$. Its past Fourier transform has both frequency signs. For $y=\omega/\kappa$ and damping $\epsilon>0$, the [Gamma function](../../../../../gamma-function.md) evaluates the Fourier integrals as

$$
I_\pm=\int_0^\infty x^{iy}e^{-\epsilon x\pm i\omega' x}dx=\frac{\Gamma(1+iy)}{(\epsilon\mp i\omega')^{1+iy}}.
$$

As $\epsilon\downarrow0$, the two denominator arguments approach $\mp\pi/2$, so $|I_+|/|I_-|=e^{-\pi y}$. Thus the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md) is $|\beta|^2/|\alpha|^2=e^{-2\pi\omega/\kappa}$. Together with the bosonic normalization difference, this yields $1/(e^{2\pi\omega/\kappa}-1)$. Potential scattering adds a [greybody factor](../../../../../greybody-factor.md):

$$
\frac{dN}{dt\,d\omega}=\frac1{2\pi}\sum_{\ell,m}\frac{\Gamma_\ell(\omega)}{e^{2\pi\omega/\kappa}-1},\qquad\boxed{T_H=\frac{\hbar}{8\pi GM}}.
$$

The collapse state has outgoing flux at future infinity without an incoming thermal bath and is regular for infall. It is not the eternal-hole equilibrium state. Horizon-entering modes complete the future basis; tracing over their correlated partners gives the approximately thermal exterior state. The collapsing geometry is not literally Minkowskian everywhere in the far future: asymptotically flat null-infinity modes are the relevant application of the earlier in/out construction.

Emission reduces the isolated hole's mass. Schwarzschild temperature is proportional to $M^{-1}$, giving the [negative heat capacity of a Schwarzschild black hole](../../../../../negative-heat-capacity-of-a-schwarzschild-black-hole.md): losing energy makes it hotter. Dimensional estimates give luminosity proportional to $M^{-2}$ and evaporation time proportional to $M^3$, with species and greybody factors determining coefficients. Area may shrink because quantum stress violates the energy assumptions of [Hawking's area theorem](../../../../../hawking-s-area-theorem.md). The [generalized second law](../../../../../generalized-second-law.md) instead concerns $S_{\rm gen}=A/(4G\hbar)+S_{\rm outside}$, incorporating radiation entropy and preventing ordinary thermodynamic violations by disposal of entropy into a hole.

Pair correlations also distinguish thermal reduced states from the complete pure state. The [black hole information paradox](../../../../../black-hole-information-paradox.md) asks whether complete evaporation preserves quantum information: an exactly thermal final exterior with no remaining partners would appear inconsistent with unitary pure-state evolution. The semiclassical calculation controls late-time flux, not the Planck-scale endpoint, and does not itself settle this question. **Quantum emission gives the temperature–entropy identification physical meaning; generalized entropy replaces the classical area alone when radiation back-reacts.**

## ↑ Ancestors (11)

1. [3](../3.md)
2. [Section II](../section-ii.md)
3. [Paper 58](../../paper-58-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
