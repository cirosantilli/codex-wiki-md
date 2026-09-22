<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mathbf x$ for a [comoving coordinate](../../../../../../comoving-coordinate.md), $\mathbf u$ for the [peculiar velocity](../../../../../../peculiar-velocity.md), $H=\dot a/a$ for the [Hubble parameter](../../../../../../hubble-parameter.md), and $\delta=\delta\rho/\bar\rho$ for the [density contrast](../../../../../../density-contrast.md). For a homogeneous self-gravitating fluid, the linearized [continuity equation](../../../../../../continuity-equation.md), [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md), and [cosmological Poisson equation](../../../../../../cosmological-poisson-equation.md) are

$$
\dot\delta=-\frac1a\nabla\cdot\mathbf u,
\qquad
\dot{\mathbf u}+H\mathbf u=-\frac{c_s^2}{a}\nabla\delta-\frac1a\nabla\phi,
\qquad
\nabla^2\phi=4\pi G a^2\bar\rho\delta.
$$

Here $c_s$ is the physical [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md), gradients refer to [comoving coordinates](../../../../../../comoving-coordinate.md), and the homogeneous background force has already been subtracted. Differentiating the first equation and eliminating $\mathbf u$ and $\phi$ gives

$$
\ddot\delta+2H\dot\delta-\frac{c_s^2}{a^2}\nabla^2\delta-4\pi G\bar\rho\delta=0.
$$

A [Fourier mode](../../../../../../fourier-mode.md) with comoving [wavenumber](../../../../../../wavenumber.md) $k$ therefore obeys

$$
\ddot\delta_k+2H\dot\delta_k+
\left(\frac{c_s^2k^2}{a^2}-4\pi G\bar\rho\right)\delta_k=0.
$$

The [Jeans wavenumber](../../../../../../jeans-wavenumber.md) occurs where the coefficient in parentheses vanishes. Since a comoving [wavelength](../../../../../../wavelength.md) is $2\pi/k$, the result is

$$
\boxed{k_J=\frac{a\sqrt{4\pi G\bar\rho}}{c_s},\qquad
\lambda_J^{\rm com}=\frac{c_s}{a}\sqrt{\frac{\pi}{G\bar\rho}}.}
$$

Below this [comoving Jeans length](../../../../../../comoving-jeans-length.md), pressure restores a displaced fluid element: there are [acoustic waves](../../../../../../acoustic-wave.md) rather than growing [Jeans instability](../../../../../../jeans-instability.md). In a static background they oscillate; expansion changes their amplitude and frequency, and dissipation can damp them. Pressure support alone does not erase them. In the pre-recombination [photon-baryon fluid](../../../../../../photon-baryon-fluid.md), [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) supplies a separate erasure mechanism.

For collisionless matter, replace the [sound speed](../../../../../../speed-of-sound.md) by a characteristic [velocity dispersion](../../../../../../velocity-dispersion.md). For an isotropic [Maxwell-Boltzmann velocity distribution](../../../../../../maxwell-boltzmann-velocity-distribution.md), defining $\sigma^2=\langle u_x^2\rangle=\langle|\mathbf u|^2\rangle/3$, the static collisionless marginal-stability calculation gives

$$
\boxed{\lambda_{J,\rm collisionless}^{\rm com}
=\frac{\sigma}{a}\sqrt{\frac{\pi}{G\bar\rho}}
=\frac{v_{\rm rms}}a\sqrt{\frac{\pi}{3G\bar\rho}}.}
$$

The coefficient depends on the distribution and the convention for [velocity dispersion](../../../../../../velocity-dispersion.md). Small-scale suppression is now [collisionless free streaming](../../../../../../free-streaming.md) and [phase mixing](../../../../../../phase-mixing.md), rather than collisional [acoustic waves](../../../../../../acoustic-wave.md). An instantaneous [collisionless Jeans length](../../../../../../collisionless-jeans-length.md) must be distinguished from the accumulated comoving distance $\int v\,dt/a$ traveled since decoupling.

For the requested thermal histories, an [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) describes the matter-era limit: it cannot literally also have a radiation-dominated epoch. Interpret the question as a spatially flat universe with negligible [cosmological constant](../../../../../../cosmological-constant.md), passing from [radiation domination](../../../../../../radiation-domination.md), $a\propto t^{1/2}$, to [matter domination](../../../../../../matter-domination.md), $a\propto t^{2/3}$. For the usual schematic dynamical Jeans scale use $\bar\rho_{\rm tot}$ in the estimate, so

$$
\lambda_{\rm dyn}^{\rm com}\propto
\begin{cases}
c_s a,&t\ll t_{\rm eq},\quad\bar\rho_{\rm tot}\propto a^{-4},\\
c_s a^{1/2},&t\gg t_{\rm eq},\quad\bar\rho_{\rm tot}\propto a^{-3}.
\end{cases}
$$

Near the [particle horizon](../../../../../../particle-horizon.md) a relativistic perturbation calculation replaces the Newtonian derivation; the scaling estimate still identifies the relevant sound-crossing or streaming scale.

Before [cosmological recombination](../../../../../../recombination-cosmology.md), [adiabatic initial conditions](../../../../../../adiabatic-initial-conditions.md) keep the entropy per [baryon](../../../../../../baryon.md) fixed in the tightly coupled [photon-baryon fluid](../../../../../../photon-baryon-fluid.md). With $R_b=3\bar\rho_b/(4\bar\rho_\gamma)\propto a$, its [photon-baryon sound speed](../../../../../../photon-baryon-sound-speed.md) is

