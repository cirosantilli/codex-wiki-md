<h1 id="section-b/b5/solution">Solution</h1>

↑ **Parent:** [B5](../b5.md)

**Solvent quality.** The [Flory interaction parameter](../../../../flory-interaction-parameter.md) $\chi$ measures the free-energy cost of polymer–solvent contacts relative to like contacts. In the simplest lattice model,

$$
\chi=\frac{z_c}{k_BT}\left[\epsilon_{ps}-\frac{\epsilon_{pp}+\epsilon_{ss}}2\right],
$$

where $z_c$ is the coordination number and the $\epsilon$ values are contact energies. For lattice-site volume $v_0$, the effective two-segment [excluded volume](../../../../excluded-volume.md) is $v_{\mathrm{eff}}=v_0(1-2\chi)$. Its sign determines the leading tendency of a long dilute flexible chain.

For $\chi<1/2$, $v_{\mathrm{eff}}>0$: a [good solvent](../../../../good-solvent.md) favors a swollen coil because segment encounters are effectively repulsive. For $\chi=1/2$, the leading attraction and repulsion cancel, giving approximately [ideal chain](../../../../ideal-chain.md) statistics. For $\chi>1/2$, effective attraction favors contraction in a [poor solvent](../../../../poor-solvent.md), eventually producing a compact [polymer globule](../../../../polymer-globule.md) under sufficiently poor conditions. This does not mean that every finite-chain solution with $\chi>1/2$ is automatically phase-separated; that also depends on composition and chain length.

The condition $\chi=1/2$ is the [theta temperature](../../../../theta-temperature.md) condition for that polymer–solvent pair. For an energetic model $\chi=A/T$, it occurs at $T=\Theta=2A$. More generally, if $\chi=A/T+B$, it occurs when $A/\Theta+B=1/2$. It is not the absence of all intermolecular interactions and does not require the polymer and solvent to be chemically identical.

**Chain dimensions.** Interpret $R$ as the root-mean-square [end-to-end distance of a polymer chain](../../../../end-to-end-distance-of-a-polymer-chain.md). Let $a$ denote the supplied statistical step length, calibrated to the same count $N$ as the [degree of polymerization](../../../../degree-of-polymerization.md). At the theta condition, random-walk statistics give

$$
\boxed{R_\theta=aN^{1/2}}.
$$

For a [good solvent](../../../../good-solvent.md), the [Flory approximation](../../../../flory-approximation.md) balances entropic stretching and two-segment interaction:

$$
\frac{F(R)}{k_BT}\sim\frac{R^2}{Na^2}+\frac{v_{\mathrm{eff}}N^2}{R^3}.
$$

Minimization gives $R^5\sim v_{\mathrm{eff}}a^2N^3$, hence

$$
\boxed{R_{\mathrm{good}}\sim a\left(\frac{v_{\mathrm{eff}}}{a^3}\right)^{1/5}N^{3/5}}.
$$

Thus the familiar good-solvent scaling is $R\sim aN^{3/5}$ when its nonuniversal solvent-quality amplitude is suppressed. With the additional lattice estimate $v_0\simeq a^3$, the more explicit form is $R\sim a(1-2\chi)^{1/5}N^{3/5}$. This swollen-coil estimate is used away from the narrow theta crossover; it must not be extrapolated to predict $R=0$ as $\chi\uparrow1/2$. The crossover occurs when $(1-2\chi)N^{1/2}$ is of order one. Nearer theta, the ideal-coil size supplies the appropriate limit.

**Numerical sizes.** The theta value is

$$
\boxed{R_\theta=(0.67\,\mathrm{nm})\sqrt{1500}=25.9\,\mathrm{nm}}.
$$

For $\chi=0.3$, the plain good-solvent scaling gives

$$
\boxed{R_{\mathrm{good}}\sim(0.67\,\mathrm{nm})(1500)^{3/5}=53.9\,\mathrm{nm}}.
$$

If the solvent-quality amplitude is retained with $v_0=a^3$, it instead gives

$$
\boxed{R_{\chi=0.3}\sim(0.67\,\mathrm{nm})(0.4)^{1/5}(1500)^{3/5}=44.9\,\mathrm{nm}}.
$$

The distinction is an explicitly stated modeling convention: the question does not give a microscopic site volume or an absolute swollen-coil prefactor. Both estimates describe a coil larger than the theta coil. Here $(1-2\chi)\sqrt N\simeq15.5$, so a swollen-coil estimate is reasonable. Neither result is an exact microscopic prediction from the supplied data alone.

