<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**Molecular transport across gradients.** A [gas](../../../../../gas.md) can transport [momentum](../../../../../momentum-split.md), thermal [energy](../../../../../energy-split.md) and species abundance even when its average bulk [velocity](../../../../../velocity.md) is zero. [Molecules](../../../../../molecule-split.md) arriving at a point carry properties acquired near their preceding [collisions](../../../../../collision.md). A small gradient makes the populations arriving from opposite sides slightly different, producing transport from larger to smaller values of the carried property. A continuum transport law requires a [mean free path](../../../../../mean-free-path.md) $\lambda$ small compared with the gradient [length](../../../../../length.md), and relaxation times short compared with the observation [time](../../../../../time-in-physics.md).

For a dilute [hard-sphere gas](../../../../../hard-sphere-gas.md),

$$
\overline v=\sqrt{\frac{8k_BT}{\pi m}},\qquad
\lambda=\frac1{\sqrt2\,n\pi d^2},
$$

where $d$ is molecular [collision](../../../../../collision.md) diameter. Both [speed](../../../../../speed.md) and [collision](../../../../../collision.md) distance matter: high [speed](../../../../../speed.md) alone does not determine a transport coefficient.

A simple kinetic estimate makes the common structure explicit. For a quantity $a(y)$ carried per [particle](../../../../../particle-physics.md), a [molecule](../../../../../molecule-split.md) moving at angle $\theta$ to $+y$ brings approximately $a(y-\lambda\cos\theta)$. Expanding to first order and averaging an isotropic [velocity](../../../../../velocity.md) distribution gives

