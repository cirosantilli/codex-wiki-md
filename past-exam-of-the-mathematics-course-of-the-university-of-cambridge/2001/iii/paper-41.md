# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper41.pdf)

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
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)

## 1

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a radial [null geodesic](../../../special-relativity.md#null-geodesic) in the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), define $\chi(r)=\int_0^r(1-kr'^2)^{-1/2}\,dr'$. Two successive wave crests emitted and received at the same comoving positions obey

$$
\chi_e=c\int_{t_e}^{t_0}\frac{dt}{a(t)}
=c\int_{t_e+\Delta t_e}^{t_0+\Delta t_0}\frac{dt}{a(t)}.
$$

Subtracting and keeping the first order in the wave periods gives $\Delta t_0/a(t_0)=\Delta t_e/a(t_e)$. Thus the [cosmological time dilation](../../../cosmology.md#cosmological-time-dilation) and the [cosmological redshift](../../../cosmology.md#cosmological-redshift) have the same factor:

$$
\boxed{1+z=\frac{\lambda_0}{\lambda_e}
=\frac{\nu_e}{\nu_0}
=\frac{\Delta t_0}{\Delta t_e}
=\frac{a(t_0)}{a(t_e)}=\frac1{a(t_e)}.}
$$

Here the emitter and observer are comoving; an additional [peculiar velocity](../../../cosmology.md#peculiar-velocity) would supply a separate [kinematic redshift](../../../physics.md#kinematic-redshift). The derivation uses the [null geodesic](../../../special-relativity.md#null-geodesic) propagation of the crests rather than interpreting a finite cosmological distance as an ordinary [Doppler effect](../../../physics.md#doppler-effect).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [luminosity distance](../../../cosmology.md#luminosity-distance) is defined by $F=L/(4\pi d_L^2)$, where $L$ is the [bolometric luminosity](../../../astrophysics.md#luminosity) and $F$ the received [radiative flux](../../../astrophysics.md#radiative-flux). In the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) a sphere through the observer around a comoving source has area $4\pi a_0^2r_e^2$. The [cosmological redshift](../../../cosmology.md#cosmological-redshift) reduces each photon's [energy](../../../classical-mechanics.md#energy) by $(1+z)^{-1}$, and [cosmological time dilation](../../../cosmology.md#cosmological-time-dilation) reduces their arrival rate by another such factor. Hence

$$
F=\frac{L}{4\pi a_0^2r_e^2(1+z)^2},
\qquad \boxed{d_L=(1+z)a_0r_e=(1+z)r_e.}
$$

The positive radial lookback integral is $\chi_e=c\int_{t_e}^{t_0}dt/a(t)=\int_0^{r_e}dr/\sqrt{1-kr^2}$. The printed time limits are reversed; also the factor $c$ is required unless units $c=1$ are adopted. The areal coordinate $r_e$ and the radial [comoving distance](../../../cosmology.md#comoving-radial-distance) $\chi_e$ agree only when $k=0$.

For an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $H(z)=H_0(1+z)^{3/2}$. Using the [redshift-time relation](../../../cosmology.md#redshift-time-relation) in the radial [null geodesic](../../../special-relativity.md#null-geodesic) integral yields

$$
r_e=c\int_0^z\frac{dz'}{H(z')}
=\frac{2c}{H_0}\left[1-(1+z)^{-1/2}\right].
$$

Thus the [Einstein-de Sitter luminosity-distance relation](../../../cosmology.md#einstein-de-sitter-luminosity-distance-relation) is

$$
\boxed{d_L(z)=\frac{2c}{H_0}\left[(1+z)-\sqrt{1+z}\right].}
$$

Its small-[redshift](../../../optics.md#redshift) expansion $d_L=(c/H_0)[z+z^2/4+O(z^3)]$ recovers [Hubble's law](../../../cosmology.md#hubble-s-law).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A [Type Ia supernova](../../../stellar-astrophysics.md#type-ia-supernova) can be standardized as a [standard candle](../../../astrophysics.md#standard-candle) by correcting its peak brightness using the [light curve](../../../astrophysics.md#light-curve) shape and [colour index](../../../astrophysics.md#color-index). Its host spectrum gives the [redshift](../../../optics.md#redshift); the corrected [apparent magnitude](../../../astrophysics.md#apparent-magnitude) and calibrated [absolute magnitude](../../../astrophysics.md#absolute-magnitude) give the [distance modulus](../../../astrophysics.md#distance-modulus)

$$
\mu=m-M=5\log_{10}\!\left(\frac{d_L}{10\,\mathrm{pc}}\right).
$$

The resulting [Hubble diagram](../../../cosmology.md#hubble-diagram) measures the shape of the [luminosity distance](../../../cosmology.md#luminosity-distance) as a function of [redshift](../../../optics.md#redshift). A spatially flat matter-and-vacuum model, for example, predicts

$$
d_L(z)=(1+z)\frac{c}{H_0}
\int_0^z\frac{dz'}{\sqrt{\Omega_m(1+z')^3+\Omega_\Lambda}}.
$$

Nonzero [cosmological spatial curvature](../../../cosmology.md#spatial-curvature-of-an-flrw-universe) changes both the expansion rate and the conversion from radial to transverse [comoving distance](../../../cosmology.md#comoving-radial-distance). Comparing the observed [Hubble diagram](../../../cosmology.md#hubble-diagram) with these predictions constrains the [matter density parameter](../../../cosmology.md#matter-density-parameter), [cosmological constant](../../../cosmology.md#cosmological-constant) and [cosmological spatial curvature](../../../cosmology.md#spatial-curvature-of-an-flrw-universe); a single low-[redshift](../../../optics.md#redshift) observation cannot separate them. The nearby sample calibrates the common intercept, while distant [Type Ia supernovae](../../../stellar-astrophysics.md#type-ia-supernova) supply the redshift-dependent shape. Relative faintness at a specified [redshift](../../../optics.md#redshift) means a greater inferred [luminosity distance](../../../cosmology.md#luminosity-distance).

[Type Ia supernova cosmology](../../../cosmology.md#type-ia-supernova-cosmology) requires correction for [interstellar extinction](../../../galaxy.md#interstellar-extinction), possible evolution of the standardized [luminosity](../../../astrophysics.md#luminosity), and [selection bias](../../../causal-inference.md#selection-bias). The [absolute magnitude–Hubble constant degeneracy](../../../cosmology.md#absolute-magnitude-hubble-constant-degeneracy) means that an uncalibrated sample constrains the shape rather than independently determining $H_0$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Use the luminosity convention in the supplied flux relation: $P_\nu=L_\nu/(4\pi)$, where $L_\nu$ is the total [spectral luminosity](../../../astrophysics.md#spectral-luminosity). For a general spectrum $P_\nu\propto\nu^\alpha$, the [cosmological spectral flux-density relation](../../../cosmology.md#cosmological-spectral-flux-density-relation) gives

$$
S_{\nu_0}=\frac{(1+z)P_{(1+z)\nu_0}}{d_L^2}
=\frac{P_{\nu_0}(1+z)^{\alpha-1}}{r_e^2}.
$$

In a spatially flat universe, a shell subtending the [solid angle](../../../geometry-and-topology.md#solid-angle) $d\Omega$ contains $dN=n_0r_e^2dr_e\,d\Omega$ sources, because $n_0$ is their [comoving number density](../../../cosmology.md#comoving-number-density). The [cosmological spectral background](../../../cosmology.md#cosmological-spectral-background) intensity per unit [solid angle](../../../geometry-and-topology.md#solid-angle) is consequently

$$
I_{\nu_0}(z_{\max})
=n_0P_{\nu_0}\int_0^{r_e(z_{\max})}(1+z)^{\alpha-1}dr_e
=\frac{cn_0P_{\nu_0}}{H_0}
\int_0^{z_{\max}}(1+z)^{\alpha-5/2}\,dz.
$$

This is the [cosmological background intensity from comoving emissivity](../../../cosmology.md#cosmological-background-intensity-from-comoving-emissivity) specialized to identical, nonevolving sources in an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe). For $\alpha=1$ the integrand reduces to $(1+z)^{-3/2}$, or directly $dI_{\nu_0}=n_0P_{\nu_0}dr_e$. The finite [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) therefore gives

$$
I_{\nu_0}(z_{\max})=
\frac{2cn_0P_{\nu_0}}{H_0}[1-(1+z_{\max})^{-1/2}],
\qquad
\boxed{I_{\nu_0}(\infty)=\frac{2cn_0P_{\nu_0}}{H_0}.}
$$

For $\alpha=2$, instead,

$$
\boxed{I_{\nu_0}(z_{\max})=
\frac{2cn_0P_{\nu_0}}{H_0}[\sqrt{1+z_{\max}}-1]\longrightarrow\infty.}
$$

The emitted [frequency](../../../physics.md#frequency) grows with [redshift](../../../optics.md#redshift), and the rising [spectral luminosity](../../../astrophysics.md#spectral-luminosity) now defeats the redshift dimming. The [Einstein-de Sitter spectral-background convergence criterion](../../../cosmology.md#einstein-de-sitter-spectral-background-convergence-criterion) is $\alpha<3/2$; equality produces a logarithmic divergence. This divergence describes the unbounded power-law, eternal-population model. A finite formation epoch, a high-frequency spectral break or absorption changes that model and can make its background finite.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The term $2H\dot\delta$ is [Hubble friction](../../../cosmology.md#hubble-friction) in the equation for the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast). During expansion, $H>0$, it damps the peculiar motion producing density growth. It therefore slows [gravitational instability](../../../astrophysical-fluid-dynamics.md#gravitational-instability) relative to the otherwise identical static model; it does not necessarily stop growth.

Multiplying by $a^2$ shows the mechanism without confusing it with microscopic dissipative friction:

$$
\frac{d}{dt}(a^2\dot\delta)=4\pi G\rho_m a^2\delta.
$$

When the self-gravity term is negligible, the [expansion-weighted derivative of a passive density perturbation](../../../linear-cosmological-density-perturbation.md#expansion-weighted-derivative-of-a-passive-density-perturbation) is conserved, so $\dot\delta\propto a^{-2}$. Expansion also reduces $\rho_m\propto a^{-3}$ and hence weakens the source on the right. A contracting background has $H<0$ and reverses the sign of this effect.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For constant $a$ and constant $\rho_m>0$, [Hubble friction](../../../cosmology.md#hubble-friction) vanishes. Put $\omega_J=\sqrt{4\pi G\rho_m}$. The constant-coefficient [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) is $\ddot\delta-\omega_J^2\delta=0$, so its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) has the real [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) $\pm\omega_J$:

$$
\boxed{\delta(t)=C_+e^{\omega_Jt}+C_-e^{-\omega_Jt}.}
$$

These are the pressureless special case of the [Static-universe Jeans modes](../../../linear-cosmological-density-perturbation.md#static-universe-jeans-modes). A positive growing-mode coefficient gives exponential [gravitational instability](../../../astrophysical-fluid-dynamics.md#gravitational-instability), with time scale $(4\pi G\rho_m)^{-1/2}$. For initial data $\delta(t_*)=\delta_*$ and $\dot\delta(t_*)=v_*$, the equivalent answer is $\delta_*\cosh[\omega_J(t-t_*)]+(v_*/\omega_J)\sinh[\omega_J(t-t_*)]$. This solves the stated perturbation model; a globally static dust-only [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) would require additional background support.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $a\propto t^{2/3}$ and $H=2/(3t)$. The [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\rho_m=\frac{3H^2}{8\pi G}=\frac1{6\pi Gt^2},
\qquad
\ddot\delta+\frac4{3t}\dot\delta-\frac2{3t^2}\delta=0.
$$

This is an [Euler differential equation](../../../differential-equation.md#cauchy-euler-equation). Substitution of $\delta=t^p$ gives $p(p-1)+(4/3)p-2/3=0$, namely $(p-2/3)(p+1)=0$. The [Einstein-de Sitter density-growth modes](../../../linear-cosmological-density-perturbation.md#einstein-de-sitter-density-growth-modes) are therefore

$$
\boxed{\delta(t)=C_+t^{2/3}+C_-t^{-1}
=A_+a(t)+A_-a(t)^{-3/2}.}
$$

The [linear growth factor](../../../linear-cosmological-density-perturbation.md#linear-growth-factor) for the growing mode is proportional to $a$, rather than an exponential in cosmic time. These expressions apply while the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) is small enough for [linear cosmological density perturbations](../../../linear-cosmological-density-perturbation.md).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

After the decay products dominate the background, [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) gives $\rho_r\propto a^{-4}$. Neglecting curvature and vacuum terms, the [Friedmann equation](../../../cosmology.md#friedmann-equations) implies $\dot a/a=C/a^2$, so $a\propto(t-t_B)^{1/2}$ and

$$
\boxed{H=\frac1{2(t-t_B)}.}
$$

The displayed $1/(2t)$ form uses a cosmic-time origin with $t_B=0$. After a late transition the extrapolated radiation-era origin need not be the original Big Bang; this time shift does not change the growth law.

For the remaining pressureless matter, neglect its self-gravity to leading order in $\rho_m/\rho_r$. Its [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) obeys $\ddot\delta+(t-t_B)^{-1}\dot\delta=0$. Using the conserved [expansion-weighted derivative of a passive density perturbation](../../../linear-cosmological-density-perturbation.md#expansion-weighted-derivative-of-a-passive-density-perturbation) gives

$$
\boxed{\delta(t)=C_1+C_2\log\!\left(\frac{t-t_B}{t_*-t_B}\right)
=A+B\log a(t).}
$$

Thus [logarithmic growth of matter perturbations during radiation domination](../../../linear-cosmological-density-perturbation.md#logarithmic-growth-of-matter-perturbations-during-radiation-domination) replaces the static exponential growth and the matter-era $t^{2/3}$ growth. The expansion persists while its dominant radiation component supplies little sustained clustering in this pressureless test-component approximation. The residual matter can eventually become important again because $\rho_m/\rho_r\propto a$; the approximation is for the radiation-dominated interval. The equation is not a pressureless growth equation for the relativistic decay products themselves, whose pressure and, when a fluid description applies, [radiation acoustic oscillations](../../../linear-cosmological-perturbation-theory.md#subhorizon-radiation-acoustic-oscillations) must be retained.

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a statistically homogeneous matter distribution, the [cosmological two-point correlation function](../../../large-scale-structure-of-the-universe.md#correlation-function-astronomy) of the mean-zero [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) $\delta=(\rho-\bar\rho)/\bar\rho$ is

$$
\boxed{\xi(r)=\langle\delta(\mathbf x)\delta(\mathbf x+\mathbf r)\rangle,
\qquad r=|\mathbf r|.}
$$

[Spatial homogeneity](../../../cosmology.md#spatial-homogeneity) removes dependence on $\mathbf x$, and [isotropy](../../../continuum-mechanics.md#isotropy) reduces the separation argument to its magnitude. For discrete [galaxies](../../../galaxy.md), the [galaxy two-point correlation function](../../../large-scale-structure-of-the-universe.md#galaxy-two-point-correlation-function) equivalently specifies the excess pair probability at distinct positions:

$$
dP_{12}=\bar n^2[1+\xi(r)]\,dV_1dV_2.
$$

Consequently the mean density of other [galaxies](../../../galaxy.md), conditioned on a [galaxy](../../../galaxy.md) at the origin, is $\bar n[1+\xi(r)]$. The self-pair at zero separation is excluded from this definition; its [Dirac delta](../../../distribution-theory.md#dirac-delta-function) contribution is the [galaxy power spectrum shot noise](../../../large-scale-structure-of-the-universe.md#galaxy-power-spectrum-shot-noise) of the unsmoothed number-density field.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

With the specified [Fourier transform](../../../analysis.md#fourier-transform) convention, the inverse is $\delta(\mathbf x)=\int d^3k\,\delta_{\mathbf k}e^{-i\mathbf k\cdot\mathbf x}/(2\pi)^3$. Inserting both inverse transforms into the [cosmological two-point correlation function](../../../large-scale-structure-of-the-universe.md#correlation-function-astronomy) and applying the given [Dirac delta](../../../distribution-theory.md#dirac-delta-function) covariance yields

$$
\begin{aligned}
\xi(\mathbf r)
&=\int\frac{d^3k\,d^3k'}{(2\pi)^6}
e^{-i\mathbf k\cdot\mathbf x-i\mathbf k'\cdot(\mathbf x+\mathbf r)}
\langle\delta_{\mathbf k}\delta_{\mathbf k'}\rangle\\
&=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
\end{aligned}
$$

For an isotropic [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum), align the polar axis with $\mathbf r$. The angular integral is $2\pi\int_{-1}^1e^{ikr\mu}\,d\mu=4\pi\sin(kr)/(kr)$. Hence the [isotropic cosmological correlation-power-spectrum relation](../../../large-scale-structure-of-the-universe.md#isotropic-cosmological-correlation-power-spectrum-relation) is

$$
\boxed{\xi(r)=\frac1{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin(kr)}{kr}\,dk.}
$$

The angular kernel is the order-zero [Spherical Bessel function](../../../analysis.md#spherical-bessel-function) $j_0(kr)$. At $r=0$, replace it by its [limit](../../../calculus.md#limit-of-a-function) one, giving the unsmoothed [variance](../../../variance.md) when the integral converges. The argument assumes an ordinary integrable spectrum, or an explicitly specified [distributional Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-tempered-distribution) interpretation otherwise.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [galaxy-conditioned neighbour count](../../../large-scale-structure-of-the-universe.md#galaxy-conditioned-neighbour-count) is the integral of the conditional number density $\bar n[1+\xi(r)]$, rather than of $\bar n$ alone. For a [power law](../../../analysis.md#power-law) $\xi=(r_0/r)^\gamma$ with $\gamma<3$,

$$
N_{\rm gal}(<R)=4\pi\bar n\left[\frac{R^3}{3}
+\frac{r_0^\gamma R^{3-\gamma}}{3-\gamma}\right].
$$

With the specified $\gamma=2$, $R=10h^{-1}\,\mathrm{Mpc}$, $r_0=5h^{-1}\,\mathrm{Mpc}$ and $\bar n=0.01(h^{-1}\,\mathrm{Mpc})^{-3}$, the factors of $h$ cancel and

$$
\boxed{N_{\rm gal}(<R)=4\pi(0.01)\left(\frac{1000}{3}+250\right)
=\frac{70\pi}{3}\simeq73.30.}
$$

A uniformly chosen point in space is not conditioned to lie on a [galaxy](../../../galaxy.md). Its [expected value](../../../probability-theory.md#expected-value) is simply the mean number density times the volume:

$$
\boxed{N_{\rm random}(<R)=\frac{4\pi}{3}\bar nR^3
=\frac{40\pi}{3}\simeq41.89.}
$$

The difference $10\pi\simeq31.42$ is the clustering excess. The first count means other [galaxies](../../../galaxy.md); including the chosen central [galaxy](../../../galaxy.md) adds one. Although the assumed [galaxy two-point correlation function](../../../large-scale-structure-of-the-universe.md#galaxy-two-point-correlation-function) diverges at $r=0$, its contribution is integrable here because $r^2\xi(r)$ is constant.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Apply the [isotropic cosmological correlation-power-spectrum relation](../../../large-scale-structure-of-the-universe.md#isotropic-cosmological-correlation-power-spectrum-relation) and put $K=k_{\max}$, $q=Kr$. The [band-limited linear density correlation](../../../linear-cosmological-density-perturbation.md#band-limited-linear-density-correlation) is

$$
\xi(r)=\frac{A}{2\pi^2r}\int_0^K k^2\sin(kr)\,dk.
$$

Two [integrations by parts](../../../calculus.md#integration-by-parts) give the primitive $-k^2\cos(kr)/r+2k\sin(kr)/r^2+2\cos(kr)/r^3$. Evaluating both endpoints yields

$$
\boxed{\xi(r)=\frac{A}{2\pi^2r^4}
[-q^2\cos q+2q\sin q+2(\cos q-1)],\qquad r>0.}
$$

The apparent singularity at the origin is removable. Either the [Taylor series](../../../calculus.md#taylor-series) or the original integral gives

$$
\boxed{\xi(0)=\frac{AK^4}{8\pi^2}.}
$$

In fact $\xi(r)=\xi(0)[1-q^2/9+q^4/240+O(q^6)]$. The sharp spectral cutoff produces oscillations and negative correlations at some nonzero separations, even though the [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) is everywhere nonnegative. A [covariance function](../../../stochastic-process.md#covariance-function) need not be pointwise nonnegative; its required positivity is that of the covariance quadratic form.

<a id="3/iv/image-an-abrupt-cutoff-in-a-nonnegative-density-power-spectrum-produces-an-oscillating-correlation-function"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41-cutoff-correlation.png)

**[Figure 1](#3/iv/image-an-abrupt-cutoff-in-a-nonnegative-density-power-spectrum-produces-an-oscillating-correlation-function). An abrupt cutoff in a nonnegative density power spectrum produces an oscillating correlation function**.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Consider a logarithmic band of [wavenumbers](../../../wave-equation.md#wavenumber) around $k\sim R^{-1}$, where $R$ is a comoving scale. The [dimensionless cosmological power spectrum](../../../cosmic-inflation.md#dimensionless-cosmological-power-spectrum) of the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) is $\Delta_\delta^2(k)=k^3P_\delta(k)/(2\pi^2)$. For $P_\delta=Ak$ this scales as $k^4$, so the rms density amplitude in such a band scales as $R^{-2}$.

The [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives $-k^2\Phi_{\mathbf k}=4\pi Ga^2\bar\rho_m\delta_{\mathbf k}$, with $\Phi$ a dimensionful [peculiar gravitational potential](../../../linear-cosmological-density-perturbation.md#peculiar-gravitational-potential). Its spectrum and its [potential fluctuations per logarithmic wavenumber](../../../linear-cosmological-density-perturbation.md#potential-fluctuations-per-logarithmic-wavenumber) are therefore

$$
P_\Phi(k)=\frac{(4\pi Ga^2\bar\rho_m)^2A}{k^3},
\qquad
\boxed{\Delta_\Phi^2(k)=\frac{(4\pi Ga^2\bar\rho_m)^2A}{2\pi^2},}
$$

independent of $k$. Equivalently, $\Phi_R\sim G\bar\rho_m(aR)^2\delta_R$ is independent of $R$ because $\delta_R\propto R^{-2}$. This is the scale-local meaning of the [Harrison-Zeldovich spectrum](../../../linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum). An uncut spectrum has a divergent total potential [variance](../../../variance.md); equal amplitude per logarithmic band does not imply a finite unsmoothed [variance](../../../variance.md) over all scales. For wavelengths beyond the [Hubble radius](../../../cosmology.md#hubble-radius), the statement is formulated using the corresponding conserved primordial curvature mode and its adiabatic matter-era potential, rather than treating the subhorizon Poisson approximation as universally valid.

On angular scales larger than roughly a degree, the [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect) relates the last-scattering potential to the observed [Cosmic microwave background anisotropy](../../../cosmic-microwave-background-anisotropy.md): $\Delta T/T\simeq\Phi/(3c^2)$ for adiabatic modes in [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination). Thus the observed large-angle amplitude constrains $A$. Scale-invariant potential bands produce a [Sachs-Wolfe plateau](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-plateau), $\ell(\ell+1)C_\ell$ approximately constant, rather than constant $C_\ell$. Its amplitude and any tilt test the normalization and spectral shape. [Cosmic variance](../../../cosmic-microwave-background-anisotropy.md#cosmic-variance), [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect) and assumptions about adiabatic initial conditions limit this inference; the density spectrum's late-time transfer must also be included when comparing it with galaxy clustering.

## 4

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For approximately circular motion in a spherically dominated [Newtonian gravitational field](../../../classical-mechanics.md#newtonian-gravitational-field), $v_c^2(r)=GM(<r)/r$. If most gravitating mass followed the concentrated luminous [galaxies](../../../galaxy.md), then beyond their main light distribution the enclosed mass would nearly saturate, giving a declining Keplerian [galaxy rotation curve](../../../galaxy.md#galaxy-rotation-curve), $v_c\propto r^{-1/2}$.

Instead, extended [galaxy rotation curves](../../../galaxy.md#galaxy-rotation-curve) commonly remain roughly flat. The [spherical mass profile for a flat rotation curve](../../../galaxy.md#spherical-mass-profile-for-a-flat-rotation-curve) then requires

$$
\boxed{M(<r)\simeq\frac{v_0^2r}{G},\qquad
\rho(r)\simeq\frac{v_0^2}{4\pi Gr^2}.}
$$

The inferred mass continues growing where the luminous contribution is small, so the [mass-to-light ratio](../../../galaxy.md#mass-to-light-ratio) increases outward. Under the assumed gravitational dynamics this is evidence for an extended [dark matter halo](../../../large-scale-structure-of-the-universe.md#dark-matter-halo). Measurements of neutral-gas motion can probe radii beyond the bright stellar disk. A realistic disk contribution must be computed using its flattened geometry; the spherical formula describes a halo-dominated region and does not turn every disk [rotation curve](../../../galaxy.md#galaxy-rotation-curve) into a spherical mass profile.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The three probes constrain the same deep gravitational potential by different observations. A large member-galaxy [velocity dispersion](../../../galaxy.md#velocity-dispersion) requires a large binding mass. Applying the [virial theorem](../../../classical-mechanics.md#virial-theorem), with a gravitational scale radius $R$ and approximately isotropic orbits, gives a [cluster velocity-dispersion mass estimate](../../../large-scale-structure-of-the-universe.md#cluster-velocity-dispersion-mass-estimate) of order $M\sim R\sigma_v^2/G$, with a profile-dependent numerical coefficient. The inferred [mass-to-light ratio](../../../galaxy.md#mass-to-light-ratio) is much larger than the stellar value. Membership, orbital anisotropy and equilibrium assumptions affect the precision.

The hot [intracluster medium](../../../large-scale-structure-of-the-universe.md#intracluster-medium) radiates through [thermal bremsstrahlung](../../../astrophysics.md#thermal-bremsstrahlung) and line emission. Its X-ray spectrum measures [temperature](../../../thermodynamics.md#temperature), while its surface brightness constrains gas density. Confining this gas requires a potential with characteristic $GM/R\sim k_BT/(\mu m_p)$. Combining resolved profiles through the [cluster hydrostatic mass estimator](../../../large-scale-structure-of-the-universe.md#cluster-hydrostatic-mass-estimator) gives the total mass, not just the gas mass. The detected gas contributes substantial baryonic mass but does not normally account for the full gravitating mass. Nonthermal pressure or a merging cluster can invalidate a purely thermal [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) estimate.

Finally, [gravitational lensing](../../../general-relativity.md#gravitational-lensing) measures mass through light deflection. [Strong gravitational lensing](../../../general-relativity.md#strong-gravitational-lensing) supplies multiple images and arcs; [weak gravitational lensing](../../../general-relativity.md#weak-gravitational-lensing) measures coherent background-image distortion over larger radii. The [lensing convergence](../../../general-relativity.md#lensing-convergence) is projected [surface mass density](../../../fluid-mechanics.md#projected-surface-mass-density) divided by the critical surface density, irrespective of whether the material emits light. [Cluster gravitational-lensing mass estimates](../../../large-scale-structure-of-the-universe.md#cluster-gravitational-lensing-mass-estimate) agree broadly with the high masses implied by galaxy motions and hot gas, while having different equilibrium assumptions. Together these observations support a dominant nonluminous component in [galaxy clusters](../../../large-scale-structure-of-the-universe.md#galaxy-cluster), after accounting for their stars and observed gas.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Use [conservation of energy](../../../physics.md#conservation-of-energy) for an isolated spherical perturbation of fixed mass $M$, with negligible initial random motion and no significant surface-pressure term. For a homologous density profile its [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) is $U=-\alpha GM^2/R$, with the same positive structure coefficient $\alpha$ at both stages; a uniform sphere has $\alpha=3/5$.

At [spherical-collapse turnaround](../../../large-scale-structure-of-the-universe.md#turnaround-of-spherical-collapse), coherent radial motion momentarily vanishes, so $E=U_{\max}=-\alpha GM^2/R_{\max}$. In the final virialized state, the [virial theorem](../../../classical-mechanics.md#virial-theorem) gives $2T_{\rm vir}+U_{\rm vir}=0$, hence $E=T_{\rm vir}+U_{\rm vir}=U_{\rm vir}/2$. Therefore

$$
-\frac{\alpha GM^2}{R_{\max}}
=-\frac{\alpha GM^2}{2R_{\rm vir}},
\qquad
\boxed{R_{\rm vir}=\frac12R_{\max}.}
$$

This is the [virial radius from turnaround energy](../../../large-scale-structure-of-the-universe.md#virial-radius-from-turnaround-energy) in the [spherical-collapse model](../../../large-scale-structure-of-the-universe.md#spherical-collapse-model). It is an idealized virial-radius estimate rather than the radius of the formal pressureless point collapse. If the profile coefficient changes, the same argument instead gives $R_{\rm vir}/R_{\max}=\alpha_{\rm vir}/(2\alpha_{\max})$. Significant energy loss, mass loss or boundary work also changes the result.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Let $\rho_g(r)$ be the gas density and $M(<r)$ the total gravitating mass. For a spherically symmetric gas in [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium), radial force balance is

$$
\frac{dP}{dr}=-\rho_g\frac{GM(<r)}{r^2}.
$$

Using the [ideal gas law](../../../thermodynamics.md#ideal-gas-law) $P=\rho_gk_BT/(\mu m_p)$, with constant [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) $\mu$, differentiate the product rather than setting $T$ constant:

$$
\frac{dP}{dr}=\frac{k_BT\rho_g}{\mu m_pr}
\left(\frac{d\log\rho_g}{d\log r}+\frac{d\log T}{d\log r}\right).
$$

Substitution and cancellation of $\rho_g$ give the [cluster hydrostatic mass estimator](../../../large-scale-structure-of-the-universe.md#cluster-hydrostatic-mass-estimator)

$$
\boxed{M(<r)=-\frac{k_BT(r)r}{\mu m_pG}
\left[\frac{d\log\rho_g}{d\log r}+\frac{d\log T}{d\log r}\right].}
$$

Here $k_B$ is the [Boltzmann constant](../../../thermodynamics.md#boltzmann-constant), denoted $K$ in the question. The prefactor has units of mass; a pressure decreasing outward makes the bracket negative and the inferred mass positive. For an isothermal gas with $\rho_g\propto r^{-\beta}$, this reduces to $M(<r)=\beta k_BTr/(\mu m_pG)$. The density in the logarithmic derivative is the gas density, not the total density. A varying $\mu$ or nonthermal pressure would require the corresponding extra terms.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Measure the cluster's baryonic mass, dominated by its [intracluster medium](../../../large-scale-structure-of-the-universe.md#intracluster-medium) with a smaller stellar contribution, and divide it by an independently inferred total mass. If this cluster baryon fraction $f_b$ is representative of the [cosmic baryon fraction](../../../cosmology.md#cosmic-baryon-fraction), then $f_b=\Omega_b/\Omega_m$. Thus the [cluster baryon-fraction estimate of matter density](../../../cosmology.md#cluster-baryon-fraction-estimate-of-matter-density) is

$$
\boxed{\Omega_m=\frac{\Omega_b}{f_b}.}
$$

[Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) constrains the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) and hence $\Omega_bh^2$ through primordial light-element abundances. A specified $h$ converts this to $\Omega_b$; the cluster mass and gas-mass estimates also have distance-dependent $h$ factors, which must be used consistently. This method estimates the total nonrelativistic matter density, including baryonic and [dark matter](../../../cosmology.md#dark-matter). It does not add radiation or vacuum energy to that inferred $\Omega_m$; in a matter-dominated interpretation the question's $\Omega$ is this matter parameter.

[Primordial deuterium as a baryon-density indicator](../../../cosmology.md#primordial-deuterium-as-a-baryon-density-indicator) works because increasing baryon density makes the destruction of [deuterium](../../../chemistry.md#deuterium) into heavier nuclei more efficient during [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis). Smaller inferred primordial D/H therefore implies larger $\Omega_b$, with the other nucleosynthesis assumptions fixed. **For a fixed measured cluster baryon fraction, a smaller primordial deuterium abundance raises the inferred matter density.** A low abundance caused instead by stellar processing is not a lower primordial abundance; depletion, gas ejection and the representativeness of clusters must also be assessed before identifying the cluster fraction with the cosmic one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
