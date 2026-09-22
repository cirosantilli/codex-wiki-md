# Cold-plasma radio dispersion

↑ **Parent:** [Ionosphere](ionosphere.md)

Take a cold, unmagnetized, collisionless [plasma](plasma-physics.md) with uniform equilibrium [electron density](electron-density.md) $n_e$, fixed neutralizing [ions](ion.md), and a small [electromagnetic wave](electromagnetic-wave-split.md) that is a [transverse wave](transverse-wave.md). Cold means that thermal-motion corrections are neglected. For [electron mass](electron-mass.md) $m_e$, [elementary charge](elementary-charge.md) magnitude $e$ and [electric field](electric-field-split.md) $\mathbf E=\operatorname{Re}(\widehat{\mathbf E}e^{-i\omega t})$, the linear [Newton's second law](newton-s-second-law.md) equation is $m_e\dot{\mathbf v}=-e\mathbf E$. Thus $\widehat{\mathbf v}=-ie\widehat{\mathbf E}/(m_e\omega)$ and the [current density](current-density.md) is $\widehat{\mathbf J}=in_ee^2\widehat{\mathbf E}/(m_e\omega)$. Writing the induced [electric polarization](polarization-density.md) as $\widehat{\mathbf J}=-i\omega\widehat{\mathbf P}$ gives a negative [electric susceptibility](electric-susceptibility.md). With [vacuum permittivity](vacuum-permittivity.md) $\epsilon_0$,

$$
\epsilon_r=1-\frac{\omega_p^2}{\omega^2},\qquad
\omega_p^2=\frac{n_ee^2}{\epsilon_0m_e},\qquad
c^2k^2=\omega^2-\omega_p^2,\qquad
n^2=\frac{c^2k^2}{\omega^2}=1-\frac{\omega_p^2}{\omega^2}.
$$

The [plasma frequency](plasma-frequency.md) $\omega_p$ controls the response. For $\omega>\omega_p$, the propagating branch has real [refractive index](refractive-index.md) $0<n<1$. For $\omega<\omega_p$, this homogeneous model has an [evanescent wave](evanescent-wave.md), not an ordinary propagating wave with a negative real [refractive index](refractive-index.md). In a slowly varying vertical profile, a normally incident ray approaches a turning region where $\omega_p(z)=\omega$; the geometrical-ray approximation fails right at that region. At oblique incidence the conserved horizontal [wave vector](wavevector.md) changes the turning condition. A smooth density gradient can therefore return a [skywave](skywave.md) without a mirror or a layer of metal.

For a homogeneous propagating section, direct [differentiation](differentiation.md) of the [dispersion relation](dispersion-relation-split.md) gives

$$
v_{\rm ph}=\frac{\omega}{k}=\frac c n>c,\qquad
v_g=\frac{d\omega}{dk}=cn<c,\qquad
n_g=n+\omega\frac{dn}{d\omega}=\frac1n.
$$

A [phase velocity](phase-velocity.md) greater than $c$ does not send information faster than $c$. Here a narrow [wave packet](wave-packet.md) has [group velocity](group-velocity.md) $v_g$, while the full causal response must still respect [special relativity](special-relativity-split.md). Even this stripped-down [plasma](plasma-physics.md) is strongly dispersive near its [plasma frequency](plasma-frequency.md). In the actual [ionosphere](ionosphere.md), collisions produce absorption, and the [magnetic field](magnetic-field-split.md) of [Earth](earth.md) changes the response with direction and [wave polarization](polarization-waves.md); a single real scalar $n$ cannot capture all of that behavior.

**Table of contents**

- [Ionospheric virtual height](ionospheric-virtual-height.md)

## ↑ Ancestors (6)

1. [Ionosphere](ionosphere.md)
2. [Upper atmosphere](upper-atmosphere.md)
3. [Geophysics](geophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ionosphere](ionosphere.md)
- [Ionospheric virtual height](ionospheric-virtual-height.md)
