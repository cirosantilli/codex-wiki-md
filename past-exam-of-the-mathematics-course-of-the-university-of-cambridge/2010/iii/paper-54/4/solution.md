<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work initially in units $G=c=\hbar=k_B=1$ and consider gravitational collapse settling to a nonextremal [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md). Classically, outgoing rays sufficiently close to the forming [event horizon](../../../../../event-horizon.md) suffer an arbitrarily large redshift. Quantum mechanically, the meaning of [positive frequency](../../../../../positive-frequency-solution.md) at [past null infinity](../../../../../past-null-infinity.md) differs from that at [future null infinity](../../../../../future-null-infinity.md); a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md) between these two mode descriptions can therefore mix [creation operators](../../../../../creation-operator.md) and [annihilation operators](../../../../../annihilation-operator.md). Hawking's argument computes that mixing and obtains a thermal occupation, even when the incoming state has no particles.

To see why the frequency mixing is universal, use final [Schwarzschild time](../../../../../schwarzschild-time.md) $t$, the [Schwarzschild tortoise coordinate](../../../../../schwarzschild-tortoise-coordinate.md) $r_*$, and retarded time $u=t-r_*$. Near the final [event horizon](../../../../../event-horizon.md), $r_*\sim(2\kappa)^{-1}\log(r-2M)$, with [Schwarzschild surface gravity](../../../../../schwarzschild-surface-gravity.md) $\kappa=1/(4M)$. On a fixed advanced-time section, $u=v-2r_*$, so $r-2M$ is proportional to $e^{-\kappa u}$. Tracing a ray back through the regular collapsing region maps this small separation smoothly to its separation from the last escaping incoming ray. If $U$ is an affine incoming [null coordinate](../../../../../null-coordinate.md) and $U_H$ labels that limiting ray, the [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md) is

$$
U_H-U=Ae^{-\kappa u}(1+o(1)),\qquad A>0.
$$

The logarithm at a simple horizon root fixes the exponent. Smooth propagation through the earlier collapse changes $A$ and phases but not the leading exponential redshift.

For a massless bosonic test [scalar field](../../../../../scalar-field.md), an outgoing mode of frequency $\omega>0$ at [future null infinity](../../../../../future-null-infinity.md) behaves as $e^{-i\omega u}$. Trace it backward in the high-frequency [geometric optics](../../../../../geometrical-optics.md) approximation. Its relevant incoming dependence is, up to normalization and a phase,

$$
p_\omega(U)\sim\Theta(U_H-U)\left(\frac{U_H-U}{A}\right)^{ia},\qquad a=\frac\omega\kappa.
$$

Here $\Theta$ is the [Heaviside step function](../../../../../heaviside-step-function.md). Incoming rays with $U>U_H$ do not escape. This truncated logarithmic phase is not purely [positive frequency](../../../../../positive-frequency-solution.md) with respect to $U$. Decomposing it into incoming [positive-frequency solutions](../../../../../positive-frequency-solution.md) $e^{-i\omega' U}$ and negative modes $e^{+i\omega' U}$ gives the [Bogoliubov transformation](../../../../../bogoliubov-transformation.md). With $x=U_H-U$, the two relevant [Fourier transform](../../../../../fourier-transform.md) integrals are

$$
I_-(\omega')=\int_0^\infty x^{ia}e^{-(\epsilon+i\omega')x}\,dx,
\qquad
I_+(\omega')=\int_0^\infty x^{ia}e^{-(\epsilon-i\omega')x}\,dx,
\qquad\epsilon>0.
$$

The former is the positive-frequency coefficient and the latter is the negative-frequency coefficient; the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) introduces the same frequency normalization into their modulus ratio. By the defining integral of the [gamma function](../../../../../gamma-function.md) and analytic continuation in its Laplace parameter,

$$
I_\mp=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia}.
$$

For a complex number $z$ in the right half-plane, $|z^{-1-ia}|=|z|^{-1}e^{a\arg z}$. As $\epsilon\downarrow0$, the two arguments tend to $+\pi/2$ and $-\pi/2$. This gives the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md):

