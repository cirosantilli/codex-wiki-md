<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Use peak [phasors](../../../../../phasor.md) with time dependence $e^{-i\omega t}$, real positive [electrical conductivity](../../../../../electrical-conductivity.md) $\sigma$, and absolute permeability $\mu_a=\mu\mu_0$. [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) and Faraday equations give

$$
\nabla\times\mathbf H=(\sigma-i\omega\epsilon\epsilon_0)\mathbf E=-i\omega\epsilon_0\epsilon'\mathbf E,\qquad \nabla\times\mathbf E=i\omega\mu_a\mathbf H,
$$

so **$\epsilon'=\epsilon+i\sigma/(\omega\epsilon_0)$**. The sign of the imaginary term follows from the stated time convention. For a transverse [plane wave](../../../../../plane-wave.md) in a homogeneous conductor,

$$
k^2=\mu_a\epsilon\epsilon_0\omega^2+i\mu_a\sigma\omega.
$$

In the good-conductor limit, choose the root that decays into $z>0$:

$$
\boxed{k=\frac{1+i}{\delta},\qquad \delta=\sqrt{\frac2{\sigma\mu_a\omega}}.}
$$

The electric [phasor](../../../../../phasor.md) and physical field are consequently $\widetilde E_x=E_0e^{(i-1)z/\delta}$ and $E_x=\operatorname{Re}[E_0e^{i(z/\delta-\omega t)-z/\delta}]$, as required. Tangential boundary matching sets $E_0$; it need not equal the incident [amplitude](../../../../../wave-amplitude.md).

[Faraday's law](../../../../../faraday-s-law-of-induction.md) fixes the [magnetic field](../../../../../magnetic-field-split.md), including its phase:

$$
\boxed{\widetilde{\mathbf H}=\frac{1+i}{\omega\mu_a\delta}E_0e^{(i-1)z/\delta}\widehat{\mathbf y}.}
$$

For real $E_0$ and $\psi=z/\delta-\omega t$, this means $H_y=E_0e^{-z/\delta}(\cos\psi-\sin\psi)/(\omega\mu_a\delta)$, with other components zero. The time-averaged [Poynting vector](../../../../../poynting-vector.md) is

$$
\boxed{\langle\mathbf N(z)\rangle=\frac12\operatorname{Re}(\widetilde{\mathbf E}\times\widetilde{\mathbf H}^{*})=\frac{|E_0|^2}{2\omega\mu_a\delta}e^{-2z/\delta}\widehat{\mathbf z}.}
$$

The [energy](../../../../../energy-split.md) entering a thin slab exceeds that leaving it by $-d\langle N_z\rangle/dz$ per unit [volume](../../../../../volume.md), giving

$$
p_{\rm loss}=\frac{|E_0|^2}{\omega\mu_a\delta^2}e^{-2z/\delta}=\boxed{\frac{\sigma|E_0|^2}{2}e^{-2z/\delta}.}
$$

Directly, $\mathbf J=\sigma\mathbf E$ and $\mathbf J\cdot\mathbf E=J^2/\sigma$ at each time. Therefore $\langle J^2/\sigma\rangle=\sigma|\widetilde E_x|^2/2$ is exactly this loss. The factors one half use peak rather than [root mean square](../../../../../root-mean-square.md) [phasors](../../../../../phasor.md); [amplitude](../../../../../wave-amplitude.md) decays over $\delta$, while intensity decays over $\delta/2$.

For a cold collisionless unmagnetized [plasma](../../../../../plasma-physics.md), [electron](../../../../../electron.md) inertia gives $\widetilde\sigma=i\epsilon_0\omega_p^2/\omega$ and real $\epsilon'=1-\omega_p^2/\omega^2$. Above the [plasma frequency](../../../../../plasma-frequency.md) the [wave](../../../../../wave-split.md) propagates without this resistive attenuation. Below it, a semi-infinite [plasma](../../../../../plasma-physics.md) supports an evanescent field with electric and magnetic components in quadrature and **zero mean inward [energy](../../../../../energy-split.md) flux**: the incident [energy](../../../../../energy-split.md) is reflected, not absorbed as [Joule heating](../../../../../joule-heating.md). [electron](../../../../../electron.md) [kinetic energy](../../../../../kinetic-energy.md) is reversibly stored, so the nondispersive [dielectric](../../../../../dielectric.md) field-energy formula alone is incomplete. Collisions introduce a real dissipative [electrical conductivity](../../../../../electrical-conductivity.md) and can produce absorption.[Section 9.7, equations 9.36–9.53, evanescence, phase quadrature and unit reflectance](../../../../../oscillations-and-waves-by-richard-fitzpatrick.md)

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
