# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper66.pdf)

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [a](#4/iv/a)
      - [Solution](#4/iv/a/solution)
    - [b](#4/iv/b)
      - [Solution](#4/iv/b/solution)
    - [c](#4/iv/c)
      - [Solution](#4/iv/c/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $H=\dot a/a$ for the [Hubble parameter](../../../cosmology.md#hubble-parameter). Subtracting the [Friedmann equation](../../../cosmology.md#friedmann-equations) from the second equation gives the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation),

$$
\frac{\ddot a}{a}=-\frac{4\pi G}{3}\left(\rho+\frac{3p}{c^2}\right)+\frac{\Lambda c^2}{3}.
$$

Since $\dot H=\ddot a/a-H^2$, eliminating $H^2$ with the first equation yields

$$
\dot H-\frac{kc^2}{a^2}=-4\pi G\left(\rho+\frac p{c^2}\right).
$$

Differentiating the first equation, with constant [cosmological constant](../../../cosmology.md#cosmological-constant) and curvature parameter, now gives

$$
\frac{8\pi G}{3}\dot\rho=2H\left(\dot H-\frac{kc^2}{a^2}\right)=-8\pi GH\left(\rho+\frac p{c^2}\right).
$$

Thus the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) is $\dot\rho+3H(\rho+p/c^2)=0$. Multiplying by $a^3$ and using $d(a^3)/dt=3Ha^3$ proves

$$
\boxed{\frac{d}{dt}(\rho a^3)+\frac p{c^2}\frac{d}{dt}(a^3)=0.}
$$

This is local [conservation of energy](../../../physics.md#conservation-of-energy): expansion changes the energy in a [comoving volume](../../../cosmology.md#comoving-volume) through pressure work.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

With constant [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) $w$, the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) becomes $\dot\rho+3(1+w)H\rho=0$. Consequently

$$
\frac{d}{dt}\bigl(\rho a^{3(1+w)}\bigr)=a^{3(1+w)}\bigl[\dot\rho+3(1+w)H\rho\bigr]=0,
\qquad\boxed{\rho a^{3(1+w)}=C.}
$$

The [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) includes $\rho\propto a^{-3}$ for [pressureless matter](../../../cosmology.md#pressureless-matter) and $\rho\propto a^{-4}$ for [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For $w=-1$, [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) makes $\rho_{\rm DE}$ constant. In the first [Friedmann equation](../../../cosmology.md#friedmann-equations), its contribution combines with the [cosmological constant](../../../cosmology.md#cosmological-constant) as

$$
\frac{8\pi G\rho_{\rm DE}}3+\frac{\Lambda c^2}3=\frac{\Lambda_{\rm eff}c^2}3,
\qquad\boxed{\Lambda_{\rm eff}=\Lambda+\frac{8\pi G\rho_{\rm DE}}{c^2}.}
$$

In the second equation, $-8\pi Gp_{\rm DE}/c^2=8\pi G\rho_{\rm DE}$ produces precisely the same shift of $\Lambda c^2$. Therefore homogeneous expansion measures the sum of these contributions; a constant-density fluid with $p=-\rho c^2$ is dynamically indistinguishable from [cosmological constant energy](../../../cosmology.md#cosmological-constant) in these equations.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Define the present [critical density](../../../cosmology.md#critical-density) and [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) by

$$
\rho_{\rm crit,0}=\frac{3H_0^2}{8\pi G},\qquad\Omega_{{\rm DE},0}=\frac{\rho_{{\rm DE},0}}{\rho_{\rm crit,0}}.
$$

Spatial flatness with $\Lambda=0$ implies $\Omega_{M,0}=1-\Omega_{{\rm DE},0}$. [Separately conserved cosmological fluids](../../../cosmology.md#separately-conserved-cosmological-fluids) and [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) give $\rho_M=\rho_{M,0}a^{-3}$ and $\rho_{\rm DE}=\rho_{{\rm DE},0}a^{-3(1+w)}$. Inserting both into the [Friedmann equation](../../../cosmology.md#friedmann-equations) yields

$$
\boxed{H(a)^2=H_0^2\left[(1-\Omega_{{\rm DE},0})a^{-3}+\Omega_{{\rm DE},0}a^{-3(1+w)}\right]=H_0^2\left[\Omega_{{\rm DE},0}a^{-3}(a^{-3w}-1)+a^{-3}\right].}
$$

This is the constant-$w$ case of the [Hubble parameter for matter and dynamical dark energy](../../../cosmology.md#hubble-parameter-for-matter-and-dynamical-dark-energy).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Assume both densities are nonnegative and $\Omega_{{\rm DE},0}<1$, so a nonzero [pressureless matter](../../../cosmology.md#pressureless-matter) component exists. Their ratio obeys

$$
\boxed{\frac{\rho_{\rm DE}}{\rho_M}=\frac{\Omega_{{\rm DE},0}}{1-\Omega_{{\rm DE},0}}a^{-3w}\longrightarrow0\quad(a\to0,\ w<0).}
$$

Thus [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) gives

$$
\boxed{H(a)\sim H_0\sqrt{1-\Omega_{{\rm DE},0}}\,a^{-3/2}.}
$$

At fixed $H_0$, the early expansion rate does depend on the present [dark energy](../../../cosmology.md#dark-energy) fraction: increasing it reduces $\rho_{M,0}=(1-\Omega_{{\rm DE},0})3H_0^2/(8\pi G)$. There is no contradiction with negligible early [dark energy](../../../cosmology.md#dark-energy), since the leading expression is simply $H^2\sim8\pi G\rho_M/3$. At fixed physical matter density, that leading rate is independent of the negligible component.

The endpoint $\Omega_{{\rm DE},0}=1$ has no matter, so the ratio argument does not apply. Its [Hubble parameter](../../../cosmology.md#hubble-parameter) is $H=H_0a^{-3(1+w)/2}$: it diverges for $-1<w<0$, is constant for $w=-1$, and tends to zero for $w<-1$.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For [pressureless matter](../../../cosmology.md#pressureless-matter) and zero [cosmological constant](../../../cosmology.md#cosmological-constant), the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) gives $\ddot a/a=-4\pi G\rho/3$. The [deceleration parameter](../../../cosmology.md#deceleration-parameter) therefore satisfies the [dust relation between deceleration and density](../../../cosmology.md#dust-relation-between-deceleration-and-density), $q=4\pi G\rho/(3H^2)$. Evaluating today,

$$
\boxed{\rho_0=\frac{3H_0^2q_0}{4\pi G}.}
$$

Substitute this into the present [Friedmann equation](../../../cosmology.md#friedmann-equations) to obtain $H_0^2+kc^2/a_0^2=2q_0H_0^2$, or

$$
\boxed{\frac{kc^2}{a_0^2}=(2q_0-1)H_0^2.}
$$

In particular, $q_0>1/2$, $q_0=1/2$, and $q_0<1/2$ correspond to positive, zero, and negative spatial curvature.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Normalize the [scale factor](../../../cosmology.md#scale-factor-cosmology) by $x=a/a_0$. [Constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) for [pressureless matter](../../../cosmology.md#pressureless-matter) gives $\rho=\rho_0x^{-3}$. Multiplying the [Friedmann equation](../../../cosmology.md#friedmann-equations) by $x^2$ and substituting the expressions from part (i),

$$
\dot x^2=\frac{8\pi G\rho_0}{3x}-\frac{kc^2}{a_0^2}=H_0^2\left(\frac{2q_0}{x}+1-2q_0\right).
$$

Take the expanding branch $\dot x>0$ and set the origin of [cosmic time](../../../cosmology.md#cosmic-time) at the [Big Bang](../../../cosmology.md#big-bang), $x=0$. The [age of a dust universe without a cosmological constant](../../../cosmology.md#age-of-a-dust-universe-without-a-cosmological-constant) is consequently

$$
\boxed{t_0=\frac1{H_0}\int_0^1\left(1-2q_0+\frac{2q_0}{x}\right)^{-1/2}\,dx.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The stated real trigonometric substitution applies to the closed case $q_0>1/2$. Set $A=2q_0-1$, so $x=q_0(1-\cos\theta)/A$, $dx=q_0\sin\theta\,d\theta/A$, and

$$
1-2q_0+\frac{2q_0}{x}=A\frac{1+\cos\theta}{1-\cos\theta}.
$$

The upper limit obeys $1-\cos\theta_*=A/q_0$, with $0<\theta_*<\pi$ on the expanding branch. Substitution into the [age of a dust universe without a cosmological constant](../../../cosmology.md#age-of-a-dust-universe-without-a-cosmological-constant) yields

$$
\boxed{H_0t_0=\frac{q_0}{(2q_0-1)^{3/2}}\int_0^{\theta_*}\frac{\sin\theta\sqrt{1-\cos\theta}}{\sqrt{1+\cos\theta}}\,d\theta.}
$$

On this interval, the integrand equals $1-\cos\theta$, so it can also be evaluated:

$$
H_0t_0=\frac{q_0(\theta_*-\sin\theta_*)}{(2q_0-1)^{3/2}},\qquad\cos\theta_*=\frac{1-q_0}{q_0}.
$$

For $q_0=1/2$, the original integral instead gives $H_0t_0=2/3$. For $0<q_0<1/2$, use a hyperbolic substitution to obtain $H_0t_0=q_0(\sinh\eta_*-\eta_*)/(1-2q_0)^{3/2}$, where $\cosh\eta_*=(1-q_0)/q_0$. A real $\theta$ cannot implement the printed substitution in that open case.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

An empty universe with $\Lambda=0$ has $\Omega_{r,0}=\Omega_{m,0}=\Omega_{\Lambda,0}=0$. The present [Friedmann equation](../../../cosmology.md#friedmann-equations) then requires $\Omega_{k,0}=1$, so

$$
\boxed{H(z)=H_0(1+z).}
$$

The [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) gives $\ddot a=0$, hence $a\propto t$ after choosing its zero at $t=0$, and

$$
\boxed{q_0=0.}
$$

This is the [Milne universe](../../../cosmology.md#milne-model). A larger past [Hubble parameter](../../../cosmology.md#hubble-parameter) does not require negative $\ddot a$: even constant $\dot a$ produces $H=\dot a/a=1/t$. Equivalently, [deceleration parameter from the Hubble derivative](../../../cosmology.md#deceleration-parameter-from-the-hubble-derivative) gives $q=-1-\dot H/H^2=-1+1=0$. The age is $t_0=H_0^{-1}$.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) is the collection of [absorption lines](../../../stellar-astrophysics.md#absorption-line) blueward of a distant [quasar](../../../astrophysics.md#quasar)'s own [Lyman-alpha line](../../../physics.md#lyman-alpha-line). Foreground neutral hydrogen removes photons at rest wavelength $\lambda_\alpha\simeq1215.67$ angstroms, observed at $\lambda=(1+z)\lambda_\alpha$ because of [cosmological redshift](../../../cosmology.md#cosmological-redshift). Gas at many different foreground redshifts therefore produces many lines. The weak forest traces diffuse, mostly ionized [intergalactic medium](../../../astrophysics.md#intergalactic-medium), rather than a population of fully neutral clouds; much stronger, self-shielded absorbers are a separate regime. [Madau's account of quasar absorption systems](https://ned.ipac.caltech.edu/level5/Madau6/Madau2.html) distinguishes these column-density regimes.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For highly ionized hydrogen in [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium), balance the [photoionization rate](../../../physics.md#photoionization-rate) against [radiative recombination](../../../physics.md#radiative-recombination):

$$
n_{\rm HI}\Gamma_{\rm HI}=\alpha(T)n_en_{\rm HII}\simeq\alpha(T)n_H^2.
$$

Thus the neutral fraction is $n_{\rm HI}/n_H\simeq\alpha(T)n_H/\Gamma_{\rm HI}$ and the neutral [column density](../../../statistical-physics.md#column-density) across a proper path $L$ is

$$
N_{\rm HI}\simeq\frac{\alpha(T)n_H^2L}{\Gamma_{\rm HI}}.
$$

For an illustrative diffuse gas with $T\sim10^4\,\mathrm K$, $\alpha\sim4\times10^{-13}\,\mathrm{cm^3\,s^{-1}}$, $\Gamma_{\rm HI}\sim10^{-12}\,\mathrm{s^{-1}}$, and $n_H\sim10^{-5}\,\mathrm{cm^{-3}}$, the neutral fraction is only $4\times10^{-6}$. A proper path of $100$ kiloparsecs then gives $N_{\rm HI}\sim10^{13}\,\mathrm{cm^{-2}}$, enough to produce a weak [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption) feature even though the gas is almost entirely ionized.

This hydrogen [number density](../../../statistical-physics.md#number-density) is of the order of the cosmic mean at redshift a few. Since the weak forest is common along most high-redshift [lines of sight](../../../astrophysics.md#line-of-sight), substantial path length passes through such diffuse gas. Much denser material would give much larger [column density](../../../statistical-physics.md#column-density) for comparable path lengths and ionizing flux. These arguments support near-mean or modestly overdense [intergalactic medium](../../../astrophysics.md#intergalactic-medium) as the origin of weak forest lines, not the claim that every absorber has exactly the cosmic mean density: path length, temperature, and [ionizing background](../../../astrophysics.md#cosmic-ionizing-background) must also be constrained.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A radial [null geodesic](../../../special-relativity.md#null-geodesic) in the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) obeys $d\chi=c\,|dt|/a$. The [redshift-time relation](../../../cosmology.md#redshift-time-relation) $dt=-dz/[(1+z)H(z)]$, with $a_0=1$, therefore gives

$$
\Delta\chi=c\int_{z_1}^{z_2}\frac{dz}{H(z)}\simeq\boxed{\frac{c\,\Delta z}{H(\bar z)}},\qquad\bar z=\frac{z_1+z_2}{2}.
$$

This is [comoving radial distance](../../../cosmology.md#comoving-radial-distance). The [proper distance in cosmology](../../../cosmology.md#proper-distance-in-cosmology) at the clouds' approximately common epoch is instead

$$
\boxed{\Delta d_{\rm proper}\simeq\frac{c\,\Delta z}{(1+\bar z)H(\bar z)}.}
$$

The distinction is essential when quoting a cloud separation. The approximation neglects the change of $H$ across the interval and assumes the observed spacing is dominated by [cosmological redshift](../../../cosmology.md#cosmological-redshift); [peculiar velocity](../../../cosmology.md#peculiar-velocity) can perturb the inferred separation. It is the redshift version of [proper absorber separation from a wavelength interval](../../../cosmology.md#proper-absorber-separation-from-a-wavelength-interval).

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The [quasar proximity effect](../../../astrophysics.md#proximity-effect-astrophysics) is weaker [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) absorption near a [quasar](../../../astrophysics.md#quasar)'s emission redshift. Extra photons from the [quasar](../../../astrophysics.md#quasar) increase the [photoionization rate](../../../physics.md#photoionization-rate) and reduce the neutral fraction without necessarily reducing the total gas density.

For isotropic [specific intensity](../../../astrophysics.md#specific-intensity) $J_\nu$ and a steady, isotropically radiating [quasar](../../../astrophysics.md#quasar) with [spectral luminosity](../../../astrophysics.md#spectral-luminosity) $L_\nu$, the background and local rates are

$$
\Gamma_{\rm bg}=4\pi\int_{\nu_0}^\infty\frac{J_\nu\sigma_\nu}{h\nu}\,d\nu,\qquad\Gamma_Q(r)=\int_{\nu_0}^\infty\frac{L_\nu\sigma_\nu}{4\pi r^2h\nu}\,d\nu.
$$

Here $r$ is a proper separation small enough that attenuation and expansion across it can initially be neglected, and $\sigma_\nu$ is the hydrogen photoionization cross-section. At fixed density and temperature, [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium) makes the neutral [column density](../../../statistical-physics.md#column-density), and hence a given line's [optical depth](../../../astrophysics.md#optical-depth), scale as

$$
\boxed{\frac{\tau(r)}{\tau_{\rm field}}\simeq\frac{\Gamma_{\rm bg}}{\Gamma_{\rm bg}+\Gamma_Q(r)}.}
$$

The observed [quasar](../../../astrophysics.md#quasar) luminosity supplies $\Gamma_Q(r)$; the distance at which the absorption changes significantly estimates where $\Gamma_Q\sim\Gamma_{\rm bg}$. Adopting a background spectral shape then converts the inferred rate to its [specific intensity](../../../astrophysics.md#specific-intensity), often quoted near the hydrogen [ionization energy](../../../physics.md#ionization-energy) threshold.

Important uncertainties include an enhanced gas [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) around the host, the unobserved ionizing spectrum, anisotropic emission, source lifetime and variability, the systemic redshift and continuum placement, attenuation between source and absorber, and fluctuations between [lines of sight](../../../astrophysics.md#line-of-sight). Higher gas density enhances recombination and can partially hide the effect, biasing a simple background estimate upward. [Dall'Aglio, Wisotzki and Worseck's 2008 measurements](https://arxiv.org/abs/0801.1767) illustrate the observed sightline scatter and the roles of variability and clustering.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

The [ionizing background](../../../astrophysics.md#cosmic-ionizing-background) is produced mainly by hot stars in [star-forming galaxies](../../../galaxy.md#star-forming-galaxy) and by accretion-powered [quasars](../../../astrophysics.md#quasar). The stellar contribution depends on [star formation](../../../stellar-astrophysics.md#star-formation) and the [ionizing photon escape fraction](../../../galaxy.md#ionizing-photon-escape-fraction); the [quasar](../../../astrophysics.md#quasar) contribution depends on its evolving [luminosity function](../../../astrophysics.md#luminosity-function-astronomy). [Radiative transfer](../../../astrophysics.md#radiative-transfer) through the [intergalactic medium](../../../astrophysics.md#intergalactic-medium), including absorption, recombination emission, and cosmological redshifting, determines the radiation actually available for [photoionization](../../../physics.md#photoionization).

In the picture relevant to this 2009 paper, increasingly rare [quasars](../../../astrophysics.md#quasar) cannot by themselves explain the high-redshift hydrogen ionizing field, so galaxies become especially important above $z\sim3$. Harder [quasar](../../../astrophysics.md#quasar) radiation is important for doubly ionizing helium around $z\sim3$. Hydrogen [reionization](../../../cosmology.md#reionization) must be largely accomplished by $z\sim6$. At lower redshift the evolution reflects declining source emissivity together with the increasing propagation distance of ionizing photons; near [reionization](../../../cosmology.md#reionization), short absorption lengths and spatially uneven ionized regions prevent a simple uniform-background description. The background rate need not follow the [quasar](../../../astrophysics.md#quasar) population alone: a roughly flat hydrogen [photoionization rate](../../../physics.md#photoionization-rate) over $2\lesssim z\lesssim4$ is compatible with a changing mixture of galaxies and [quasars](../../../astrophysics.md#quasar). [Faucher-Giguère and collaborators' 2009 background calculation](https://arxiv.org/abs/0901.4554) and [their preceding opacity analysis](https://arxiv.org/abs/0807.4177) give this interpretation. These redshifts describe the broad historical picture, rather than precise universal transition times.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) is the maximum radial distance a photon could have travelled since the initial [Big Bang](../../../cosmology.md#big-bang), expressed in [comoving coordinates](../../../cosmology.md#comoving-coordinate). It describes possible past causal contact, whereas a [cosmological event horizon](../../../general-relativity.md#cosmological-event-horizon) concerns photons that can reach an observer in the future.

For a radial [null geodesic](../../../special-relativity.md#null-geodesic) in the [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), $dr/\sqrt{1-kr^2}=c\,dt/a$. Spatial flatness sets $k=0$, so with $a_0=1$,

$$
r_p(t)=c\int_0^t\frac{dt'}{a(t')}=c\int_0^{a(t)}\frac{da'}{a'^2H(a')}.
$$

The given [Hubble parameter](../../../cosmology.md#hubble-parameter) then supplies $a^2H=H_0\sqrt{\Omega_{r,0}+\Omega_{m,0}a+\Omega_{\Lambda,0}a^4}$. Since [cosmological redshift](../../../cosmology.md#cosmological-redshift) obeys $a=(1+z)^{-1}$,

$$
\boxed{r_p(z)=\frac c{H_0}\int_0^{(1+z)^{-1}}\frac{da}{\sqrt{\Omega_{r,0}+\Omega_{m,0}a+\Omega_{\Lambda,0}a^4}}.}
$$

The corresponding proper horizon at that epoch is $a(z)r_p(z)$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Well before [matter-radiation equality](../../../cosmology.md#matter-radiation-equality), [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) makes the integrand approximately constant:

$$
r_p(a)\simeq\frac{ca}{H_0\sqrt{\Omega_{r,0}}}.
$$

At equality, $\Omega_{r,0}a_{\rm eq}^{-4}=\Omega_{m,0}a_{\rm eq}^{-3}$, so $a_{\rm eq}\simeq1/3000$ and $\Omega_{r,0}\simeq10^{-4}$. Extrapolating the radiation-only result gives $r_p(a_{\rm eq})\simeq133\,\mathrm{Mpc}$. This overestimates the horizon because matter is no longer negligible at equality and increases the expansion rate.

Retain both matter and radiation, still neglecting the insignificant early [cosmological constant](../../../cosmology.md#cosmological-constant). The [particle horizon through radiation-matter equality](../../../cosmology.md#particle-horizon-through-radiation-matter-equality) is

$$
r_p(a)=\frac{2c}{H_0\Omega_{m,0}}\left(\sqrt{\Omega_{r,0}+\Omega_{m,0}a}-\sqrt{\Omega_{r,0}}\right).
$$

Therefore

$$
\boxed{r_p(a_{\rm eq})\simeq2(\sqrt2-1)(133\,\mathrm{Mpc})\simeq110\,\mathrm{Mpc}.}
$$

This is a comoving distance; the proper horizon at equality is approximately $110/3000\,\mathrm{Mpc}\simeq37$ kiloparsecs.

For today's horizon, extrapolating [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) gives

$$
r_p(1)\simeq\frac c{H_0}\int_0^1\frac{da}{\sqrt{\Omega_{m,0}a}}=\frac{2c}{H_0\sqrt{\Omega_{m,0}}}\simeq1.46\times10^4\,\mathrm{Mpc}.
$$

This is an order-of-magnitude estimate: [dark energy](../../../cosmology.md#dark-energy) is significant late, and radiation matters early. Numerical integration of the complete expression with the supplied density parameters and $\Omega_{r,0}\simeq10^{-4}$ gives

$$
\boxed{r_p(t_0)\simeq1.30\times10^4\,\mathrm{Mpc}.}
$$

Both neglected positive-density terms increase $H$ at fixed $a$ and reduce the horizon relative to the matter-only extrapolation.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The [distance modulus](../../../astrophysics.md#distance-modulus) gives $m_V-M_V=5\log_{10}(d/10\,\mathrm{pc})$. At the magnitude limit, $m_V-M_V=17-(-21)=38$, so

$$
d=10^{1+38/5}\,\mathrm{pc}=10^{8.6}\,\mathrm{pc},\qquad\boxed{d\simeq398\,\mathrm{Mpc}\simeq400\,\mathrm{Mpc}.}
$$

Thus the stated sample reaches a typical galaxy to approximately $400$ megaparsecs. This uses the assumed [absolute magnitude](../../../astrophysics.md#absolute-magnitude), neglects the specified spectral correction, and equates [luminosity distance](../../../cosmology.md#luminosity-distance), [angular diameter distance](../../../cosmology.md#angular-diameter-distance), and proper distance as permitted. It does not imply completeness for galaxies fainter than the adopted typical luminosity.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/a">a</h4>

↑ **Parent:** [Iv](#4/iv)

<h5 id="4/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#4/iv/a)

The plot uses comoving [wavenumber](../../../wave-equation.md#wavenumber) in $\mathrm{Mpc^{-1}}$. Using the inverse [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) from part (ii) gives $1/r_{p,\rm eq}\simeq9\times10^{-3}\,\mathrm{Mpc^{-1}}$. The conventional [matter-radiation equality scale](../../../cosmology.md#matter-radiation-equality-scale) is instead

$$
k_{\rm eq}=\frac{a_{\rm eq}H_{\rm eq}}c\simeq\frac{H_0}c\sqrt{\frac{2\Omega_{m,0}}{a_{\rm eq}}}\simeq\boxed{1.1\times10^{-2}\,\mathrm{Mpc^{-1}}.}
$$

These are consistent order-one conventions for locating the turnover near $10^{-2}\,\mathrm{Mpc^{-1}}$. The horizon-entry condition is $k/(aH/c)\sim1$; equating an entire Fourier wavelength $2\pi/k$ to the particle horizon would attach a different numerical factor.

For [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions), the [asymptotic cold-dark-matter power spectrum](../../../linear-cosmological-perturbation-theory.md#asymptotic-cold-dark-matter-power-spectrum) has $P(k)\propto k^{n_s}T(k)^2$, where the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) is $n_s\simeq1$ and $T$ is the [cosmological transfer function](../../../linear-cosmological-perturbation-theory.md#cosmological-transfer-function). Modes below $k_{\rm eq}$ enter during [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) and have little relative suppression, giving approximately $P\propto k$. Modes above $k_{\rm eq}$ enter during [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), when [logarithmic growth of matter perturbations during radiation domination](../../../linear-cosmological-density-perturbation.md#logarithmic-growth-of-matter-perturbations-during-radiation-domination) is much slower. Their transfer is approximately $T\propto\ln(k/k_{\rm eq})/k^2$, giving $P\propto k^{-3}\ln^2(k/k_{\rm eq})$ well above equality. This explains the broad turnover; [baryon acoustic oscillations](../../../cosmology.md#baryon-acoustic-oscillation) add structure, and nonlinear evolution modifies sufficiently small scales.

<h4 id="4/iv/b">b</h4>

↑ **Parent:** [Iv](#4/iv)

<h5 id="4/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#4/iv/b)

The comoving distance to the [Cosmic microwave background last-scattering surface](../../../cosmology.md#cosmic-microwave-background-last-scattering-surface) is of order the present horizon, $\chi_*\sim1.3\times10^4\,\mathrm{Mpc}$. At recombination the particle horizon is much smaller, so replacing $\chi_*$ by today's horizon is adequate for the requested estimate. A transverse [Fourier mode](../../../fourier-analysis.md#fourier-mode) projects approximately to angular multipole $\ell\sim k\chi_*$. If an angular feature's width is estimated by $\theta\sim1/\ell$, the resolution $\theta_{\min}\sim10^{-3}$ gives

$$
k_{\max}\sim\frac1{\chi_*\theta_{\min}}\sim0.08\,\mathrm{Mpc^{-1}}.
$$

Using the common half-wavelength convention $\theta\sim\pi/\ell$ instead gives $\ell_{\max}\sim3000$ and $k_{\max}\sim0.2$--$0.3\,\mathrm{Mpc^{-1}}$. These express the same order-of-magnitude resolution estimate with different angular-scale conventions. On the graph, a useful indicative band is therefore **from about $10^{-4}\,\mathrm{Mpc^{-1}}$ to order $10^{-1}\,\mathrm{Mpc^{-1}}$, potentially a few times $10^{-1}$**; it is not a sharp instrumental boundary. The lowest useful multipoles are of order a few, with substantial [cosmic variance](../../../cosmic-microwave-background-anisotropy.md#cosmic-variance).

The [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) constrains the [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) indirectly through the primordial spectrum and radiation/matter [cosmological transfer functions](../../../linear-cosmological-perturbation-theory.md#cosmological-transfer-function). Beam resolution, [Cosmic microwave background diffusion damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping), foreground emission, and projection of three-dimensional fluctuations into angular anisotropy limit the recoverable small-scale information. Resolving a given angle alone does not guarantee a precise matter-spectrum measurement there.

<h4 id="4/iv/c">c</h4>

↑ **Parent:** [Iv](#4/iv)

<h5 id="4/iv/c/solution">Solution</h5>

↑ **Parent:** [C](#4/iv/c)

A survey depth $R\sim400\,\mathrm{Mpc}$ makes wavelengths substantially larger than its volume poorly measurable. A characteristic inverse depth is $1/R\simeq2.5\times10^{-3}\,\mathrm{Mpc^{-1}}$; a Fourier wavelength that fits across a dimension $L$ instead requires $k\gtrsim2\pi/L$. For $L$ between $R$ and $2R$, this is roughly $0.008$--$0.016\,\mathrm{Mpc^{-1}}$. A limited sky patch can have smaller transverse dimensions, so its [survey window function](../../../large-scale-structure-of-the-universe.md#survey-window-function) raises the practical minimum in those directions. An indicative useful band for a broad survey is **around $10^{-2}\,\mathrm{Mpc^{-1}}$ and above**, including scales near equality if its volume is large enough.

There is no upper [wavenumber](../../../wave-equation.md#wavenumber) determined by depth alone. Mean separation of observed galaxies, [galaxy power spectrum shot noise](../../../large-scale-structure-of-the-universe.md#galaxy-power-spectrum-shot-noise), angular/redshift resolution, and nonlinear clustering set it. Straightforward linear inference is typically restricted to roughly $k\lesssim0.1\,\mathrm{Mpc^{-1}}$ at low redshift, with smaller scales requiring modelling. The magnitude limit does not specify the galaxy [comoving number density](../../../cosmology.md#comoving-number-density), so a more precise sampling cutoff cannot be deduced from these data.

The two measurements are complementary. The [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) samples a large volume at an early epoch when relevant perturbations are mostly linear, and is free of [galaxy bias](../../../large-scale-structure-of-the-universe.md#galaxy-bias); its matter-spectrum inference is indirect and depends on projection, cosmological parameters, foregrounds, and [cosmic variance](../../../cosmic-microwave-background-anisotropy.md#cosmic-variance). A [galaxy survey](../../../large-scale-structure-of-the-universe.md#galaxy-survey) gives three-dimensional late-time information and can reach smaller scales, but observes biased, discrete tracers: [galaxy bias](../../../large-scale-structure-of-the-universe.md#galaxy-bias), nonlinear gravitational growth, [redshift-space distortions](../../../large-scale-structure-of-the-universe.md#redshift-space-distortions), selection effects, and [galaxy power spectrum shot noise](../../../large-scale-structure-of-the-universe.md#galaxy-power-spectrum-shot-noise) must be controlled. Combining both constrains the initial spectrum and its subsequent growth more strongly than either alone, while their overlapping modes test the inferred evolution.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