$$
\boxed{\frac{|\beta_{\omega\omega'}|^2}{|\alpha_{\omega\omega'}|^2}=e^{-2\pi\omega/\kappa}.}
$$

The regulator fixes the branches and is essential to the sign of the thermal exponent.

Expand the outgoing annihilator as $b=\int d\omega'(\alpha_{\omega\omega'}^*a_{\omega'}-\beta_{\omega\omega'}^*a_{\omega'}^\dagger)$, including a complete set of incoming channels. The [canonical identities for a bosonic Bogoliubov transformation](../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md) express $[b,b^\dagger]=1$. For normalized outgoing [wave packets](../../../../../wave-packet.md), they give $\int(|\alpha|^2-|\beta|^2)\,d\omega'=1$. In the incoming [Fock vacuum](../../../../../fock-vacuum.md), the outgoing mean of the [particle number operator](../../../../../number-operator.md) is $N_\omega=\int|\beta|^2\,d\omega'$. Combining the two identities with the thermal ratio, in the late-time narrow-frequency packet limit, yields

$$
N_\omega=\frac1{e^{2\pi\omega/\kappa}-1},\qquad
\boxed{T_H=\frac\kappa{2\pi}=\frac1{8\pi M}.}
$$

[Wave packets](../../../../../wave-packet.md) avoid interpreting the divergent normalization of infinitely long continuum modes as a finite particle count. The temperature is the [Hawking temperature](../../../../../hawking-temperature.md), and the occupation is the zero-chemical-potential [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md). Restoring constants, the [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md) temperature is $T_H=\hbar c^3/(8\pi G M k_B)$ for physical mass $M$.

The preceding thermal occupation describes the horizon-originating channel before exterior scattering. The exterior angular and curvature potential partly reflects it. For a [scalar field](../../../../../scalar-field.md), the number flux at [future null infinity](../../../../../future-null-infinity.md) is consequently

$$
\frac{dN}{dt\,d\omega}=\frac1{2\pi}\sum_{\ell=0}^\infty(2\ell+1)\frac{\Gamma_\ell(\omega)}{e^{\omega/T_H}-1},
$$

where the [greybody factor](../../../../../greybody-factor.md) $\Gamma_\ell$ is the transmission probability of a partial wave. Multiplication by $\omega$ gives its energy flux. Thus the asymptotic spectrum has the thermal denominator but is not an exact blackbody spectrum. For fermionic fields the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) replace the minus sign in the occupation denominator by a plus sign, at the same [Hawking temperature](../../../../../hawking-temperature.md).

The relevant state is the [collapse vacuum for Hawking radiation](../../../../../collapse-vacuum-for-hawking-radiation.md): no incoming thermal bath at [past null infinity](../../../../../past-null-infinity.md), and regular short-distance behavior in freely falling coordinates at the forming [event horizon](../../../../../event-horizon.md). It predicts an outgoing flux, unlike equilibrium with a thermal bath on an eternal [black hole](../../../../../black-hole.md). The derivation uses [quantum field theory in curved spacetime](../../../../../quantum-field-theory-in-curved-spacetime.md) on a prescribed classical geometry; it does not require outgoing particles to follow forbidden classical paths out of the interior. Positive energy carried to infinity is accompanied, in the semiclassical description, by negative Killing-energy flux into the [black hole](../../../../../black-hole.md). Including that flux in slow backreaction decreases its [mass](../../../../../mass.md), giving [black-hole evaporation](../../../../../black-hole-evaporation.md).

The approximation applies to the late radiation of a large nonextremal [black hole](../../../../../black-hole.md) while its [surface gravity](../../../../../surface-gravity.md) changes slowly on a time scale $\kappa^{-1}$. Backward propagation involves very high locally measured frequencies, so the calculation assumes the usual regular short-distance quantum-field state. It determines the leading radiation and temperature, not the Planck-scale endpoint of [black-hole evaporation](../../../../../black-hole-evaporation.md). **The exponential horizon redshift forces positive/negative frequency mixing with a thermal ratio, giving outgoing Hawking radiation at $T_H=\kappa/(2\pi)$.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
