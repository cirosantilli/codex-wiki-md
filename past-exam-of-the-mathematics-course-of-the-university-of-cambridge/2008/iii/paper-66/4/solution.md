<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Hawking radiation](../../../../../hawking-radiation.md) is a prediction of [quantum field theory in curved spacetime](../../../../../quantum-field-theory-in-curved-spacetime.md), not of classical collapse alone. Consider a free massless [Klein-Gordon field](../../../../../klein-gordon-field.md) in the [collapse vacuum for Hawking radiation](../../../../../collapse-vacuum-for-hawking-radiation.md): initially no incoming particles from [past null infinity](../../../../../past-null-infinity.md), with the short-distance state regular for freely falling observers through the forming [event horizon](../../../../../event-horizon.md). At late times use the approximately fixed exterior [Schwarzschild metric](../../../../../schwarzschild-spacetime.md); neglect backreaction during the observation interval. First set $G=c=\hbar=k_B=1$.

The exterior metric has $f(r)=1-2M/r$. Introduce the [tortoise coordinate](../../../../../tortoise-coordinate.md) and outgoing and ingoing null coordinates,

$$
r_*=r+2M\log\left(\frac r{2M}-1\right),\qquad u=t-r_*,\qquad v=t+r_*.
$$

The [surface gravity](../../../../../surface-gravity.md) is $\kappa=1/(4M)$. The logarithm in $r_*$ makes a late escaping ray spend a long exterior coordinate time close to the [event horizon](../../../../../event-horizon.md). One of the regular outgoing [Kruskal–Szekeres coordinates](../../../../../kruskal-szekeres-coordinates.md) is proportional to $-e^{-\kappa u}$. Smooth propagation backwards through the collapsing body relates this regular coordinate to the incoming coordinate on [past null infinity](../../../../../past-null-infinity.md). If $v_H$ labels the last ray able to escape, the late-time [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md) is consequently

$$
\boxed{v_H-v=C e^{-\kappa u},\qquad
u(v)=-\frac1\kappa\log\left(\frac{v_H-v}{C}\right),\quad C>0.}
$$

Here the symbol $u(v)$ is the outgoing retarded time evaluated on the ray; the first equation is the leading asymptotic relation, with subleading corrections that vanish at late times. The constant $C$ depends on collapse history, whereas the exponential rate is determined by the final [surface gravity](../../../../../surface-gravity.md). The relation follows from a nondegenerate [Killing horizon](../../../../../killing-horizon.md); a linear ray map would not have the same effect.

An outgoing positive-frequency mode at [future null infinity](../../../../../future-null-infinity.md) behaves as $p_\omega\sim e^{-i\omega u}/\sqrt{4\pi\omega}$, where $\omega>0$ is measured with respect to the asymptotic stationary time. In the near-horizon [geometric optics](../../../../../geometrical-optics.md) approximation its backward-propagated form on [past null infinity](../../../../../past-null-infinity.md) is

$$
p_\omega(v)\sim\frac{1}{\sqrt{4\pi\omega}}\,
\Theta(v_H-v)\left(\frac{v_H-v}{C}\right)^{i\omega/\kappa}.
$$

This is not purely positive frequency in $v$. Its decomposition into incoming positive-frequency modes $f_{\omega'}\sim e^{-i\omega'v}/\sqrt{4\pi\omega'}$ and their complex conjugates is a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md):

$$
p_\omega=\int_0^\infty\left(\alpha_{\omega\omega'}f_{\omega'}+\beta_{\omega\omega'}f_{\omega'}^*\right)d\omega'.
$$

The coefficients follow from the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md), or equivalently from the [Fourier transform](../../../../../fourier-transform.md) with the indicated flux normalization. Writing $y=v_H-v$ and $a=\omega/\kappa$, the two Fourier integrals, after a convergence regulator, are