$$
J_a\sim n\overline v\left\langle\cos\theta\,[a(y)-\lambda\cos\theta\,a'(y)]\right\rangle
=-\frac13n\overline v\lambda\frac{da}{dy},
$$

since $\langle\cos\theta\rangle=0$ and $\langle\cos^2\theta\rangle=1/3$. This mean-free-path argument estimates the coefficients; a detailed [collision](../../../../../collision.md) calculation changes their numerical prefactors and distinguishes different relaxation rates.

**[Momentum](../../../../../momentum-split.md) transport and [viscosity](../../../../../dynamic-viscosity-split.md).** For a [shear flow](../../../../../shear-flow.md) with [mean](../../../../../expected-value-split.md) [velocity](../../../../../velocity.md) $U_x(y)$, the transported directed [momentum](../../../../../momentum-split.md) per [molecule](../../../../../molecule-split.md) is $mU_x$. The net flux of $x$ [momentum](../../../../../momentum-split.md) in the $+y$ direction is

$$
\Pi_{yx}=-\eta\frac{dU_x}{dy},\qquad
\boxed{\eta\sim\frac13nm\overline v\lambda.}
$$

Here $\eta$ is [dynamic viscosity](../../../../../dynamic-viscosity-split.md) in $\mathrm{Pa\,s}$. The associated shear [stress](../../../../../stress.md) on a material surface has the corresponding traction sign convention; the flux carries [momentum](../../../../../momentum-split.md) from the faster-moving layer towards the slower-moving one. The [kinematic viscosity](../../../../../kinematic-viscosity.md) is $\nu=\eta/(nm)$, with units $\mathrm{m^2\,s^{-1}}$. [Viscosity](../../../../../dynamic-viscosity-split.md) smooths [velocity](../../../../../velocity.md) gradients, and the lost ordered mechanical [energy](../../../../../energy-split.md) becomes [heat](../../../../../heat-split.md).

**[Heat](../../../../../heat-split.md) transport.** Let $c_v=d\varepsilon/dT$ be the thermal [heat capacity](../../../../../heat-capacity.md) _per [molecule](../../../../../molecule-split.md)_, in $\mathrm{J\,K^{-1}}$. Substituting $a=\varepsilon(T)$ gives [Fourier's law](../../../../../fourier-s-law.md),

$$
\mathbf J_Q=-\kappa\nabla T,\qquad
\boxed{\kappa\sim\frac13n c_v\overline v\lambda.}
$$

[Thermal conductivity](../../../../../thermal-conductivity.md) has units $\mathrm{W\,m^{-1}K^{-1}}$. For a [monatomic gas](../../../../../monatomic-gas.md), translational equipartition gives $c_v=3k_B/2$. Rotational or vibrational excitations in other [gases](../../../../../gas.md) can increase the [energy](../../../../../energy-split.md) carried per [molecule](../../../../../molecule-split.md), while [collisions](../../../../../collision.md) govern how those modes exchange [energy](../../../../../energy-split.md). A [temperature gradient](../../../../../temperature-gradient.md) can therefore be transported differently from directed [momentum](../../../../../momentum-split.md) even when the dimensional estimates look similar.

**Species transport.** For a dilute tracer or a mixture with prescribed total density and negligible bulk flow, [molecules](../../../../../molecule-split.md) diffuse down concentration gradients. The first-gradient number flux is [Fick's first law](../../../../../fick-s-first-law.md),

$$
\mathbf J_s=-D\nabla n_s,\qquad
\boxed{D\sim\frac13\overline v\lambda.}
$$

The [diffusivity](../../../../../diffusion-coefficient.md) $D$ has units $\mathrm{m^2\,s^{-1}}$; multiplying number flux by the species [mass](../../../../../mass.md) gives [mass](../../../../../mass.md) flux. More generally one uses [diffusion](../../../../../diffusion.md) flux relative to the mixture's bulk [velocity](../../../../../velocity.md) and specifies [mass](../../../../../mass.md) or mole fractions. The approximation is not a claim that an arbitrary pure-gas [pressure](../../../../../pressure-split.md) gradient can remain at rest while only a Fick flux acts. In a mixture, [collision](../../../../../collision.md) cross-sections and relative molecular [speeds](../../../../../speed.md), including the [reduced mass](../../../../../reduced-mass.md), determine the species diffusivities.

**Dependence on density and [temperature](../../../../../temperature-split.md).** The [kinetic estimates of gas transport coefficients](../../../../../kinetic-estimates-of-gas-transport-coefficients.md) predict, for fixed [collision](../../../../../collision.md) diameter and molecular [heat capacity](../../../../../heat-capacity.md),

$$
\eta\propto\frac{\sqrt{m k_BT}}{d^2},\qquad
\kappa\propto\frac{c_v}{d^2}\sqrt{\frac{k_BT}{m}},\qquad
D\propto\frac1{nd^2}\sqrt{\frac{k_BT}{m}}.
$$

Thus [dynamic viscosity](../../../../../dynamic-viscosity-split.md) and [thermal conductivity](../../../../../thermal-conductivity.md) are approximately density independent in the dilute continuum regime. Reducing density reduces the number of carriers but increases their [mean free path](../../../../../mean-free-path.md) in the same proportion. At fixed density all three estimates grow as $T^{1/2}$; at fixed [pressure](../../../../../pressure-split.md), $n=p/(k_BT)$ and

$$
\boxed{D\propto\frac{T^{3/2}}p,\qquad
\eta\propto T^{1/2},\qquad \kappa\propto T^{1/2}.}
$$

[Kinematic viscosity](../../../../../kinematic-viscosity.md) and [thermal diffusivity](../../../../../thermal-diffusivity.md) also grow roughly as $T^{3/2}/p$ at fixed [pressure](../../../../../pressure-split.md) in this model. Real interaction potentials make effective [collision](../../../../../collision.md) cross-sections [temperature](../../../../../temperature-split.md) dependent, and internal excitations change $c_v$. Dense-gas correlations and boundaries invalidate the simple cancellation. In particular, when the [mean free path](../../../../../mean-free-path.md) approaches the apparatus scale, transport becomes free molecular; it cannot be described by extending the same local, pressure-independent Fourier and [viscosity](../../../../../dynamic-viscosity-split.md) coefficients indefinitely.

**[Heat](../../../../../heat-split.md) [diffusion equation](../../../../../diffusion-equation-split.md).** For a stationary [gas](../../../../../gas.md) with constant [volumetric heat capacity](../../../../../volumetric-heat-capacity.md) $c=n c_v$, constant [thermal conductivity](../../../../../thermal-conductivity.md) and negligible compression [work](../../../../../work.md), the [energy](../../../../../energy-split.md) balance in any fixed [volume](../../../../../volume-thermodynamics.md) is

$$
\frac{d}{dt}\int_V cT\,dV=-\oint_{\partial V}\mathbf J_Q\cdot\widehat{\mathbf n}\,dA+\int_VH\,dV.
$$

Here $H$ is a possible [heat](../../../../../heat-split.md) generation rate per [volume](../../../../../volume-thermodynamics.md). The [divergence theorem](../../../../../divergence-theorem.md) and [Fourier's law](../../../../../fourier-s-law.md) yield

$$
\boxed{c\frac{\partial T}{\partial t}=\kappa\nabla^2T+H,
\qquad \frac{\partial T}{\partial t}=\alpha\nabla^2T+\frac Hc,
\qquad \alpha=\frac\kappa c.}
$$

[Thermal diffusivity](../../../../../thermal-diffusivity.md) $\alpha$ has units $\mathrm{m^2\,s^{-1}}$ and is of order $\overline v\lambda/3$. In a moving or compressing [gas](../../../../../gas.md), the [material derivative](../../../../../material-derivative.md), pressure-volume [work](../../../../../work.md) and viscous heating must also enter the internal-energy equation. The displayed pure [diffusion equation](../../../../../diffusion-equation-split.md) describes the approximation in which those effects are absent or negligible.

**Representative solutions.** With no source, a steady one-dimensional slab between [temperatures](../../../../../temperature-split.md) $T_a,T_b$ at $x=0,L$ has $T=T_a+(T_b-T_a)x/L$ and uniform [heat flux](../../../../../heat-flux-density.md) $-\kappa(T_b-T_a)/L$. Thus a constant spatial gradient transports [heat](../../../../../heat-split.md) without changing local [temperature](../../../../../temperature-split.md) in [time](../../../../../time-in-physics.md) when the boundaries continually supply and remove it.

For an infinite medium and an initial sinusoidal [temperature](../../../../../temperature-split.md) perturbation,

$$
\boxed{T(x,t)=T_b+A\cos(kx)e^{-\alpha k^2t}.}
$$

Short spatial wavelengths decay faster, and the characteristic smoothing [length](../../../../../length.md) after [time](../../../../../time-in-physics.md) $t$ is $\sqrt{\alpha t}$. A finite slab with both ends held at $T_b$ has a [sine](../../../../../sine.md) expansion with factors $e^{-\alpha(n\pi/L)^2t}$; its slowest relaxation [time](../../../../../time-in-physics.md) is $L^2/(\pi^2\alpha)$.

An instantaneous [heat](../../../../../heat-split.md) input $Q_A$ per unit transverse [area](../../../../../surface-area.md) at $x=0$ in an otherwise uniform infinite medium gives the [Gaussian](../../../../../normal-distribution.md) solution

$$
\boxed{T(x,t)-T_b=\frac{Q_A}{c\sqrt{4\pi\alpha t}}\exp\left(-\frac{x^2}{4\alpha t}\right),\quad t>0.}
$$

Its [integral](../../../../../integral-split.md) $\int c(T-T_b)dx=Q_A$ conserves the deposited [heat](../../../../../heat-split.md). The peak falls as $t^{-1/2}$ while its width grows as $\sqrt t$; [diffusion](../../../../../diffusion.md) redistributes [energy](../../../../../energy-split.md) instead of transporting a sharp front at a single [velocity](../../../../../velocity.md).

Finally, a semi-infinite body initially at $T_i$ and held at surface [temperature](../../../../../temperature-split.md) $T_s$ from $t=0$ has

$$
\boxed{T(x,t)=T_i+(T_s-T_i)\operatorname{erfc}\left(\frac{x}{2\sqrt{\alpha t}}\right),\quad x\geq0.}
$$

It has $T(0,t)=T_s$ and approaches $T_i$ far from the boundary at finite [time](../../../../../time-in-physics.md). These solutions demonstrate steady conduction, mode decay, spreading of localized [heat](../../../../../heat-split.md) and boundary-driven [diffusion](../../../../../diffusion.md). Their idealized behaviour at extremely short times or arbitrarily long distances must be interpreted within the continuum regime rather than as an assertion of instantaneous microscopic communication.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
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
