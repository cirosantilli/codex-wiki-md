<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For photon-dominated inertia, $R\gg1$ and $c_s^2\simeq1/3$. The baryon expansion and pressure terms are suppressed by $1/R$. Ignoring metric driving as stipulated, the common-velocity Euler equation is $\theta'=-\delta_\gamma/4+\sigma_\gamma$. Differentiating the photon continuity equation gives

$$
\boxed{\delta_\gamma''+\frac13k^2\delta_\gamma-\frac43k^2\sigma_\gamma=0.}
$$

This limit is compatible with a matter-dominated background: [cold dark matter](../../../../../../cold-dark-matter.md) can dominate the expansion while photons dominate the inertia of the photon-baryon subsystem.

In the first nonzero quadrupole approximation, neglect $\sigma_\gamma'$ relative to its collision damping. The shear equation gives

$$
\sigma_\gamma\simeq-\frac4{15}\tau_c k^2\theta=-\frac15\tau_c\delta_\gamma',\qquad\tau_c=\kappa^{-1}.
$$

Substitution yields the [shear-only photon diffusion damping](../../../../../../shear-only-photon-diffusion-damping.md) equation

$$
\boxed{\delta_\gamma''+\frac4{15}\tau_c k^2\delta_\gamma'+\frac13k^2\delta_\gamma=0.}
$$

The sign of the first-derivative term is positive, so finite photon mean free time damps acoustic energy.

Put $\omega=k/\sqrt3$ and $\gamma(\tau)=4k^2\tau_c(\tau)/15$. For constant $\tau_c$, the characteristic roots are $-\gamma/2\pm i\sqrt{\omega^2-\gamma^2/4}$. The frequency shift begins at second order in the mean free time. To the requested order the general solution is

$$
\delta_\gamma=e^{-2k^2\tau_c(\tau-\tau_i)/15}
[A\cos(\omega(\tau-\tau_i))+B\sin(\omega(\tau-\tau_i))]+O(\tau_c^2),
$$

where the error describes the frequency expansion at fixed $k$ and time interval. Keeping the exponential retains the accumulated damping rather than expanding away a possibly important effect.

For a general time-dependent coefficient, a first-order solution with prescribed initial conditions can also be written as

$$
\delta_\gamma(\tau)=\delta_0(\tau)
-\int_{\tau_i}^{\tau}\frac{\sin[\omega(\tau-s)]}{\omega}\gamma(s)\delta_0'(s)\,ds+O(\tau_c^2),
$$

where $\delta_0=A\cos[\omega(\tau-\tau_i)]+B\sin[\omega(\tau-\tau_i)]$. Substitution verifies that the integral solves the oscillator forced by $-\gamma\delta_0'$, and its value and first derivative vanish initially. This gives the general first-order result without assuming arbitrary time dependence may be absorbed exactly into an exponential.

To obtain the slowly varying subhorizon form, set $\delta_\gamma=e^{-G}y$ with $G'=\gamma/2$. The exact transformed equation is

$$
y''+[\omega^2-\tfrac12\gamma'-\tfrac14\gamma^2]y=0.
$$

Dropping the quadratic term alone leaves $\omega^2-\gamma'/2$, so slow variation is also needed. When $k\gg\mathcal H$, $k\tau_c\ll1$, and the mean free time changes on an expansion timescale, $|\gamma'|/\omega^2\ll1$. The [WKB method](../../../../../../wkb-method.md) solution has local frequency $\Omega=(\omega^2-\gamma'/2)^{1/2}$ and prefactor $\Omega^{-1/2}$. At leading acoustic order both reduce to constants; the small derivative corrections to phase and prefactor can be neglected. This [slowly varying shear-damped photon oscillator](../../../../../../slowly-varying-shear-damped-photon-oscillator.md) therefore gives

$$
\boxed{\delta_\gamma(k,\tau)\simeq[A(k)\cos(k\tau/\sqrt3)+B(k)\sin(k\tau/\sqrt3)]e^{-k^2/k_D^2(\tau)},\qquad
k_D^{-2}(\tau)=\frac2{15}\int_{\tau_i}^{\tau}\tau_c(s)\,ds.}
$$

A change in the phase origin is absorbed into $A,B$. At zero mean free time the damping vanishes; as time passes the diffusion length grows and $k_D$ decreases. The coefficient is that of the question's isotropic-scattering, shear-only truncation, not the polarization-inclusive full [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) formula.

If ionization remains approximately constant during [matter domination](../../../../../../matter-domination.md), $n_e\propto a^{-3}$, so $\tau_c\propto a^2\propto\tau^4$. Away from the lower limit this gives

$$
k_D^{-2}\simeq\frac2{75}\tau\tau_c(\tau),\qquad k_D\propto\tau^{-5/2}.
$$

Near recombination the rapidly changing ionization fraction and eventual failure of [tight coupling](../../../../../../tight-coupling-approximation.md) require the full hierarchy; the integral formula specifies the damping accumulated during the regime used here.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
