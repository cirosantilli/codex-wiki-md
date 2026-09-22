<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $M=M_1+M_2$, $a=a_1+a_2$, and $\mu=M_1M_2/M$, the [reduced mass](../../../../../reduced-mass.md). In the [center of mass](../../../../../center-of-mass.md) frame, $a_1=aM_2/M$ and $a_2=aM_1/M$. Both components of the [circular orbit](../../../../../circular-orbit.md) have the same [angular velocity](../../../../../angular-velocity.md) $\Omega$. Thus their total orbital [angular momentum](../../../../../angular-momentum.md) is

$$
J=(M_1a_1^2+M_2a_2^2)\Omega=\mu a^2\Omega.
$$

Using [Kepler's third law](../../../../../kepler-s-third-law.md), $\Omega^2=GM/a^3$, and the [orbital period](../../../../../orbital-period.md) $P=2\pi/\Omega$, gives the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md)

$$
\boxed{J=\mu\sqrt{GMa}=\frac{G^{2/3}P^{1/3}M_1M_2}{(2\pi)^{1/3}M^{1/3}}.}
$$

Take $\dot M_1<0$, so $\dot M_2=-f\dot M_1$ and $\dot M=(1-f)\dot M_1$. A parcel in an isotropic [stellar wind](../../../../../stellar-wind.md) has, on average, the [donor star](../../../../../donor-star.md)'s orbital velocity. Its wind velocity relative to the [donor star](../../../../../donor-star.md) averages to zero, so its mean specific orbital [angular momentum](../../../../../angular-momentum.md) about the [center of mass](../../../../../center-of-mass.md) is $j_1=a_1^2\Omega$. The escaping mass per unit time is $-(1-f)\dot M_1$. With negligible stellar spin, no additional wind torque, and internal redistribution of the [angular momentum](../../../../../angular-momentum.md) of retained matter, [donor-wind angular-momentum loss](../../../../../donor-wind-angular-momentum-loss.md) therefore gives

$$
\boxed{\dot J=(1-f)\dot M_1a_1^2\Omega<0\quad(f<1),}\qquad
\frac{\dot J}{J}=(1-f)\dot M_1\frac{M_2}{M_1M}.
$$

Isotropy is in the [donor star](../../../../../donor-star.md)'s frame: it does not make the escaping orbital [angular momentum](../../../../../angular-momentum.md) vanish. This is also different from [isotropic re-emission from a binary star](../../../../../isotropic-re-emission-from-a-binary-star.md), where matter escapes from the accretor.

Logarithmically differentiate the expression for $J$ along a slowly evolving sequence of [circular orbits](../../../../../circular-orbit.md):

$$
\frac{\dot J}{J}=\frac13\frac{\dot P}{P}+\frac{\dot M_1}{M_1}+\frac{\dot M_2}{M_2}-\frac13\frac{\dot M}{M}.
$$

Substitution of the [donor-wind angular-momentum loss](../../../../../donor-wind-angular-momentum-loss.md) and mass rates gives

$$
\frac{\dot P}{P}=3\dot M_1\left[\frac{(1-f)M_2}{M_1M}-\frac1{M_1}+\frac f{M_2}\right]+(1-f)\frac{\dot M_1}{M}
=\left[-\frac{3f}{M_1}+\frac{3f}{M_2}-\frac{2(1-f)}M\right]\dot M_1.
$$

For **constant $f$**, the last expression is $-3f\,d\log M_1/dt-3\,d\log M_2/dt-2\,d\log M/dt$. Hence the [period invariant for constant-fraction donor-wind mass loss](../../../../../period-invariant-for-constant-fraction-donor-wind-mass-loss.md) is

$$
\boxed{PM_1^{3f}M_2^3M^2=\text{constant},\qquad P\propto M_1^{-3f}M_2^{-3}M^{-2}.}
$$

For a time-dependent $f$, the differential equation still holds, but this integrated power law does not. At $f=1$ it reduces to the [period-product invariant for conservative mass transfer](../../../../../period-product-invariant-for-conservative-mass-transfer.md); at $f=0$, $M_2$ is constant and $PM^2$ is constant, as in [Jeans-mode mass loss](../../../../../jeans-mode-mass-loss.md).

Set the [binary mass ratio](../../../../../binary-mass-ratio.md) $q=M_1/M_2$. Since $a^3=GMP^2/(4\pi^2)$, the [Kepler third law](../../../../../kepler-s-third-law.md) and the preceding [orbital period](../../../../../orbital-period.md) derivative imply

$$
\frac{\dot a}{a}=\frac{\dot M_1}{M_1}\left[2f(q-1)-\frac{(1-f)q}{1+q}\right].
$$

The specified approximation to the [Roche lobe](../../../../../roche-lobe.md) gives $\log R_L=\log(0.46)+\log a+\frac13(\log M_1-\log M)$. Consequently the [donor-wind Roche-lobe response](../../../../../donor-wind-roche-lobe-response.md) is

$$
\frac{\dot R_L}{R_L}=\frac{\dot M_1}{M_1}\left[2f(q-1)+\frac13-\frac{4(1-f)q}{3(1+q)}\right]
=\frac{\dot M_1}{M_1}\left\{f\left[2q+\frac{4q}{3(1+q)}-2\right]+\frac13-\frac{4q}{3(1+q)}\right\}.
$$

This is a local [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md), so it remains valid instantaneously even if $f$ varies.

The [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) of $R_1\propto M_1^{-n}$ is $\zeta_*=-n$. Maintaining [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) in exact contact requires $\dot R_1/R_1=\dot R_L/R_L$, yielding

$$
\boxed{f\left[2q+\frac{4q}{3(1+q)}-2\right]=\frac{4q}{3(1+q)}-n-\frac13.}
$$

For a precise [feasibility of donor-wind binary contact](../../../../../feasibility-of-donor-wind-binary-contact.md) test, put $\zeta_0=\frac13-\frac{4q}{3(1+q)}$ and $\zeta_1=2q-\frac53$. The [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is $\zeta_L=(1-f)\zeta_0+f\zeta_1$. Thus **a permitted contact fraction exists exactly when**

$$
\boxed{\min(\zeta_0,\zeta_1)\le -n\le\max(\zeta_0,\zeta_1).}
$$

Unless $A=\zeta_1-\zeta_0=2q+4q/[3(1+q)]-2$ vanishes, the required fraction is $f=(-n-\zeta_0)/A$. At $q=(\sqrt{10}-1)/3$, both limiting [Roche-lobe radius response exponents](../../../../../roche-lobe-radius-response-exponent.md) coincide: contact is possible for any $f$ only if $n=5/3-2q$, and for no $f$ otherwise.

The sign of the overfilling change resolves the failure of contact:

$$
\frac{d}{dt}\log\frac{R_1}{R_L}=(\zeta_*-\zeta_L)\frac{\dot M_1}{M_1}.
$$

If $\zeta_*>\max(\zeta_0,\zeta_1)$, mass loss makes the [donor star](../../../../../donor-star.md) underfill its [Roche lobe](../../../../../roche-lobe.md): **the system detaches and contact-driven transfer stops**. If $\zeta_*<\min(\zeta_0,\zeta_1)$, mass loss increases the overfilling: **transfer is destabilized**, and rapid transfer or a [common envelope](../../../../../common-envelope.md) may result. Calling this a failure of [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) specifically requires $-n$ to be the adiabatic [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md); a thermal or equilibrium response concerns a different timescale. Additional [angular momentum](../../../../../angular-momentum.md) losses or intrinsic stellar expansion can change these outcomes by changing the contact equation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
