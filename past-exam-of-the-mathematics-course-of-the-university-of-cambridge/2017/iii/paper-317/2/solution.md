<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a quasistatic spherical [star](../../../../../star.md) with fixed total mass, the [stellar structure equations](../../../../../stellar-structure-equations.md) in radius are

$$
\boxed{\frac{dM_r}{dr}=4\pi r^2\rho,\qquad\frac{dP}{dr}=-\frac{GM_r\rho}{r^2},\qquad\frac{dL_r}{dr}=4\pi r^2\rho\left(\varepsilon_{\rm nuc}-\varepsilon_\nu-T\frac{Ds}{Dt}\right),\qquad\frac{dT}{dr}=\frac TP\nabla\frac{dP}{dr}.}
$$

Here $s$ is the [specific entropy](../../../../../specific-entropy.md) of a moving mass shell, and the [entropy](../../../../../entropy.md) term accounts for release or storage of thermal and gravitational [energy](../../../../../energy.md). In thermal equilibrium it vanishes. An [equation of state](../../../../../equation-of-state.md), [opacity](../../../../../opacity.md), energy-generation law and composition evolution close the equations. The absence of mass loss fixes the outer mass coordinate; it does not require the [star](../../../../../star.md) to be in thermal equilibrium.

The [radiative temperature gradient](../../../../../radiative-temperature-gradient.md) needed to carry the full [luminosity](../../../../../luminosity.md) is

$$
\nabla_{\rm rad}=\frac{3\kappa L_rP}{16\pi a_{\rm rad}cGM_rT^4}.
$$

Here the actual [temperature gradient](../../../../../temperature-gradient.md) is $\nabla=d\log T/d\log P$. For uniform composition the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) says that a radiative layer is stable if $\nabla_{\rm rad}<\nabla_{\rm ad}$, with marginal stability at equality, where the [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md) is $(\partial\log T/\partial\log P)_s$. Use $\nabla=\nabla_{\rm rad}$ there. If $\nabla_{\rm rad}>\nabla_{\rm ad}$, [convection](../../../../../convection.md) carries some of the flux. Efficient [convection](../../../../../convection.md) gives $\nabla\simeq\nabla_{\rm ad}$; inefficient surface [convection](../../../../../convection.md) needs a transport prescription and can be superadiabatic. For composition gradients, use the [Ledoux criterion](../../../../../ledoux-criterion.md), with threshold $\nabla_{\rm ad}+\phi\nabla_{\mu_{\rm mol}}/\delta_{\rm th}$ instead. Here $\nabla_{\mu_{\rm mol}}=d\log\mu_{\rm mol}/d\log P$, $\phi=(\partial\log\rho/\partial\log\mu_{\rm mol})_{P,T}$ and $\delta_{\rm th}=-(\partial\log\rho/\partial\log T)_{P,\mu_{\rm mol}}$, using the [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu_{\rm mol}$.

Above the thin burning shell, take constant [luminosity](../../../../../luminosity.md) $L$, constant [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu_{\rm mol}$, ideal-gas [pressure](../../../../../pressure.md) $P=\mathcal RT\rho$ with $\mathcal R=k_B/(\mu_{\rm mol}m_u)$, and the [Kramers' opacity law](../../../../../kramers-opacity-law.md) $\kappa=\kappa_0\rho T^{-7/2}$. Then the [temperature](../../../../../temperature.md) equation is

$$
\frac{dT}{dr}=-\frac{3\kappa_0L}{16\pi a_{\rm rad}c}\frac{\rho^2}{r^2T^{13/2}}.
$$

To implement the printed assumption that $P,\rho$ and $M_r$ are all [power laws](../../../../../power-law.md) while retaining mass conservation, write $M_r\propto r^m$, $\rho\propto r^b$, $P\propto r^p$ and $T\propto r^d$. The mass equation gives $m=b+3$; the [ideal gas](../../../../../ideal-gas.md) law gives $d=p-b$; [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) gives $d=m-1$. The diffusion equation gives $d-1=2b-2-13d/2$. Solving this linear system gives the [self-gravitating Kramers power-law envelope](../../../../../self-gravitating-kramers-power-law-envelope.md):

$$
\boxed{M_r\propto r^{1/11},\qquad\rho\propto r^{-32/11},\qquad P\propto r^{-42/11},\qquad T\propto r^{-10/11}.}
$$

The coefficients can also be matched consistently. If $r_c$ is the core boundary and $M_c$ its [enclosed mass](../../../../../enclosed-mass.md),

$$
M_r=M_c\left(\frac r{r_c}\right)^{1/11},\qquad\rho(r)=\frac{M_r}{44\pi r^3},\qquad T(r)=\frac{11}{42}\frac{GM_r}{\mathcal Rr},\qquad P=\mathcal R\rho T.
$$

[Radiative transfer](../../../../../radiative-transfer.md) fixes the constant [luminosity](../../../../../luminosity.md) through

$$
L=\frac{160\pi a_{\rm rad}c}{33\kappa_0}\frac{rT^{15/2}}{\rho^2},
$$

whose right-hand side is independent of radius for these exponents. Thus this is a solution of all four envelope equations, not just a dimensional estimate.

Matching the boundary [temperature](../../../../../temperature.md) to the isothermal core and extrapolating the idealized [power law](../../../../../power-law.md) to the specified [photosphere](../../../../../photosphere.md) gives

$$
\boxed{\frac R{r_c}=\left(\frac{10^7}{4000}\right)^{11/10}=2500^{11/10}\simeq5.47\times10^3.}
$$

For reference $M_R/M_c=(R/r_c)^{1/11}=2500^{1/10}\simeq2.19$, so the envelope mass is not negligible in this particular solution. The given $M_c\simeq M_\odot$ fixes the core-radius normalization $r_c=(11/42)GM_c/(\mathcal R10^7\,\mathrm K)$; a numerical absolute radius needs the unspecified molecular weight. The exponent ratio also gives $\nabla=d/p=5/21<2/5$, so the fully ionized monatomic version of this idealization is convectively stable.

A different common approximation neglects the envelope's self-gravity and sets $M_r\simeq M_c$ in the force equation. It cannot obey the exact mass equation with a nonzero density and exactly constant $M_r$. Under that additional approximation, the same calculation instead gives

$$
T\propto r^{-1},\quad\rho\propto r^{-13/4},\quad P\propto r^{-17/4},\qquad\boxed{R/r_c\simeq2500.}
$$

This is the constant-core-mass [power-law opacity radiative envelope](../../../../../power-law-opacity-radiative-envelope.md) limit, not the full power-law solution with changing [enclosed mass](../../../../../enclosed-mass.md). Stating which approximation is used resolves the otherwise different numerical radius ratios.

A compact nearly isothermal core, a thin luminosity-producing shell and a much larger cool envelope describe a shell-burning [red giant](../../../../../red-giant.md). The full power-law profile is a deliberately simple model. The [Kramers' opacity law](../../../../../kramers-opacity-law.md) and an ionized [ideal gas](../../../../../ideal-gas.md) are not reliable at a $4000\,\mathrm K$ [photosphere](../../../../../photosphere.md); partial ionization, other [opacity](../../../../../opacity.md) sources and a [convective envelope](../../../../../convective-envelope.md) usually modify real cool giants. The quoted radius ratios are extrapolations within the stipulated model.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