$$
c_s^2=\frac{c^2}{3(1+R_b)}.
$$

For example, this follows from $\delta\rho_\gamma/\bar\rho_\gamma=(4/3)\delta\rho_b/\bar\rho_b$ and $\delta P=c^2\delta\rho_\gamma/3$. In the radiation-dominated limit $R_b\ll1$, $c_s\simeq c/\sqrt3$; in the strongly baryon-loaded matter-era limit $R_b\gg1$, $c_s\propto a^{-1/2}$. Thus the [baryon Jeans length across recombination](../../../../../../baryon-jeans-length-across-recombination.md) has the asymptotic history

$$
\boxed{\lambda_{J,b}^{\rm com}\propto
\begin{cases}
a\propto t^{1/2},&t\ll t_{\rm eq},\\
\text{approximately constant},&t_{\rm eq}\ll t<t_{\rm rec},\\
a^{-1/2}\propto t^{-1/3},&t>t_{\rm rec}\text{ with adiabatic gas cooling}.
\end{cases}}
$$

The transition to the plateau is smooth: retaining $1+R_b$ gives $\lambda_{J,b}^{\rm com}\propto a^{1/2}/\sqrt{1+R_b}$ in [matter domination](../../../../../../matter-domination.md). If baryon loading is still small, this intermediate segment instead rises as $a^{1/2}$ until loading becomes important.

At [photon decoupling](../../../../../../photon-decoupling.md), radiation ceases to provide pressure support to the [baryons](../../../../../../baryon.md), so the [sound speed](../../../../../../speed-of-sound.md) drops from the coupled-fluid value to that of a nonrelativistic [ideal gas](../../../../../../ideal-gas.md), $c_{s,b}^2=\gamma k_BT_b/(\mu m_p)$, with $\gamma=5/3$. The drop in [comoving Jeans length](../../../../../../comoving-jeans-length.md) at fixed density is the same ratio of [sound speeds](../../../../../../speed-of-sound.md), typically several orders of magnitude. Subsequently an [isentropic process](../../../../../../isentropic-process.md) gives $T_b\propto\bar\rho_b^{\gamma-1}\propto a^{-2}$, so $c_{s,b}\propto a^{-1}$ and $\lambda_{J,b}^{\rm com}\propto a^{-1/2}$. Residual energy exchange through [Compton scattering](../../../../../../compton-scattering.md) can initially keep $T_b\propto a^{-1}$, producing a short approximately flat gas segment before the decreasing segment. The idealized sketch assumes immediate adiabatic cooling:

```
log(comoving baryon Jeans scale)
  ^
  |                   __________________
  |                 /                   |
  |               /                     |  loss of photon pressure
  |             /                       |
  |           /                         +---\
  |         /                                \
  +-------------------|-----------------|----------> log(time)
                    t_eq              t_rec
        slope 1/2          slope ~0        slope -1/3
```

For the [cold-dark-matter kinetic Jeans scale](../../../../../../cold-dark-matter-kinetic-jeans-scale.md), take the stated toy history to mean that collisions maintain a particle [temperature](../../../../../../temperature.md) equal to the photon [temperature](../../../../../../temperature.md) until [kinetic decoupling](../../../../../../kinetic-decoupling.md). This is an assumption about thermal coupling; a negligible collision rate after decoupling makes the subsequent treatment collisionless. Assume the ordering $t_{\rm NR}<t_{\rm dec}<t_{\rm eq}<t_{\rm rec}$. While relativistic, the characteristic particle speed is constant; while nonrelativistic but thermally coupled, $\sigma\propto\sqrt T\propto a^{-1/2}$; after [kinetic decoupling](../../../../../../kinetic-decoupling.md), particle momentum redshifts as $a^{-1}$ and $\sigma\propto a^{-1}$. Combining these with the background dynamical density gives

$$
\boxed{\lambda_{\rm dyn,CDM}^{\rm com}\propto
\begin{cases}
a\propto t^{1/2},&t<t_{\rm NR},\\
a^{1/2}\propto t^{1/4},&t_{\rm NR}<t<t_{\rm dec},\\
\text{constant},&t_{\rm dec}<t<t_{\rm eq},\\
a^{-1/2}\propto t^{-1/3},&t>t_{\rm eq}.
\end{cases}}
$$

There is no sudden change at [cosmological recombination](../../../../../../recombination-cosmology.md): [cold dark matter](../../../../../../cold-dark-matter.md) has already decoupled. Its small initial [velocity dispersion](../../../../../../velocity-dispersion.md) makes its suppression scale much smaller than the pre-recombination [baryon](../../../../../../baryon.md) scale.

```
log(comoving CDM dynamical Jeans scale)
  ^
  |                        _______________
  |                    ___/               \
  |                ___/                    \       no jump
  |              /                          \      at t_rec
  |            /                             \
  +-----------|------------|--------------|----|------> log(time)
            t_NR         t_dec          t_eq t_rec
   slope 1/2    slope 1/4       slope 0       slope -1/3
```

The density convention matters. If one instead defines a species' self-gravitating [collisionless Jeans length](../../../../../../collisionless-jeans-length.md) using only its own nonrelativistic density $\bar\rho_m\propto a^{-3}$, its thermally coupled segment is constant and its decoupled segment decreases as $a^{-1/2}$ even during [radiation domination](../../../../../../radiation-domination.md). The constant radiation-era segment in the second sketch is the usual instantaneous background dynamical streaming estimate, not an exact single-species self-gravity threshold. A complete multicomponent calculation uses the separate perturbation equations and their combined [cosmological Poisson equation](../../../../../../cosmological-poisson-equation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