**Overlap concentration.** The [polymer overlap concentration](../../../../polymer-overlap-concentration.md) corresponds to one chain per coil volume. Using the scaling convention $V_{\mathrm{coil}}\sim R_\theta^3$ gives

$$
n_p^*\sim R_\theta^{-3}=5.72\times10^{22}\,\mathrm{m^{-3}},\qquad
n_m^*\sim\frac{N}{R_\theta^3}=8.58\times10^{25}\,\mathrm{m^{-3}}.
$$

The first is chain [number density](../../../../number-density.md); the second counts [repeat units](../../../../repeat-unit.md). Thus the repeat-unit [molar concentration](../../../../molar-concentration.md) is approximately $0.143\,\mathrm{mol\,L^{-1}}$. If the lattice-site volume is taken as $v_0=a^3$, this is equivalently

$$
\boxed{\phi^*\sim\frac{Nv_0}{R_\theta^3}\simeq N^{-1/2}=2.58\times10^{-2}}.
$$

For a mass-concentration estimate, a [polystyrene](../../../../polystyrene.md) repeat unit $\mathrm{C_8H_8}$ has [molar mass](../../../../molar-mass.md) about $104.15\,\mathrm{g\,mol^{-1}}$, so this scaling convention gives

$$
\boxed{c^*\sim14.8\,\mathrm{g\,L^{-1}}}.
$$

There is no sharp coil surface fixing an exact numerical prefactor. For example, using the often adopted geometric definition $V_{\mathrm{coil}}=4\pi R_g^3/3$, with the [ideal chain](../../../../ideal-chain.md) [radius of gyration](../../../../radius-of-gyration.md) $R_g=R_\theta/\sqrt6=10.6\,\mathrm{nm}$, gives $c^*\simeq52\,\mathrm{g\,L^{-1}}$. The invariant content is one chain per coil volume and the theta scaling $\phi^*\propto N^{-1/2}$; the radius and coil-volume convention must accompany a numerical value.

**Osmotic pressure.** In the given lattice expression, $\phi$ is a dimensionless polymer [volume fraction](../../../../volume-fraction.md), not a dimensional [number density](../../../../number-density.md), and $f$ is the mixing [free energy](../../../../thermodynamic-free-energy.md) per lattice site. Introduce $v_0$ to obtain a physical [osmotic pressure](../../../../osmotic-pressure.md). If $M=N_s+NN_p$ is the number of sites and $\phi=NN_p/M$, differentiation of $F_{\mathrm{mix}}=Mf(\phi)$ with respect to the solvent count at fixed chain count gives

$$
\Delta\mu_s=f-\phi f'.
$$

Balancing this change in solvent [chemical potential](../../../../chemical-potential-split.md) against the pressure contribution $v_0\Pi$ gives $\Pi=(\phi f'-f)/v_0$. For composition-independent $\chi$,

$$
\frac{f'}{k_BT}=\frac{\ln\phi+1}{N}-\ln(1-\phi)-1+\chi(1-2\phi),
$$

and therefore the [osmotic pressure in Flory-Huggins solution theory](../../../../osmotic-pressure-in-flory-huggins-solution-theory.md) is

$$
\boxed{\Pi=\frac{k_BT}{v_0}\left[\frac\phi N-\ln(1-\phi)-\phi-\chi\phi^2\right]}.
$$

Expanding the [logarithm](../../../../logarithm.md) as $\phi\to0$ gives

$$
\boxed{\Pi=\frac{k_BT}{v_0}\left[\frac\phi N+\left(\frac12-\chi\right)\phi^2+\frac{\phi^3}{3}+O(\phi^4)\right]}.
$$

The first term is $n_pk_BT$ with $n_p=\phi/(Nv_0)$ now denoting chain [number density](../../../../number-density.md): a whole chain supplies one translational contribution. The sign of the quadratic correction reproduces the solvent-quality classification. It is positive for a [good solvent](../../../../good-solvent.md), zero at the [theta temperature](../../../../theta-temperature.md), and negative for a [poor solvent](../../../../poor-solvent.md). This is the same two-segment interaction that swells or contracts a single coil. At theta, a positive third-order contribution remains; the chain is approximately ideal in its large-scale conformation, not a gas of segments with no interactions at all.

## ↑ Ancestors (13)

1. [B5](../b5.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