$$
I_\pm=\int_0^\infty y^{ia}e^{-(\epsilon\pm i\omega')y}\,dy
=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia},\qquad\epsilon>0.
$$

The equality is the defining integral of the [Gamma function](../../../../../gamma-function.md), continued to these arguments from the right half-plane. Up to phases of unit modulus, $\alpha$ is $\sqrt{\omega'/\omega}\,I_+/(2\pi)$ and $\beta$ is $\sqrt{\omega'/\omega}\,I_-/(2\pi)$. Taking $\epsilon\downarrow0$ on the principal branches, the arguments of $\epsilon\pm i\omega'$ tend to $\pm\pi/2$. Thus $|I_+|\propto e^{\pi a/2}$ and $|I_-|\propto e^{-\pi a/2}$, giving the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md)

$$
\boxed{\frac{|\beta_{\omega\omega'}|^2}{|\alpha_{\omega\omega'}|^2}=e^{-2\pi\omega/\kappa}.}
$$

In particular, using $|\Gamma(1+ia)|^2=\pi a/\sinh(\pi a)$,

$$
|\beta_{\omega\omega'}|^2=\frac{1}{2\pi\kappa\omega'}\frac{1}{e^{2\pi\omega/\kappa}-1}.
$$

The collapse-dependent phases and $C$ disappear from the ratio. The [canonical identities for a bosonic Bogoliubov transformation](../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md) state that the positive-frequency norm minus the negative-frequency norm is one for a normalized outgoing mode. Combining that identity with the thermal ratio yields the late-time mean occupation

$$
\boxed{\langle N_\omega\rangle=\frac{1}{e^{2\pi\omega/\kappa}-1},\qquad
T_H=\frac{\kappa}{2\pi}=\frac{1}{8\pi M}.}
$$

These are the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) and the [Hawking temperature](../../../../../hawking-temperature.md). Strictly, monochromatic modes have delta-function normalization, and $\int d\omega'\,|\beta_{\omega\omega'}|^2$ contains the infinite-duration divergence $\int d\omega'/\omega'$. Normalized [wave packets](../../../../../wave-packet.md) with a finite frequency band and a finite retarded-time window remove this artifact. For sufficiently late packets the occupation is the frequency average of the displayed thermal factor, tending to it for a narrow band. Fermionic fields instead give the corresponding denominator $e^{2\pi\omega/\kappa}+1$ because their canonical normalization uses anticommutators.

Four-dimensional propagation adds an important qualification to the word thermal. Separation of the massless [Klein-Gordon equation](../../../../../klein-gordon-equation.md) into [spherical harmonics](../../../../../spherical-harmonic.md) gives an exterior radial scattering potential

$$
V_\ell(r)=f(r)\left(\frac{\ell(\ell+1)}{r^2}+\frac{2M}{r^3}\right).
$$

Only a fraction $\Gamma_\ell(\omega)$ of the outgoing mode is transmitted to [future null infinity](../../../../../future-null-infinity.md); this is the [greybody factor](../../../../../greybody-factor.md). The scalar particle flux there is

$$
\boxed{\frac{dN}{du\,d\omega}=\frac{1}{2\pi}\sum_{\ell=0}^\infty
(2\ell+1)\frac{\Gamma_\ell(\omega)}{e^{8\pi M\omega}-1}.}
$$

The factor $2\ell+1$ counts the angular modes, and multiplication by $\omega$ gives the spectral [energy](../../../../../energy.md) flux. An observer at infinity therefore receives an outgoing thermal population filtered by curvature scattering, rather than an exact unfiltered blackbody spectrum. In physical units, for mass $M_{\mathrm{phys}}$,

$$
\boxed{T_H=\frac{\hbar c^3}{8\pi G k_BM_{\mathrm{phys}}}.}
$$

There is no incoming thermal bath in the [collapse vacuum for Hawking radiation](../../../../../collapse-vacuum-for-hawking-radiation.md). The outgoing flux has positive [Killing energy](../../../../../killing-energy.md); its counterpart inside the [event horizon](../../../../../event-horizon.md) can carry negative [Killing energy](../../../../../killing-energy.md). Including the expectation value of the [stress-energy tensor](../../../../../stress-energy-tensor.md) in the gravitational evolution allows the mass to decrease. The fixed-background derivation describes the slowly evolving semiclassical regime and does not determine the endpoint of evaporation. Quantum expectation values need not satisfy the classical [null energy condition](../../../../../null-energy-condition.md), so this loss of area is not a contradiction of the classical [second law of black-hole mechanics](../../../../../second-law-of-black-hole-mechanics.md). The essential late-time universality is the combination of a regular initial quantum state and the exponential redshift at the newly formed [event horizon](../../../../../event-horizon.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
