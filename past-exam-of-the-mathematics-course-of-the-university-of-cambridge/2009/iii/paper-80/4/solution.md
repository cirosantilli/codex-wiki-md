<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $a(t)$ be the particle radius and $\Delta T=T_s-T_\infty>0$ the supercooling. Use [spherical symmetry](../../../../../spherical-symmetry.md), constant thermal properties, equal phase densities $\rho$, and negligible fluid advection. Let $\mathcal L$ be [latent heat](../../../../../latent-heat.md) per unit mass, $c_p$ the liquid specific heat, $k_\ell$ its [thermal conductivity](../../../../../thermal-conductivity.md) and $\kappa=k_\ell/(\rho c_p)$ its [thermal diffusivity](../../../../../thermal-diffusivity.md). The exterior [temperature](../../../../../temperature.md) satisfies the radial [heat equation](../../../../../heat-equation.md)

$$
\boxed{T_t=\kappa\frac1{r^2}\frac\partial{\partial r}\left(r^2T_r\right),\qquad r>a(t),}
$$

with $T(r,0)=T_\infty$ for $r>a_0$, $a(0)=a_0$ and $T(r,t)\to T_\infty$ as $r\to\infty$.

The [Gibbs-Thomson effect](../../../../../gibbs-thomson-relation.md) gives [curvature-induced melting-temperature depression](../../../../../curvature-induced-melting-temperature-depression.md). For a spherical interface write

$$
\boxed{T(a(t),t)=T_s-\frac\Gamma{a(t)},\qquad
\Gamma=\frac{2\gamma T_s}{\rho\mathcal L}>0,}
$$

where $\gamma$ is solid-liquid interfacial energy per area and the factor two is the sphere's curvature $2/a$. Here $T_s$ in the thermodynamic formula is an absolute [temperature](../../../../../temperature.md). The notation $\Gamma$ also permits a given measured capillary coefficient without requiring its microscopic derivation.

In the one-phase [Stefan problem](../../../../../stefan-problem.md), the solid has no internal [heat flux](../../../../../heat-flux-density.md) and the [Stefan condition](../../../../../stefan-condition.md) is

$$
\boxed{\rho\mathcal L\dot a=-k_\ell T_r(a^+,t).}
$$

The sign follows from heat balance: positive outward liquid [heat flux](../../../../../heat-flux-density.md) releases [latent heat](../../../../../latent-heat.md) as the solid grows. If the solid's thermal storage is retained, its [temperature](../../../../../temperature.md) $T^{(s)}$ instead satisfies its own radial [heat equation](../../../../../heat-equation.md), $\partial_rT^{(s)}(0,t)=0$, and $T^{(s)}(a^-,t)=T(a^+,t)$. The two-phase condition is $\rho\mathcal L\dot a=k_sT_r^{(s)}(a^-,t)-k_\ell T_r(a^+,t)$. It reduces to the one-phase condition in the quasistatic limit because a regular harmonic [temperature](../../../../../temperature.md) inside a sphere is spatially constant. An initial solid [temperature](../../../../../temperature.md) profile is additional data for a fully time-dependent two-phase problem.

Two reciprocal [Stefan number](../../../../../stefan-number.md) conventions are common. The large parameter appropriate to the requested slow-interface limit is the [latent-to-sensible heat ratio](../../../../../latent-to-sensible-heat-ratio.md)

$$
\boxed{S=\frac{\mathcal L}{c_p\Delta T}.}
$$

It measures the energy required for phase change relative to cooling or heating by the supercooling. The often-used sensible-to-latent definition is $\mathrm{Ste}=c_p\Delta T/\mathcal L=1/S$. Thus “large Stefan number” here means large $S$, not large $\mathrm{Ste}$ in that other convention.

The thermal diffusion time for scale $a_0$ is $a_0^2/\kappa$, whereas the interface time is $Sa_0^2/\kappa$. More explicitly, with $R=r/a_0$, $\theta=(T-T_\infty)/\Delta T$ and slow time $\tau=\kappa t/(Sa_0^2)$, the liquid equation is

$$
S^{-1}\theta_\tau=\frac1{R^2}(R^2\theta_R)_R.
$$

For $S\gg1$, [temperature](../../../../../temperature.md) therefore equilibrates before the radius changes appreciably. The [quasistatic spherical Stefan problem with capillarity](../../../../../quasistatic-spherical-stefan-problem-with-capillarity.md) has a harmonic exterior [temperature](../../../../../temperature.md), fixed by its interface and far-field values:

$$
\boxed{T(r,t)=T_\infty+\frac{\Delta T\,a(t)-\Gamma}{r}.}
$$

The small initial diffusion adjustment is omitted at this order. Inserting $T_r(a)=-\Delta T/a+\Gamma/a^2$ into the [Stefan condition](../../../../../stefan-condition.md) gives

$$
\boxed{\dot a=\frac\kappa S\frac{a-a_c}{a^2},\qquad
 a_c=\frac\Gamma{\Delta T}=\frac{2\gamma T_s}{\rho\mathcal L(T_s-T_\infty)}.}
$$

This is the [critical radius for a supercooled spherical seed](../../../../../critical-radius-for-a-supercooled-spherical-seed.md). For $a_0>a_c$, the interface is warmer than the liquid and loses heat, driving growth. For $0<a_0<a_c$, its curvature-depressed interface [temperature](../../../../../temperature.md) is colder than the liquid, so heat enters and the solid melts. At $a=a_c$, the uniform [temperature](../../../../../temperature.md) $T_\infty$ supplies an equilibrium radius. It is unstable, since the radius-velocity derivative there is $\kappa/(Sa_c^2)>0$. For a growing particle with $a\gg a_c$, $a^2$ increases asymptotically as $2\kappa t/S$.

For a subcritical particle the radius decreases monotonically and remains below $a_0$. Hence

$$
\frac d{dt}a^3=-\frac{3\kappa}S(a_c-a)
\leq-\frac{3\kappa}S(a_c-a_0)<0.
$$

It cannot remain positive beyond $Sa_0^3/[3\kappa(a_c-a_0)]$, proving [finite-time extinction of a subcritical spherical seed](../../../../../finite-time-extinction-of-a-subcritical-spherical-seed.md). The exact extinction time in the reduced model is obtained by separating variables:

$$
t_e=\frac S\kappa\int_0^{a_0}\frac{a^2}{a_c-a}\,da.
$$

With $\eta_0=a_0/a_c\in(0,1)$, this is

$$
\boxed{t_e=\frac{Sa_c^2}\kappa\left[-\log(1-\eta_0)-\eta_0-\frac12\eta_0^2\right]<\infty.}
$$

Near disappearance, the capillary term dominates and $\dot a\sim-\kappa a_c/(Sa^2)$, so $\boxed{a^3\sim3\kappa a_c(t_e-t)/S}$. For $a_0\ll a_c$, the lifetime is $t_e\sim Sa_0^3/(3\kappa a_c)$; it diverges logarithmically as $a_0\to a_c^-$, consistently with the unstable equilibrium. The threshold and lifetime above are conclusions of the specified large-$S$ quasistatic continuum model, rather than an assertion that its approximation is uniform through every finite-$S$ shrinking-interface transient.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
