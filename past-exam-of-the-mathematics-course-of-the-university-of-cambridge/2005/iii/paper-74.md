# Paper 74

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper74.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper74.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
    - [a](#4/iii/a)
      - [Solution](#4/iii/a/solution)
    - [b](#4/iii/b)
      - [Solution](#4/iii/b/solution)
    - [c](#4/iii/c)
      - [Solution](#4/iii/c/solution)

## 1

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

On the sphere, both [cosmic time](../../../cosmology.md#cosmic-time) and the [comoving coordinate](../../../cosmology.md#comoving-coordinate) $r$ are constant. The positive spatial [induced metric](../../../riemannian-geometry.md#induced-metric) obtained from the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) is therefore $d\ell^2=a^2r^2(d\theta^2+\sin^2\theta\,d\phi^2)$. Its [area element](../../../differential-geometry.md#area-element-of-a-surface) is the square root of its determinant:

$$
dA=a^2r^2\sin\theta\,d\theta\,d\phi.
$$

Integrating over the [spherical coordinates](../../../calculus.md#spherical-coordinate-system) gives

$$
\boxed{A=\int_0^{2\pi}\int_0^\pi a^2r^2\sin\theta\,d\theta\,d\phi=4\pi[a(t)r]^2.}
$$

Thus $ar$ is the [areal radius](../../../general-relativity.md#areal-radius). In a curved spatial slice it need not equal the proper radial distance $a\int_0^r(1-kr'^2)^{-1/2}dr'$; the angular part of the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), rather than a Euclidean radial-distance assumption, establishes the [surface area](../../../differential-geometry.md#surface-area).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For a radial [null geodesic](../../../special-relativity.md#null-geodesic), the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) gives

$$
\int_{t_e}^{t_0}\frac{c\,dt}{a(t)}=\int_{r_e}^{r_0}\frac{|dr|}{\sqrt{1-kr^2}}.
$$

Two successive wave crests traverse the same comoving path between [comoving observers](../../../cosmology.md#comoving-observer). Subtracting their path integrals, to first order in their short emission and reception periods, gives $\delta t_0/a(t_0)=\delta t_e/a(t_e)$. Since [cosmic time](../../../cosmology.md#cosmic-time) is each observer's proper time and the [frequency](../../../physics.md#frequency) is the reciprocal period,

$$
\boxed{1+z=\frac{\nu_e}{\nu_0}=\frac{a(t_0)}{a(t_e)}.}
$$

This neglects [peculiar velocities](../../../cosmology.md#peculiar-velocity) and local [gravitational redshift](../../../general-relativity.md#gravitational-redshift) contributions.

For B's light passing through A on its way to Earth, with the comparison event at A being that passage, [cosmological redshift](../../../cosmology.md#cosmological-redshift) factors multiply:

$$
1+z_B=(1+z_{BA})(1+z_A),\qquad
\boxed{z_{BA}=\frac{4}{2}-1=1.}
$$

This is the intended numerical answer with that reception-event specification. The [reception-event dependence of intergalactic redshift](../../../cosmology.md#reception-event-dependence-of-intergalactic-redshift) is essential: Earth's two redshifts by themselves neither specify the A–B separation nor identify the emission event at B whose light A receives at a chosen time. For arbitrary directions or a different reception time at A, the general answer is $a(t_{A,\rm rec})/a(t_{B,\rm em})-1$, with the emission time fixed by the A–B [null geodesic](../../../special-relativity.md#null-geodesic); it cannot be deduced from the two supplied numbers alone.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Introduce the radial [comoving distance](../../../cosmology.md#comoving-radial-distance) $\chi=\int dr/\sqrt{1-kr^2}$. A [photon](../../../quantum-mechanics.md#photon) travels $d\chi=c\,dt/a$, so a finite [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) since a big-bang origin at $t=0$ requires

$$
\chi_{\rm hor}(t)=c\int_0^t\frac{dt'}{a(t')}<\infty.
$$

To relate this geometric criterion to a [mass density](../../../fluid-mechanics.md#density), use the [Friedmann equation](../../../cosmology.md#friedmann-equations) as well as the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric). For an early epoch dominated by $\rho=\rho_*a^{-\alpha}$, with negligible curvature and cosmological constant in the leading balance,

$$
H^2\simeq\frac{8\pi G\rho_*}{3}a^{-\alpha},\qquad
\dot a\propto a^{1-\alpha/2},\qquad a\propto t^{2/\alpha}.
$$

Equivalently $dt/a=da/(a^2H)\propto a^{\alpha/2-2}da$. Its integral at $a=0$ converges precisely when $\alpha/2-2>-1$, hence

$$
\boxed{\alpha>2.}
$$

At $\alpha=2$ the divergence is logarithmic, and at $0<\alpha<2$ it is a power divergence. If spatial curvature dominates a bang instead, $a\propto t$ and the integral again diverges; $\alpha>2$ also ensures that this curvature term, which scales as $a^{-2}$, is subdominant near the bang. This argument assumes the ordinary expanding big-bang branch of the [Friedmann equation](../../../cosmology.md#friedmann-equations); a metric alone imposes no density law, and a universe with a different past boundary needs its own lower integration limit.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), [conservation of energy](../../../physics.md#conservation-of-energy) gives $\rho\propto a^{-4}$: dilution contributes $a^{-3}$ and the [cosmological redshift](../../../cosmology.md#cosmological-redshift) of each [photon](../../../quantum-mechanics.md#photon) contributes another $a^{-1}$. Thus $\alpha=4>2$ and $a=A\sqrt t$ in the flat radiation-dominated approximation. The [particle horizon](../../../cosmology.md#particle-horizon) measured as proper radial distance on a constant-time slice is

$$
\boxed{s_{\rm hor}(t)=a(t)c\int_0^t\frac{dt'}{a(t')}=A\sqrt t\frac{2c\sqrt t}{A}=2ct.}
$$

Every local [comoving observer](../../../cosmology.md#comoving-observer) measures the [speed of light](../../../special-relativity.md#speed-of-light) to be $c$. However, the spatial separations traversed earlier have expanded by the time the final distance is measured; the present separation from the earliest accessible comoving worldline is not the integral of local path lengths measured at their different traversal times. Indeed $\dot s_{\rm hor}=Hs_{\rm hor}+c=2c$ in this era, explicitly separating [cosmic expansion](../../../cosmology.md#expansion-of-the-universe) from local propagation. Curvature or a later transition to [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) changes the exact formula; $2ct$ is the radiation-dominated result.

## 2

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) is the large collection of narrow [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption) features in the spectrum of a distant [quasar](../../../astrophysics.md#quasar). Neutral [hydrogen](../../../chemistry.md#hydrogen) in foreground gas absorbs at its own redshifted $1s\to2p$ resonance, so an absorber at $z_{\rm abs}$ places its feature at

$$
\lambda_{\rm obs}=1215.67\,(1+z_{\rm abs})\,\text{Å}.
$$

Ordinary intervening absorbers have $z_{\rm abs}<z_Q$, putting their [Lyman-alpha lines](../../../physics.md#lyman-alpha-line) blueward of the quasar's own broad [Lyman-alpha emission](../../../physics.md#lyman-alpha-emission). Many different absorbing patches along the same [line of sight](../../../astrophysics.md#line-of-sight) make the forest; they are not different transitions of one cloud. At sufficiently short wavelengths higher Lyman-series transitions can overlap the forest, so an actual analysis identifies these blends rather than treating every dip as isolated Ly-alpha.

<a id="2/a/image-schematic-quasar-lyman-alpha-forest-and-neutral-hydrogen-column-density-distribution-at-redshift-three"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-74-forest.png)

**[Figure 1](#2/a/image-schematic-quasar-lyman-alpha-forest-and-neutral-hydrogen-column-density-distribution-at-redshift-three). Schematic quasar Lyman-alpha forest and neutral-hydrogen column-density distribution at redshift three**.

The upper panel is an original schematic spectrum for $z_Q=3$, with absorption features at smaller [cosmological redshifts](../../../cosmology.md#cosmological-redshift) and a broad emission feature near $4863$ Å. The lower panel anticipates the column-density discussion: both curves are teaching sketches, not measured spectra or fitted survey distributions. The ordinary [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) mainly traces the fluctuating, photoionized [intergalactic medium](../../../astrophysics.md#intergalactic-medium), rather than a collection of identical isolated, neutral clouds.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[Hydrogen](../../../chemistry.md#hydrogen) is the most abundant element, and its [Lyman-alpha line](../../../physics.md#lyman-alpha-line) is a strong resonance from the ground state. Very small neutral fractions in an otherwise ionized [intergalactic medium](../../../astrophysics.md#intergalactic-medium) therefore produce detectable [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption). A long [quasar](../../../astrophysics.md#quasar) sightline samples a great many modest density enhancements in the cosmic gas, with a much larger covering area than the compact high-column regions that produce [damped Lyman-alpha systems](../../../physics.md#damped-lyman-alpha-system).

Heavy-element absorption additionally requires metal enrichment and enough ions in the relevant ionization state. Many weak [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) absorbers contain too few such ions to produce detectable metal lines at the same sensitivity, while high-column [Lyman limit systems](../../../physics.md#lyman-limit-system) and [damped Lyman-alpha systems](../../../physics.md#damped-lyman-alpha-system) are intrinsically rarer. Thus **abundant hydrogen, a sensitive resonance and the large interception area of diffuse gas together explain the forest's numerical dominance**. The comparison is between absorber classes at specified observational sensitivity; it does not mean that a metal-rich system has only one spectral transition.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Typical weak [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) absorbers have neutral [hydrogen](../../../chemistry.md#hydrogen) [column densities](../../../statistical-physics.md#column-density) roughly $10^{12}$–$10^{16}\,\mathrm{cm}^{-2}$, with stronger forest absorption extending towards $10^{17}\,\mathrm{cm}^{-2}$. Common [Doppler broadening](../../../statistical-physics.md#doppler-broadening) parameters are a few tens of $\mathrm{km\,s}^{-1}$, consistent with gas at approximately $10^4$ K together with bulk velocity gradients. The thermal contribution is

$$
b_{\rm th}=\sqrt{\frac{2k_BT}{m_H}}=12.9\left(\frac{T}{10^4\,\mathrm K}\right)^{1/2}\mathrm{km\,s}^{-1}.
$$

A line width is consequently a temperature upper bound if all other broadening is neglected, not a unique thermometer. The gas commonly lies in diffuse sheets and filaments at modest [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast); only the strongest systems need substantial self-shielding or a galactic environment.

For optically thin gas illuminated by the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background), [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium) requires

$$
n_{\rm HI}\Gamma_{\rm HI}=n_en_p\alpha(T),\qquad
x_{\rm HI}\equiv\frac{n_{\rm HI}}{n_H}\simeq\frac{\alpha(T)n_H}{\Gamma_{\rm HI}},
$$

where the last approximation uses almost complete hydrogen ionization. For example, $n_H=10^{-5}\,\mathrm{cm}^{-3}$, $\alpha\simeq4\times10^{-13}\,\mathrm{cm}^3\mathrm s^{-1}$ and $\Gamma_{\rm HI}=10^{-12}\,\mathrm s^{-1}$ give $x_{\rm HI}\simeq4\times10^{-6}$. A $100$ kpc path then has $N_{\rm HI}\sim10^{13}\,\mathrm{cm}^{-2}$ despite its tiny neutral fraction. This illustrates the [Lyman-alpha forest photoionization scaling](../../../astrophysics.md#lyman-alpha-forest-photoionization-scaling): low density makes the two-body [radiative recombination](../../../physics.md#radiative-recombination) rate weak relative to the one-body [photoionization](../../../physics.md#photoionization) rate, but a long path and a strong resonance still produce measurable absorption.

Independent information is important because a [column density](../../../statistical-physics.md#column-density) alone is not a volume density. Similar absorption in close pairs of [quasars](../../../astrophysics.md#quasar) indicates substantial transverse coherence, while an ionizing [optical depth](../../../astrophysics.md#optical-depth) $N_{\rm HI}\sigma_{912}\ll1$ shows that these weak systems do not shield themselves from the background. The continuum-shielding threshold is $1/\sigma_{912}\simeq1.6\times10^{17}\,\mathrm{cm}^{-2}$. Together with the observed line widths and ionization balance, these facts favor **extended, low-density, highly ionized gas** over small cold neutral clouds. The physical interpretation and characteristic scales are consistent with [Rauch's forest analysis](https://arxiv.org/abs/astro-ph/9806286) and [the measured column and line-width distributions](https://arxiv.org/abs/astro-ph/9507047).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Specify the path convention before integrating the [neutral-hydrogen column-density distribution](../../../physics.md#neutral-hydrogen-column-density-distribution). Write $f_z=\partial^2\mathcal N/(\partial N\partial z)$ and $f_X=\partial^2\mathcal N/(\partial N\partial X)$, with [absorption distance](../../../physics.md#absorption-distance) satisfying

$$
\frac{dX}{dz}=\frac{H_0}{H(z)}(1+z)^2,\qquad f_z=f_X\frac{dX}{dz}.
$$

The lower panel of the preceding sketch shows the approximate decrease of $f$ with $N=N_{\rm HI}$ near $z=3$. Ordinary forest columns are roughly described by $f\propto N^{-\beta}$, $\beta\sim1.5$, but the slope changes through partially shielded [Lyman limit systems](../../../physics.md#lyman-limit-system) and high-column [damped Lyman-alpha systems](../../../physics.md#damped-lyman-alpha-system). No single slope should be extrapolated through all these regimes. In logarithmic bins the number is $N\ln(10)f$, whereas their neutral mass contribution is proportional to $N^2f$; confusing these two weightings would give a wrong baryon inventory.

To derive the [neutral gas density from an absorption distribution](../../../physics.md#neutral-gas-density-from-an-absorption-distribution), a redshift interval $dz$ has proper light-path length $d\ell=c\,dz/[(1+z)H]$. The sum of neutral [hydrogen](../../../chemistry.md#hydrogen) columns per path length estimates the mean proper number density:

$$
\overline n_{\rm HI}(z)=\frac{(1+z)H(z)}c\int Nf_z(N,z)\,dN.
$$

The proper [mass density](../../../fluid-mechanics.md#density) is $m_H\overline n_{\rm HI}$; division by $(1+z)^3$ converts it to a comoving mass density. Thus, with today's [critical density](../../../cosmology.md#critical-density) $\rho_{\rm crit,0}=3H_0^2/(8\pi G)$,

$$
\boxed{\Omega_{\rm HI}(z)=\frac{m_HH(z)}{c\rho_{\rm crit,0}(1+z)^2}\int Nf_z\,dN
=\frac{H_0m_H}{c\rho_{\rm crit,0}}\int Nf_X\,dN.}
$$

A representative finite-sample estimator replaces the last integral by $\sum_j N_j/\Delta X$, with completeness and selection corrections. This defines a comoving inventory divided by today's [critical density](../../../cosmology.md#critical-density); a fraction of the instantaneous critical density has a different normalization. Neutral gas including accompanying helium is obtained by multiplying by a specified mass correction, approximately $1.3$; hydrogen-only $\Omega_{\rm HI}$ must not silently include it.

At $z\sim3$ the observed neutral inventory is of order $10^{-3}$, far below the [cosmological baryon density](../../../cosmology.md#cosmological-baryon-density) of order $0.04$–$0.05$ for $h\sim0.7$. High-column [damped Lyman-alpha systems](../../../physics.md#damped-lyman-alpha-system) contribute most of this neutral mass although weak forest lines dominate the counts; for $\beta=1.5$ the mass per logarithmic column interval increases as $N^{1/2}$ in the forest regime. The small neutral inventory therefore does not imply a small total gas inventory: the [intergalactic medium](../../../astrophysics.md#intergalactic-medium) contains a large ionized baryon reservoir invisible to a neutral-only count. Recovering that reservoir requires an ionization correction and a gas-density model. The survey normalization and high-column contribution are described in [the neutral-gas inventory analysis](https://ned.ipac.caltech.edu/level5/Sept05/Wolfe/Wolfe2.html).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For a fixed [column density](../../../statistical-physics.md#column-density) or rest-equivalent-width threshold, the number of ordinary [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) features per unit [redshift](../../../optics.md#redshift) generally increases towards higher redshift. Over much of $z\sim1$–$4$, a rough description is $d\mathcal N/dz\propto(1+z)^\gamma$ with an index of order $2$–$3$, dependent on selection; the evolution is much slower at low redshift. Near [reionization](../../../cosmology.md#reionization), blending and widespread opacity make a decomposition into individually detected lines increasingly inappropriate.

First separate physical evolution from geometrical path length. For comoving absorber density $n_c$ and proper interception area $\sigma_p$, [absorber incidence and comoving number density](../../../physics.md#absorber-incidence-and-comoving-number-density) gives

$$
\frac{d\mathcal N}{dz}=n_c\sigma_p\frac{c(1+z)^2}{H(z)}.
$$

Even a non-evolving population is not constant per unit redshift. Using [absorption distance](../../../physics.md#absorption-distance) removes this particular geometrical effect.

The remaining [redshift evolution of the Lyman-alpha forest](../../../astrophysics.md#redshift-evolution-of-the-lyman-alpha-forest) reflects several competing processes. [Cosmic expansion](../../../cosmology.md#expansion-of-the-universe) dilutes the gas; at fixed overdensity, [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium) gives $n_{\rm HI}\propto\alpha(T)(1+z)^6/\Gamma$, so dilution can move many features below a fixed threshold. The [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background) evolves as [quasars](../../../astrophysics.md#quasar), stellar sources and ionizing-photon absorption evolve; a decline of its intensity at late times partly offsets dilution. Photoheating changes [temperature](../../../thermodynamics.md#temperature) and [radiative recombination](../../../physics.md#radiative-recombination), while [gravitational instability](../../../astrophysical-fluid-dynamics.md#gravitational-instability) redistributes gas into denser structures and hot shocked phases and changes its velocity field. Thus evolving line counts are not a direct count of conserved clouds; the density, thermal state, radiation field, geometry and observational selection must all be accounted for. The high-redshift increase and its physical interpretation are documented in [the forest observations and models](https://arxiv.org/abs/astro-ph/9806286).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Near the background [quasar](../../../astrophysics.md#quasar), the [quasar proximity effect](../../../astrophysics.md#proximity-effect-astrophysics) typically reduces the number and strength of [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) features relative to regions farther along the sightline. It is an ionization effect, not evidence that the quasar lies in an empty region. At fixed gas density and [temperature](../../../thermodynamics.md#temperature), [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium) gives

$$
\Gamma=\Gamma_{\rm bg}+\Gamma_Q,\qquad
\omega=\frac{\Gamma_Q}{\Gamma_{\rm bg}},\qquad
\boxed{N_{\rm HI}=\frac{N_{\rm HI}^{(0)}}{1+\omega}.}
$$

If the unperturbed [neutral-hydrogen column-density distribution](../../../physics.md#neutral-hydrogen-column-density-distribution) is $AN^{-\beta}$, $\beta>1$, detecting a column above $N_{\min}$ now requires its unperturbed column to exceed $(1+\omega)N_{\min}$. Integrating that distribution shows that the number above threshold is reduced by $(1+\omega)^{1-\beta}$. This supplies an explicit model for the decline of line counts.

The known quasar luminosity estimates its [photoionization rate](../../../physics.md#photoionization-rate) at proper separation $R$:

$$
\Gamma_Q(R)=\int_{\nu_{\rm LL}}^\infty
\frac{L_\nu}{4\pi R^2h\nu}\sigma_{\rm HI}(\nu)\,d\nu,
\qquad
\Gamma_{\rm bg}=4\pi\int_{\nu_{\rm LL}}^\infty
\frac{J_\nu\sigma_{\rm HI}(\nu)}{h\nu}\,d\nu.
$$

These expressions assume unattenuated, steady, isotropic quasar emission and a specified ionizing spectrum. Fitting the measured suppression as a function of separation determines the ratio $\Gamma_Q/\Gamma_{\rm bg}$ and hence constrains the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background). A weaker background gives a larger region in which the quasar dominates. For fixed background spectral shape, this constrains its specific intensity near the [Lyman limit system](../../../physics.md#lyman-limit-system) ionization edge, not an arbitrary spectral function. The [proximity-effect estimator of the ionizing background](../../../astrophysics.md#proximity-effect-estimator-of-the-ionizing-background) is biased if the host gas is overdense, the quasar's past luminosity differs from its observed luminosity, its radiation is anisotropic, or systemic-redshift errors distort the inferred separation; absorption between source and gas also changes $\Gamma_Q$. These effects explain why the method needs environmental and source modeling, as discussed in [the proximity-effect measurements](https://ned.ipac.caltech.edu/level5/Sept01/Rauch/Rauch3_2.html).

## 3

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A superhorizon [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) is gauge dependent. The stated growth laws describe the growing [adiabatic mode](../../../linear-cosmological-perturbation-theory.md#adiabatic-mode) in the [comoving-gauge density contrast](../../../linear-cosmological-density-perturbation.md#comoving-gauge-density-contrast) (and the corresponding usual synchronous growing mode), not an arbitrary coordinate density perturbation. Work with a flat, single-fluid background with constant $w=p/\rho$, negligible [anisotropic stress](../../../general-relativity.md#anisotropic-stress), $c=1$, and a comoving Fourier wavenumber $K$.

Here is a derivation from the linear gravitational constraints and evolution equation. For an [adiabatic mode](../../../linear-cosmological-perturbation-theory.md#adiabatic-mode), the scalar gravitational potential $\Phi$ obeys

$$
\Phi''+3(1+w)\mathcal H\Phi'+wK^2\Phi+
[2\mathcal H'+(1+3w)\mathcal H^2]\Phi=0,
\qquad \mathcal H=\frac{a'}a.
$$

Primes denote [conformal time](../../../cosmology.md#conformal-time) derivatives. The [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $a\propto\tau^{2/(1+3w)}$ and $\mathcal H=2/[(1+3w)\tau]$, so the bracket vanishes. On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), $K\tau\ll1$, the leading solutions are a constant potential and a decaying solution proportional to $\tau^{-(5+3w)/(1+3w)}$. Keeping the growing adiabatic branch therefore makes $\Phi$ time independent to leading order.

Combining the time-time and time-space linear Einstein constraints eliminates the coordinate velocity and gives the comoving density constraint

$$
-K^2\Phi=4\pi Ga^2\rho\,\Delta,
\qquad
\Delta=-\frac23\left(\frac{K}{aH}\right)^2\Phi.
$$

This is the relativistic comoving constraint, not a subhorizon Newtonian approximation. Since $\rho\propto a^{-3(1+w)}$, it implies $\Delta\propto(a^2H^2)^{-1}\propto a^{1+3w}$. Also $a\propto t^{2/[3(1+w)]}$ in [cosmic time](../../../cosmology.md#cosmic-time), whence

$$
\boxed{\frac{\delta(t)}{\delta_i}=
\begin{cases}
t/t_i,&w=1/3\quad\text{(radiation domination)},\\
(t/t_i)^{2/3},&w=0\quad\text{(matter domination)}.
\end{cases}}
$$

Both epochs here mean their respective leading growing solution; matching through [matter-radiation equality](../../../cosmology.md#matter-radiation-equality) requires the full two-component evolution. The constant superhorizon curvature or potential is consistent with this growth because the comoving density perturbation carries the additional factor $(K/aH)^2$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For [statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) and [statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy), with the paper's finite-volume Fourier normalization,

$$
\xi(r)=\frac{V}{(2\pi)^3}\int d^3k\,P(k)e^{i\mathbf k\cdot\mathbf r}
=\frac{V}{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin kr}{kr}\,dk.
$$

The angular integral is $4\pi\sin(kr)/(kr)$. In particular $\xi(r)=\int\Delta^2(k)\sin(kr)/(kr)\,d\ln k$, confirming the stated [dimensionless power spectrum](../../../cosmic-inflation.md#dimensionless-cosmological-power-spectrum) normalization.

For the [scale-free matter power spectrum](../../../large-scale-structure-of-the-universe.md#scale-free-matter-power-spectrum) $P(k)=Ck^n$, set $u=kr$ to obtain

$$
\xi(r)=\frac{VC}{2\pi^2}r^{-n-3}I_n,
\qquad I_n=\int_0^\infty u^{n+1}\sin u\,du.
$$

At zero the integrand behaves as $u^{n+2}$, requiring $n>-3$; at infinity its oscillatory integral converges for $n<-1$. Thus in the ordinary convergent range $-3<n<-1$, the [scale-free density correlation transform](../../../linear-cosmological-density-perturbation.md#scale-free-density-correlation-transform) has

$$
I_n=\Gamma(n+2)\sin\frac{\pi(n+2)}2>0,
\qquad I_{-2}=\frac\pi2,
\qquad
\boxed{\gamma=n+3,\quad r_0^{\gamma}=\frac{VCI_n}{2\pi^2}.}
$$

The [gamma function](../../../complex-analysis.md#gamma-function) expression follows by introducing $e^{-\epsilon u}$, evaluating the complex Laplace integral where it converges absolutely at zero, and continuing within the convergent oscillatory range; its removable singularity at $n=-2$ is handled by the limit. Absolute convergence of the original correlation integral requires the smaller range $-3<n<-2$.

The exponent relation is a useful scaling statement beyond that interval, but a pure primordial $n\simeq1$ spectrum over all wavenumbers has no ordinary unsmoothed Fourier correlation integral. Physical transfer functions, cutoffs or smoothing must be specified, and a distributional extension need not yield a positive $r_0$ power law. Even within the convergent interval, the point variance is ultraviolet divergent without smoothing; the finite result here is at nonzero separation.

For a representative present-day ordinary galaxy sample over roughly $0.1$–$10\,h^{-1}\,\mathrm{Mpc}$, the familiar approximate fit is

$$
\boxed{r_0\simeq5\,h^{-1}\,\mathrm{Mpc},\qquad\gamma\simeq1.8,}
$$

where $H_0=100h\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$. These are empirical galaxy clustering parameters, not universal matter-spectrum constants; luminosity, color, selection and scale change the fit, as shown in [the galaxy correlation measurements](https://arxiv.org/abs/astro-ph/0408569). A formal power law of that slope corresponds to $n\simeq-1.2$ on those scales, not to the nearly scale-invariant primordial spectral index.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A useful decomposition of the linear [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum), absorbing the Fourier normalization into its amplitude, is

$$
P(k,z)=A\,k^{n_s}T^2(k)D^2(z).
$$

Here $T(k)$ is the [cold-dark-matter transfer function](../../../linear-cosmological-perturbation-theory.md#cold-dark-matter-transfer-function) and $D(z)$ the [linear growth factor](../../../linear-cosmological-density-perturbation.md#linear-growth-factor). On scales entering the horizon after [matter-radiation equality](../../../cosmology.md#matter-radiation-equality), $T\simeq1$, so $P\propto k^{n_s}$ with $n_s$ near one. Modes entering during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) undergo suppressed growth relative to later entrants, producing a turnover near the equality scale and, well above it, $T\propto\ln(k/k_{\rm eq})/k^2$. Thus the linear spectrum asymptotes approximately to $k^{n_s-4}\ln^2(k/k_{\rm eq})$. [Baryon acoustic oscillations](../../../cosmology.md#baryon-acoustic-oscillation) superpose a weak oscillatory pattern. At sufficiently short scales nonlinear [gravitational instability](../../../astrophysical-fluid-dynamics.md#gravitational-instability) invalidates this linear extrapolation.

<a id="3/iii/image-schematic-matter-power-spectrum-with-equality-turnover-baryon-oscillations-and-approximate-observational-scale-ranges"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-74-power-spectrum.png)

**[Figure 2](#3/iii/image-schematic-matter-power-spectrum-with-equality-turnover-baryon-oscillations-and-approximate-observational-scale-ranges). Schematic matter power spectrum with equality turnover, baryon oscillations and approximate observational scale ranges**.

The plotted curve illustrates the shape rather than a precision cosmological fit; the bands are overlapping approximate scale sensitivities, not sharp experiment boundaries. [Cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) anisotropies constrain primordial amplitudes and transfer physics on very large through acoustic scales; converting them to a late-time matter spectrum requires a cosmological model. Galaxy redshift surveys constrain approximately $k\sim0.01$–$0.2\,h\,\mathrm{Mpc}^{-1}$, with [galaxy bias](../../../large-scale-structure-of-the-universe.md#galaxy-bias) and [redshift-space distortions](../../../large-scale-structure-of-the-universe.md#redshift-space-distortions) modeled. [Peculiar velocities](../../../cosmology.md#peculiar-velocity) constrain large-scale mass fluctuations; cluster abundances constrain the fluctuation normalization near cluster scales. [Weak gravitational lensing](../../../general-relativity.md#weak-gravitational-lensing) measures projected matter on intermediate and smaller scales. The [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) extends constraints to roughly $k\sim0.3$–a few $h\,\mathrm{Mpc}^{-1}$ at high redshift, requiring gas, temperature and ionizing-background modeling. These are complementary measurements of the underlying spectrum rather than interchangeable direct Fourier measurements.

The matter fraction controls the equality turnover. From $a_{\rm eq}=\Omega_{r,0}/\Omega_{m,0}$ and the [Friedmann equation](../../../cosmology.md#friedmann-equations) at equality,

$$
k_{\rm eq}=\frac{a_{\rm eq}H_{\rm eq}}c
=\frac{H_0}{c}\sqrt{\frac{2\Omega_{m,0}^2}{\Omega_{r,0}}}.
$$

The measured background radiation fixes $\Omega_{r,0}h^2$, so the physical turnover scale measures approximately $\Omega_{m,0}h^2$. In units $h\,\mathrm{Mpc}^{-1}$ its location mainly constrains $\Omega_{m,0}h$; independent knowledge of $h$ is needed to extract $\Omega_{m,0}$. Standard radiation content gives the useful estimate $k_{\rm eq}\simeq0.073\Omega_{m,0}h^2\,\mathrm{Mpc}^{-1}$, approximately $0.015\,h\,\mathrm{Mpc}^{-1}$ for $\Omega_{m,0}=0.3$, $h=0.7$.

The [cosmological baryon density](../../../cosmology.md#cosmological-baryon-density) sets the inertia of the pre-decoupling photon–baryon fluid and changes its sound horizon and the oscillation pattern. The oscillation contrast and broadband suppression depend on the baryon fraction $\Omega_{b,0}/\Omega_{m,0}$; the acoustic positions depend on the sound horizon and the distance conversion. The [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) peak-height pattern independently constrains $\Omega_{b,0}h^2$. Combining these with the equality scale and a distance or [Hubble constant](../../../cosmology.md#hubble-constant) determination permits estimates of both requested density fractions. Spectral tilt, [neutrino free streaming](../../../linear-cosmological-density-perturbation.md#neutrino-free-streaming), galaxy bias and nonlinear evolution must be fitted rather than assigning every shape change to baryons. The acoustic signature was already observed in [the 2005 galaxy correlation measurement](https://arxiv.org/abs/astro-ph/0501171); [the first-year microwave-background parameter analysis](https://arxiv.org/abs/astro-ph/0302209) demonstrates the complementary parameter constraints.

## 4

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

In the hydrogen–helium approximation, take helium to be [helium-4](../../../chemistry.md#helium-4), and assume essentially all neutrons remaining at the onset of efficient nuclear burning enter it. Each [helium-4](../../../chemistry.md#helium-4) nucleus contains two [neutrons](../../../physics.md#neutron) and two [protons](../../../physics.md#proton), hence

$$
n_{\rm He}=\frac{n_n}{2},\qquad n_H=n_p-n_n,\qquad n_B=n_p+n_n.
$$

Here $n_p,n_n$ count constituent nucleons, not just free particles after burning. Neglecting the small nucleon mass difference and nuclear binding-energy correction, the helium mass is $4m_un_{\rm He}$ and the total baryon mass is $m_un_B$. Thus [neutron-limited helium synthesis](../../../cosmology.md#neutron-limited-helium-synthesis) gives

$$
\boxed{Y_p=\frac{4n_{\rm He}}{n_B}=\frac{2n_n}{n_p+n_n}=2\left(1+\frac{n_p}{n_n}\right)^{-1}.}
$$

For $n_n/n_p\simeq1/7$, this yields $Y_p\simeq1/4$ and the [hydrogen mass fraction](../../../stellar-astrophysics.md#hydrogen-mass-fraction) is $X_p\simeq3/4$. The assumptions require $n_p\ge n_n$ and negligible free neutrons, [deuterium](../../../chemistry.md#deuterium) and [helium-3](../../../chemistry.md#helium-3): the phrase hydrogen and helium must here mean predominantly hydrogen-1 and [helium-4](../../../chemistry.md#helium-4), not an arbitrary mixture of helium isotopes.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For a moderately faster [cosmic expansion](../../../cosmology.md#expansion-of-the-universe) that still permits efficient nuclear burning, **the hydrogen mass fraction is smaller**, since cooling from [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out) to helium formation takes less time, fewer free [neutrons](../../../physics.md#neutron) decay into [protons](../../../physics.md#proton), and more surviving neutrons enter [helium-4](../../../chemistry.md#helium-4). If the change also affects [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out), its higher freeze-out [temperature](../../../thermodynamics.md#temperature) leaves a larger initial [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio) and reinforces the helium increase. The conclusion assumes efficient [neutron-limited helium synthesis](../../../cosmology.md#neutron-limited-helium-synthesis): an unspecified arbitrarily rapid expansion could instead outrun the [nuclear reactions](../../../physics.md#nuclear-reaction), so the [nuclear-burning qualification of the helium expansion-rate response](../../../cosmology.md#nuclear-burning-qualification-of-the-helium-expansion-rate-response) prevents an unconditional assertion.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

**True as a major quantitative test of the hot Big Bang, with a significant lithium qualification.** [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) predicts several abundances from one main baryon-density parameter using measured nuclear and weak rates, rather than fitting a separate primordial composition for every species. Comparisons involve distinct observing environments and an independent [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) determination at a much later epoch. Their overall agreement is powerful; it is not a claim that every light-element measurement is mutually consistent without stellar or observational corrections. The [cosmological lithium problem](../../../cosmology.md#cosmological-lithium-problem) must be included in that assessment.

<h4 id="4/iii/a">a</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#4/iii/a)

The main abundance parameter is the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) $\eta=n_B/n_\gamma$, often expressed as $\eta_{10}=10^{10}\eta$. For the measured mean [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) temperature, $\eta_{10}\simeq274\Omega_bh^2$. Standard [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) also depends on the expansion rate, the [effective number of neutrino species](../../../cosmology.md#effective-number-of-neutrino-species), the neutron lifetime and the [nuclear reaction](../../../physics.md#nuclear-reaction) rates.

<a id="4/iii/a/image-schematic-primordial-deuterium-helium-3-helium-4-and-lithium-7-abundance-trends-versus-baryon-to-photon-ratio"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-74-abundances.png)

**[Figure 3](#4/iii/a/image-schematic-primordial-deuterium-helium-3-helium-4-and-lithium-7-abundance-trends-versus-baryon-to-photon-ratio). Schematic primordial deuterium, helium-3, helium-4 and lithium-7 abundance trends versus baryon-to-photon ratio**.

The curves show qualitative abundance trends and representative orders of magnitude; they are simple illustrative functions, not outputs of a [nuclear reaction](../../../physics.md#nuclear-reaction) network. [Helium-4](../../../chemistry.md#helium-4) uses the right-hand mass-fraction axis, while the other three abundances are number ratios to hydrogen on the logarithmic left axis. The lithium valley and its rising high-density branch are important and must not be replaced by a monotone curve.

At higher $\eta$, two-body reactions proceed more rapidly relative to [cosmic expansion](../../../cosmology.md#expansion-of-the-universe) and burn [deuterium](../../../chemistry.md#deuterium) more efficiently, so D/H falls strongly, approximately as $\eta^{-1.6}$ near the favored density. [Helium-3](../../../chemistry.md#helium-3) decreases more gently. The [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) rises only weakly: an earlier end to the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck) allows fewer neutrons to decay, but most surviving neutrons would already end in [helium-4](../../../chemistry.md#helium-4). [Lithium-7](../../../chemistry.md#lithium-7) first decreases as its destruction becomes effective, then increases when [beryllium-7](../../../chemistry.md#beryllium-7) production dominates; [beryllium-7](../../../chemistry.md#beryllium-7) later captures an electron and becomes [lithium-7](../../../chemistry.md#lithium-7).

A faster expansion changes both freeze-out and the time available for reactions. In units $\hbar=c=k_B=1$, weak neutron–proton conversion has rate $\Gamma_w\propto G_F^2T^5$, whereas $H\propto\sqrt{g_*}T^2/M_{\rm Pl}$; consequently $T_f\propto g_*^{1/6}$. Since the equilibrium [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio) is $e^{-(m_n-m_p)/T_f}$, additional radiation raises it; the shorter subsequent decay interval also raises $Y_p$. At fixed baryon density, moderately faster expansion leaves more unburned [deuterium](../../../chemistry.md#deuterium). A longer neutron lifetime similarly increases neutron survival. These trends assume ordinary efficient burning and no independent modifications of the nuclear or weak rates.

**[Deuterium](../../../chemistry.md#deuterium) is a sensitive baryometer, while [helium-4](../../../chemistry.md#helium-4) is particularly useful as an expansion-rate test.** [Deuterium](../../../chemistry.md#deuterium) is destroyed in stellar processing, and metal-poor absorption systems can approximate its initial abundance well. Helium's weak dependence on $\eta$ limits its precision as a baryometer, and its spectroscopic corrections matter. [Helium-3](../../../chemistry.md#helium-3) is both made and destroyed in [stars](../../../stellar-astrophysics.md#star), complicating extrapolation, while lithium is affected by stellar destruction, transport and atmosphere modeling as well as the [cosmological lithium problem](../../../cosmology.md#cosmological-lithium-problem). Accurate comparisons therefore require nuclear-rate and astrophysical uncertainties, not merely narrow instrumental error bars. The parameter responses are explained in [the primordial nucleosynthesis calculation](https://arxiv.org/abs/astro-ph/0308511).

<h4 id="4/iii/b">b</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#4/iii/b)

The [primordial light-element abundance determination](../../../cosmology.md#primordial-light-element-abundance-determination) uses minimally processed material and estimates its residual processing rather than directly observing the universe at a few minutes old.

For [deuterium](../../../chemistry.md#deuterium), high-redshift, low-metallicity [quasar](../../../astrophysics.md#quasar) absorption systems resolve isotope-shifted D I lines from the H I Lyman series. The [deuterium](../../../chemistry.md#deuterium) feature is displaced by about $82\,\mathrm{km\,s}^{-1}$ from hydrogen; fitting several transitions and the velocity components distinguishes genuine [deuterium](../../../chemistry.md#deuterium) from an unrelated hydrogen blend. The ratio of the inferred columns estimates D/H after the ionization and component structure are checked. Low metallicity minimizes stellar destruction, giving a representative primordial ratio of roughly $(2.5\text{–}3)\times10^{-5}$.

For [helium-4](../../../chemistry.md#helium-4), helium and hydrogen recombination-emission lines in metal-poor [H II regions](../../../galaxy.md#h-ii-region) of nearby dwarf [galaxies](../../../galaxy.md) give a mass fraction. Several lines constrain [temperature](../../../thermodynamics.md#temperature), [electron number density](../../../statistical-physics.md#electron-number-density) and corrections for collisional excitation, ionization structure, radiative transfer and underlying stellar absorption. Extrapolation of helium enrichment against metallicity towards zero metallicity estimates $Y_p$, approximately $0.24$–$0.25$, corresponding to helium/hydrogen by number near $0.08$.

For [helium-3](../../../chemistry.md#helium-3), the approximately $8.665$ GHz hyperfine line of ${}^3\mathrm{He}^+$ in Galactic [H II regions](../../../galaxy.md#h-ii-region) probes the abundance, with ionization and nebular structure corrections. Stellar production and destruction make its primordial value hard to extract; a characteristic abundance near $10^{-5}$ relative to hydrogen is compatible with standard nucleosynthesis but is not a comparably clean primordial measurement.

For [lithium-7](../../../chemistry.md#lithium-7), the approximately $6708$ Å Li I absorption doublet in warm, old, metal-poor halo [stars](../../../stellar-astrophysics.md#star) gives a photospheric abundance after stellar-atmosphere and effective-temperature corrections. The [Spite plateau](../../../cosmology.md#spite-plateau) suggests an initial number ratio of order $(1\text{–}2)\times10^{-10}$ if depletion is small; transport below the photosphere, nuclear destruction and atmosphere systematics can lower the measured value relative to the birth abundance. Standard [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) at the deuterium- and microwave-background-favored baryon density instead predicts several $10^{-10}$, roughly $(4\text{–}5)\times10^{-10}$ in exam-era calculations. This discrepancy is the [cosmological lithium problem](../../../cosmology.md#cosmological-lithium-problem), not a measurement of an independently adjustable primordial lithium parameter.

The approximate values deliberately represent exam-era orders of magnitude rather than a claim of current precision; [the contemporary abundance assessment](https://arxiv.org/abs/astro-ph/0308511) discusses the inference and tensions.

<h4 id="4/iii/c">c</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#4/iii/c)

[Deuterium](../../../chemistry.md#deuterium) and [helium-4](../../../chemistry.md#helium-4) broadly favor the same baryon-density range in standard [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), after systematic and reaction-rate uncertainties are allowed. Near the illustrative value $\eta_{10}\sim6$, the [baryon-density consistency between nucleosynthesis and the microwave background](../../../cosmology.md#baryon-density-consistency-between-nucleosynthesis-and-the-microwave-background) gives

$$
\boxed{\Omega_bh^2\sim0.022,\qquad \Omega_b\sim0.045\quad(h\sim0.7).}
$$

[Deuterium](../../../chemistry.md#deuterium) constrains this particularly sharply; [helium-4](../../../chemistry.md#helium-4) gives a weaker baryon-density constraint and a useful test of the expansion rate. [Helium-3](../../../chemistry.md#helium-3) observations do not supply an equally precise independent consistency test because of stellar processing. Lithium inferred directly from the metal-poor stellar plateau is lower than the standard prediction at this density by a factor of a few. Thus **broad concordance is real, but complete four-element concordance without qualifications is false**.

An independent baryon density comes from the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) acoustic pattern, especially the relative odd and even peak heights set by baryon loading of the photon–baryon fluid. For a numerical comparison appropriate to this paper's era, [the 2003 microwave-background and large-scale-structure analysis](https://arxiv.org/abs/astro-ph/0302209) obtained $\Omega_bh^2=0.0224\pm0.0009$, consistent with the density inferred from [deuterium](../../../chemistry.md#deuterium). This comparison spans the first minutes and the much later recombination epoch, and tests the thermal history and conservation of [baryon number](../../../standard-model.md#baryon-number) relative to photon entropy between them; it is more substantial than comparing several abundance fits sharing the same nuclear model.

Ionization-corrected [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) gas inventories and baryon fractions in galaxy clusters provide further checks, with their own radiation, gas-physics and total-mass uncertainties. A total matter fraction of order $\Omega_m\sim0.3$ is much larger than $\Omega_b\sim0.045$, so the abundance result also supports a predominantly nonbaryonic matter component. The lithium discrepancy and abundance systematics motivate continued tests; they do not erase the agreement between two physically distinct baryon-density determinations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
