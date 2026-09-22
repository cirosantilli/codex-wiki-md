# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_310.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [i](#1/b/iv/i)
        - [Solution](#1/b/iv/i/solution)
      - [ii](#1/b/iv/ii)
        - [Solution](#1/b/iv/ii/solution)
      - [iii](#1/b/iv/iii)
        - [Solution](#1/b/iv/iii/solution)
      - [iv](#1/b/iv/iv)
        - [Solution](#1/b/iv/iv/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Use units $c=1$ throughout. Set $\chi=|\mathbf x|$, so the spatial Euclidean metric is $d\mathbf x^2=d\chi^2+\chi^2d\Omega^2$. On either hemisphere of the embedded [three-sphere](../../../geometry-and-topology.md#three-sphere), the constraint gives $u^2=R^2-\chi^2$ and hence

$$
du=-\frac\chi u\,d\chi,\qquad
d\ell^2=\frac{d\chi^2}{1-\chi^2/R^2}+\chi^2d\Omega^2.
$$

Introduce the dimensionless [comoving coordinate](../../../cosmology.md#comoving-coordinate) $r=\chi/R$. Then

$$
\boxed{ds^2=-dt^2+a(t)^2\left\{\frac{dr^2}{1-Kr^2}+r^2d\Omega^2\right\},\qquad a(t)=Rb(t),\quad K=+1.}
$$

This is the positively curved [Friedmann-Lemaître-Robertson-Walker metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), with $a(t)$ the physical curvature radius. An equally valid convention retains $r=\chi$, takes $a=b$, and sets $K=R^{-2}$; only the coordinate normalization differs. The chart with $r\leq1$ describes a hemisphere, not the entire closed slice. Writing $r=\sin\psi$ gives $d\ell^2=R^2(d\psi^2+\sin^2\psi\,d\Omega^2)$, with $0\leq\psi\leq\pi$, displaying the full [spherical spatial slices of a closed FLRW universe](../../../cosmology.md#spherical-spatial-slices-of-a-closed-flrw-universe).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For [separately conserved cosmological fluids](../../../cosmology.md#separately-conserved-cosmological-fluids), the prerequisite is absence of energy or momentum exchange between components. Each matter action then gives its own local conservation equation $\nabla_\mu T_i^{\mu\nu}=0$. In the homogeneous [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity), its time component is

$$
\boxed{\dot\rho_i+3H(\rho_i+P_i)=0,\qquad H=\dot a/a.}
$$

This is the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation). Equivalently, a physical volume $V\propto a^3$ following the fluid satisfies $d(\rho_iV)=-P_i\,dV$.

The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) instead have the single shared metric on its left and $\sum_iT_i^{\mu\nu}$ on its right. The [Friedmann equation](../../../cosmology.md#friedmann-equations) and [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) therefore involve total density and total pressure; the same geometry cannot be sourced separately by each component's density alone.

The PDF's separate-conservation statement needs this noninteraction qualification. In an interacting system,

$$
\dot\rho_i+3H(\rho_i+P_i)=Q_i,\qquad\boxed{\sum_iQ_i=0,}
$$

where $Q_i$ is the energy-transfer rate into component $i$. Total conservation remains true, but the source-free equation does not hold individually during processes such as annihilation or particle decay.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a constant [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) $w=P/\rho$, the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) integrates to $\rho\propto a^{-3(1+w)}$. Comparing the given powers yields

$$
\boxed{w_s=-\frac13,\qquad w_w=-\frac23,\qquad P_s=-\frac{\rho_s}{3},\quad P_w=-\frac{2\rho_w}{3}.}
$$

This [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) describes a [cosmic string network](../../../cosmology.md#cosmic-string-network) and a [cosmological domain wall network](../../../cosmology.md#cosmological-domain-wall-network). An intuitive check is that the energy in a fixed comoving cell grows in proportion to the total string length, $a$, or total wall area, $a^2$, while the physical cell volume grows as $a^3$. Thus the densities scale as $a^{-2}$ and $a^{-1}$ respectively. These effective equations of state use the noninteracting, statistically isotropic network assumptions of the problem.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Choose a reference epoch with $H_0=\dot a(t_0)/a_0\ne0$ and let $x=a/a_0$. Define the [critical density](../../../cosmology.md#critical-density) and each [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) by

$$
\rho_{\mathrm{crit},0}=\frac{3H_0^2}{8\pi G},\qquad
\boxed{\Omega_{i,0}=\frac{\rho_{i,0}}{\rho_{\mathrm{crit},0}},\qquad
\Omega_{K,0}=-\frac{K}{a_0^2H_0^2}.}
$$

For a closed universe $\Omega_{K,0}<0$. Take the dark-energy component to be a [cosmological constant](../../../cosmology.md#cosmological-constant), as indicated by its $\Lambda$ label. The [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) gives

$$
\rho_r=\rho_{r,0}x^{-4},\quad\rho_m=\rho_{m,0}x^{-3},\quad
\rho_s=\rho_{s,0}x^{-2},\quad\rho_w=\rho_{w,0}x^{-1},\quad\rho_\Lambda=\rho_{\Lambda,0}.
$$

Substitution into the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
\boxed{\frac{H^2}{H_0^2}=\Omega_{r,0}x^{-4}+\Omega_{m,0}x^{-3}+(\Omega_{s,0}+\Omega_{K,0})x^{-2}+\Omega_{w,0}x^{-1}+\Omega_{\Lambda,0}.}
$$

At the reference epoch, $\Omega_{r,0}+\Omega_{m,0}+\Omega_{s,0}+\Omega_{w,0}+\Omega_{\Lambda,0}+\Omega_{K,0}=1$. The [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) is

$$
\boxed{\frac{\ddot a}{aH_0^2}=-\Omega_{r,0}x^{-4}-\frac12\Omega_{m,0}x^{-3}+\frac12\Omega_{w,0}x^{-1}+\Omega_{\Lambda,0}.}
$$

Strings have $\rho_s+3P_s=0$ and make no direct acceleration contribution, although they affect the Friedmann constraint. The normalized density parameters are undefined at a static epoch, where $H_0=0$; the static solution must therefore be described directly with dimensional densities.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

For a single positive-density component, staticity requires $\rho+3P=0$ from the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation). Among the listed components, only the [cosmic string network](../../../cosmology.md#cosmic-string-network) has $w=-1/3$. Put $a(t)=a_E>0$ and use the [Friedmann equation](../../../cosmology.md#friedmann-equations) to obtain

$$
\boxed{a(t)=a_E=\sqrt{\frac{3K}{8\pi G\rho_E}},\qquad
\rho_E=\frac{3K}{8\pi Ga_E^2},\qquad P_E=-\frac{\rho_E}{3}.}
$$

All other components are absent. This is the [static closed cosmic-string universe](../../../cosmology.md#static-closed-cosmic-string-universe).

There is a normalization condition hidden in this expression. String conservation fixes $C_s=\rho_sa^2$, and a static solution exists only when

$$
\boxed{C_s=\frac{3K}{8\pi G}.}
$$

Once this condition is imposed, every positive radius $a_E$ is a static solution, with its density determined as above. One cannot independently prescribe an arbitrary string normalization and then choose a radius to compensate: both the string density term and curvature term scale as $a^{-2}$.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/i">i</h5>

↑ **Parent:** [Iv](#1/b/iv)

<h6 id="1/b/iv/i/solution">Solution</h6>

↑ **Parent:** [I](#1/b/iv/i)

First perturb the radius consistently with the conserved string normalization. If $a_E\mapsto a_E(1+\epsilon)$ while $C_s=\rho_sa^2$ stays at its static value, the density becomes

$$
\rho_E\mapsto\rho_E(1+\epsilon)^{-2}=\rho_E(1-2\epsilon+O(\epsilon^2)).
$$

The [Friedmann equation](../../../cosmology.md#friedmann-equations) still has an exact cancellation between the string and curvature terms, and the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) still vanishes. Thus

$$
\boxed{\text{A radius displacement at fixed }C_s\text{ moves to another static solution.}}
$$

The [homogeneous stability of a static cosmic-string universe](../../../cosmology.md#homogeneous-stability-of-a-static-cosmic-string-universe) is neutral in this restricted sense: there is no restoring force and no exponentially growing displacement. Holding the density fixed while changing the radius would instead change $C_s$ and would not be this pure displacement perturbation.

<h5 id="1/b/iv/ii">ii</h5>

↑ **Parent:** [Iv](#1/b/iv)

<h6 id="1/b/iv/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#1/b/iv/ii)

The distinction between the evolution equation and the constraint is essential. For strings alone, the exact equations reduce to

$$
\ddot a=0,\qquad\dot a^2=\frac{8\pi G}{3}C_s-K.
$$

Linearizing the acceleration equation gives $\delta a=A+Bt$. At the exactly tuned static $C_s$, however, the full [Friedmann equation](../../../cosmology.md#friedmann-equations) requires $\dot a^2=0$, so $B=0$ for an admissible exact perturbation.

A small nonzero velocity $v$ can be admissible if its initial density also changes:

$$
C_s=C_E+\frac{3v^2}{8\pi G},\qquad
\delta\rho(t_E)=\frac{3v^2}{8\pi Ga_E^2},\qquad
\boxed{a(t)=a_E+v(t-t_E).}
$$

Arbitrarily small $v$ and the corresponding second-order density change therefore produce a secular departure. There is no [Lyapunov stability](../../../dynamical-systems.md#lyapunov-stability) against all nearby constrained initial data for the [static closed cosmic-string universe](../../../cosmology.md#static-closed-cosmic-string-universe). Neutral radius shifts at fixed normalization and drift when the normalization changes are different perturbation classes.

<h5 id="1/b/iv/iii">iii</h5>

↑ **Parent:** [Iv](#1/b/iv)

<h6 id="1/b/iv/iii/solution">Solution</h6>

↑ **Parent:** [Iii](#1/b/iv/iii)

Increase the density at the initial radius by a small fraction $\epsilon>0$, maintaining the string equation of state. Then $C_s=C_E(1+\epsilon)$ and the [Friedmann equation](../../../cosmology.md#friedmann-equations) fixes

$$
\dot a^2=K\epsilon.
$$

Because $\ddot a=0$, the exact expanding and contracting branches are

$$
\boxed{a(t)=a_E\pm\sqrt{K\epsilon}\,(t-t_E),\qquad
\rho_s(t)=\rho_E(1+\epsilon)\left(\frac{a_E}{a(t)}\right)^2.}
$$

The expanding branch grows indefinitely; the contracting branch reaches zero scale factor after $a_E/\sqrt{K\epsilon}$. Thus a positive density-normalization perturbation destroys staticity. The departure speed is proportional to $\sqrt\epsilon$, reflecting the fact that the Friedmann constraint is quadratic in the velocity at the static point. This is another aspect of [homogeneous stability of a static cosmic-string universe](../../../cosmology.md#homogeneous-stability-of-a-static-cosmic-string-universe).

<h5 id="1/b/iv/iv">iv</h5>

↑ **Parent:** [Iv](#1/b/iv)

<h6 id="1/b/iv/iv/solution">Solution</h6>

↑ **Parent:** [Iv](#1/b/iv/iv)

If the initial density is decreased by $\epsilon<0$ at the same radius, the string-only [Friedmann equation](../../../cosmology.md#friedmann-equations) would require

$$
\boxed{\dot a^2=K\epsilon<0,}
$$

which has no real solution. It is not an allowed initial perturbation of a closed string-only universe at fixed curvature normalization. In particular, it should not be interpreted as an oscillating or automatically recollapsing solution.

Likewise, increasing the density while keeping both $a$ and $\dot a=0$ fixed violates the constraint; the admissible velocity is the one obtained above. The [homogeneous stability of a static cosmic-string universe](../../../cosmology.md#homogeneous-stability-of-a-static-cosmic-string-universe) must always be assessed using both the acceleration equation and the Friedmann constraint. Allowing extra components or changing the spatial curvature would define a different perturbation problem.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Interpret $P(k)$ in the variance integral as the unsmoothed [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) of $\delta$. A linear smoothing window gives $P_R(k)=P(k)|\widetilde W(kR)|^2$ for the smoothed field; the PDF's description of $P(k)$ as already belonging to $\delta_R$ would otherwise count the window twice.

For a [scale-free matter power spectrum](../../../large-scale-structure-of-the-universe.md#scale-free-matter-power-spectrum) $P(k)=Ak^{n_{\mathrm{eff}}}$, substitute $q=kR$ to obtain

$$
\sigma_R^2=\frac{A}{2\pi^2}R^{-(n_{\mathrm{eff}}+3)}
\int_0^\infty q^{n_{\mathrm{eff}}+2}|\widetilde W(q)|^2\,dq.
$$

Whenever the dimensionless integral is finite and nonzero, this proves the [scale-free smoothed density variance](../../../large-scale-structure-of-the-universe.md#scale-free-smoothed-density-variance)

$$
\boxed{\sigma_R\propto R^{-(n_{\mathrm{eff}}+3)/2}.}
$$

The printed condition $n_{\mathrm{eff}}<3$ is insufficient by itself. For a normalized window with $\widetilde W(0)=1$, infrared convergence requires $n_{\mathrm{eff}}>-3$. Ultraviolet convergence depends on the filter: a [spherical top-hat window function](../../../linear-cosmological-density-perturbation.md#spherical-top-hat-window-function) requires $n_{\mathrm{eff}}<1$, a Gaussian filter suppresses every ultraviolet power, and a [sharp-k smoothing filter](../../../large-scale-structure-of-the-universe.md#sharp-k-smoothing-filter) has finite Fourier support. In particular, the monotone relation $R\to\infty\Rightarrow S=\sigma_R^2\to0$ requires $n_{\mathrm{eff}}>-3$ in the scale-free model.

At a single variance $S_*$, the [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) has $\delta_{S_*}\sim N(0,S_*)$. Thus its endpoint tail is

$$
\boxed{\mathbb P(\delta_{S_*}\geq\delta_c)=\int_{\delta_c}^{\infty}\frac{e^{-z^2/(2S_*)}}{\sqrt{2\pi S_*}}\,dz
=\frac12\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_*}}\right).}
$$

Here $\operatorname{erfc}$ is the complementary [error function](../../../calculus.md#error-function).

For the crossing probability, the key assumption is independent, symmetric increments as the smoothing scale changes. A [sharp-k smoothing filter](../../../large-scale-structure-of-the-universe.md#sharp-k-smoothing-filter), $\widetilde W(kR)=\mathbf1_{k<1/R}$, supplies this property: decreasing $R$ adds independent Fourier shells of the underlying Gaussian field. Parameterizing their accumulated variance by $S$ gives a [Brownian motion](../../../brownian-motion.md) with covariance $\min(S,S')$. An arbitrary real-space window gives correlated increments and does not justify this argument.

Reflect a trajectory after its first hit of $\delta_c$. The [Strong Markov property](../../../markov-process.md#strong-markov-property) and symmetric future increments preserve its probability, and reflection maps an endpoint below the barrier to one above it. Every endpoint above the barrier has already crossed; the reflected paths give an equally probable set that crossed but ended below. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) therefore yields the [excursion-set description of halo formation](../../../large-scale-structure-of-the-universe.md#excursion-set-description-of-halo-formation):

$$
\boxed{\mathcal P(S_*)=\mathbb P\!\left(\sup_{0\leq S\leq S_*}\delta_S\geq\delta_c\right)
=\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_*}}\right).}
$$

Its derivative is the [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) density

$$
f(S)=\frac{\delta_c}{\sqrt{2\pi}S^{3/2}}e^{-\delta_c^2/(2S)}.
$$

The factor of two resolves trajectories that crossed a larger-scale barrier but finish below it on the chosen smaller scale.

Define the [halo peak height](../../../large-scale-structure-of-the-universe.md#halo-peak-height) $\nu=\delta_c/\sigma_R$. The cumulative probability $\mathcal P(>M)$ is a dimensionless mass fraction. With $V_M=M/\bar\rho$, its conversion to halo number density gives

$$
\frac{d\bar n_h}{dM}=-\frac{\bar\rho}{M}\frac{d\mathcal P}{dM},\qquad
\frac{d\mathcal P}{dM}=\sqrt{\frac2\pi}\,\frac{\nu}{\sigma_R}e^{-\nu^2/2}\frac{d\sigma_R}{dM}.
$$

Consequently the [Press-Schechter halo mass function](../../../large-scale-structure-of-the-universe.md#press-schechter-halo-mass-function) is

$$
\boxed{\frac{d\bar n_h}{dM}=-\sqrt{\frac2\pi}\frac{\bar\rho}{M\sigma_R}\frac{d\sigma_R}{dM}\,\nu e^{-\nu^2/2},\qquad\nu=\frac{\delta_c}{\sigma_R}.}
$$

It is positive when $\sigma_R$ decreases with mass. A chosen mass-radius convention $M\propto R^3$ gives $d\log\sigma_R/d\log M=-(n_{\mathrm{eff}}+3)/6$. For a sharp Fourier filter that mass assignment needs a convention, since its real-space kernel is not a localized top-hat volume.

For [warm dark matter](../../../cosmology.md#warm-dark-matter), the cutoff introduces a new length and invalidates the pure power-law variance scaling near that length. With the same sharp-k filter and $n_{\mathrm{eff}}>-3$, the variance is exactly

$$
\boxed{S(R)=\frac{A}{2\pi^2(n_{\mathrm{eff}}+3)}
\min(R^{-1},k_{\mathrm{WDM}})^{n_{\mathrm{eff}}+3},\qquad
S_{\max}=\frac{A k_{\mathrm{WDM}}^{n_{\mathrm{eff}}+3}}{2\pi^2(n_{\mathrm{eff}}+3)}.}
$$

The Brownian walk runs only up to $S_{\max}$ and then stops. The cutoff does not destroy independence of the Fourier shells that are still present. Thus the first-crossing density and derivative mass-function formula remain valid on the invertible part of $S(M)$, using the actual cutoff variance. For $R<k_{\mathrm{WDM}}^{-1}$, $d\sigma_R/dM=0$ and this idealized sharp-filter model has no new crossings or new low-mass haloes. Its total collapsed fraction is

$$
\boxed{\mathcal P_{\mathrm{collapsed}}=\operatorname{erfc}\!\left(\frac{\delta_c}{\sqrt{2S_{\max}}}\right)<1.}
$$

This is [halo first crossing with a finite variance cutoff](../../../large-scale-structure-of-the-universe.md#halo-first-crossing-with-a-finite-variance-cutoff): some trajectories never cross, so one must not force the collapsed fraction to one. The uncut power-law abundance cannot be extrapolated to small masses. For other windows, a variance plateau still occurs but the Markov/reflection derivation is not exact; the same mass function is then a modelling approximation, rather than a result established by this calculation.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $V$ be the physical volume of a region with fixed comoving coordinates, so $V\propto a^3$, and write $U=\rho V$. The [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) is $dU=T\,dS-P\,dV+\mu\,dN$. Use [extensive quantities](../../../thermodynamics.md#extensive-quantity): under replication, $U(\lambda S,\lambda V,\lambda N)=\lambda U(S,V,N)$. The [Euler theorem for homogeneous functions](../../../real-analysis.md#euler-theorem-for-homogeneous-functions) gives

$$
U=TS-PV+\mu N.
$$

Setting $\mu=0$ yields

$$
\boxed{S=\frac{U+PV}{T}=\frac{\rho+P}{T}V.}
$$

This is the entropy form of the [Gibbs-Duhem equation](../../../thermodynamics.md#gibbs-duhem-equation); it fixes the normalization by extensivity, rather than adding an arbitrary volume-independent entropy constant.

For equilibrium expansion of the same region, the first law and the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) imply

$$
T\dot S=\dot U+P\dot V=V\dot\rho+(\rho+P)\dot V=0.
$$

Therefore $\boxed{\dot S=0}$, establishing [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) for adiabatic equilibrium evolution. Here “comoving volume” means a patch moving with the cosmological fluid; its physical volume $V$ changes. The corresponding coordinate volume is constant. The local TeX's $\dot V/P$ in the continuity-equation hint is a transcription error: the PDF correctly has $\dot V/V$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a relativistic equilibrium species with temperature $T_i$, the entropy density is $s_i=(\rho_i+P_i)/T_i=4\rho_i/(3T_i)$. In units $k_B=\hbar=c=1$, bosons have $\rho_i=\pi^2g_iT_i^4/30$, while fermions have $7/8$ times this expression. Relative to a reference bath temperature $T$, define the [effective number of relativistic degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-degrees-of-freedom) for entropy by

$$
\boxed{g_{*s}=\sum_{\mathrm{bosons}}g_i\left(\frac{T_i}{T}\right)^3
+\frac78\sum_{\mathrm{fermions}}g_i\left(\frac{T_i}{T}\right)^3,\qquad
s=\frac{2\pi^2}{45}g_{*s}T^3.}
$$

The sums here concern relativistic species, or their effective entropy contributions. Since a physical comoving patch has volume proportional to $a^3$, [cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) gives

$$
\boxed{g_{*s}a^3T^3=\text{constant}}
$$

for an isolated adiabatic bath. After [thermal decoupling in cosmology](../../../cosmology.md#thermal-decoupling-in-cosmology), one must apply this law separately to sectors that no longer exchange entropy.

Before [electron-positron annihilation in cosmology](../../../cosmology.md#electron-positron-annihilation-in-cosmology), the electromagnetic bath contains two photon polarizations and four electron/positron spin states. After [neutrino decoupling](../../../cosmology.md#neutrino-decoupling), its entropy degrees of freedom are initially

$$
g_{*s,\mathrm{before}}=2+\frac78(4)=\frac{11}{2},
$$

and after annihilation only the two photon polarizations remain. Electromagnetic entropy conservation therefore gives

$$
2(aT_\gamma)_{\mathrm{after}}^3=\frac{11}{2}(aT_\gamma)_{\mathrm{before}}^3.
$$

The decoupled [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) receives none of this entropy; its distribution temperature obeys $aT_\nu=\text{constant}$, and $T_\nu=T_\gamma$ before annihilation. Thus

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac4{11}\right)^{1/3}.}
$$

This is the [temperature of a decoupled relativistic relic](../../../cosmology.md#temperature-of-a-decoupled-relativistic-relic) in the instantaneous-decoupling approximation. The ratio remains the same afterwards in the absence of additional photon heating. At late times $T_\nu$ denotes the redshifted relic distribution temperature even when neutrino masses become relevant; it need not be a kinetic-equilibrium temperature.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Before decay, the nonrelativistic $\chi$ density redshifts as $a^{-3}$, while the photon density redshifts as $a^{-4}$. Therefore their ratio grows as $a$. Let a minus sign denote the instant just before decay and define

$$
r_d=\frac{\rho_\chi(t_d^-)}{\rho_\gamma(t_d^-)}
=\frac{a_d}{a_{\mathrm{ref}}}\frac{\rho_\chi(t_{\mathrm{ref}})}{\rho_\gamma(t_{\mathrm{ref}})}.
$$

Using the assumed [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) law $a\propto t^{1/2}$ gives $r_d=(t_d/t_{\mathrm{ref}})^{1/2}\rho_\chi(t_{\mathrm{ref}})/\rho_\gamma(t_{\mathrm{ref}})$.

Across an instantaneous decay the [scale factor](../../../cosmology.md#scale-factor-cosmology) does not change. Energy conservation and complete thermalization into a zero-chemical-potential photon bath give

$$
\rho_\gamma(t_d^+)=\rho_\gamma(t_d^-)+\rho_\chi(t_d^-)=\rho_\gamma(t_d^-)(1+r_d).
$$

Since [blackbody radiation](../../../statistical-physics.md#black-body-radiation) has $\rho_\gamma\propto T_\gamma^4$, [instantaneous photon heating by a decaying relic](../../../cosmology.md#instantaneous-photon-heating-by-a-decaying-relic) gives

$$
\boxed{\frac{T_\gamma^+}{T_\gamma^-}=(1+r_d)^{1/4}.}
$$

The already decoupled [Cosmic neutrino background](../../../cosmology.md#cosmic-neutrino-background) is not heated. Dividing its unchanged temperature by the new photon temperature therefore yields

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac4{11}\right)^{1/3}
\left[1+\left(\frac{t_d}{t_{\mathrm{ref}}}\right)^{1/2}
\frac{\rho_\chi(t_{\mathrm{ref}})}{\rho_\gamma(t_{\mathrm{ref}})}\right]^{-1/4}.}
$$

The relation written with $a_d/a_{\mathrm{ref}}$ is independent of the expansion approximation. Replacing it by the time ratio uses the radiation-dominated background assumed in the question; an appreciable matter contribution would require solving for that background instead. This photon entropy injection is not adiabatic, so the pre-decay photon entropy need not be conserved across the decay.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The [photon number density](../../../statistical-physics.md#photon-number-density) in a thermal zero-chemical-potential bath scales as $T_\gamma^3$. The heating factor from the previous calculation therefore increases photon number at fixed physical volume by $(1+r_d)^{3/4}$. The decay is nonbaryonic and preserves baryon number, giving [baryon-to-photon dilution by entropy injection](../../../cosmology.md#baryon-to-photon-dilution-by-entropy-injection):

$$
\boxed{\frac{\eta^+}{\eta^-}=(1+r_d)^{-3/4},\qquad\eta=\frac{n_b}{n_\gamma}.}
$$

If the decay occurs after the light-element abundances have frozen out in [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis) but before the epoch probed by the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background), abundance measurements infer the earlier $\eta_{\mathrm{BBN}}$, whereas the CMB measures the later $\eta_{\mathrm{CMB}}$. In this simple scenario,

$$
\boxed{\frac{\eta_{\mathrm{BBN}}}{\eta_{\mathrm{CMB}}}=(1+r_d)^{3/4}>1.}
$$

A significant discrepancy in this direction could indicate photon entropy injection by $\chi$. Several light-element abundances help distinguish a changed baryon density from a changed expansion history. If decay occurs during nucleosynthesis, the inference instead requires time-dependent $\eta$ and a modified expansion history; the before/after comparison cannot automatically be applied to every decay time allowed in the question.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In [conformal time](../../../cosmology.md#conformal-time), $\sqrt{-g}=a^4$ and $g^{\mu\nu}=a^{-2}\operatorname{diag}(-1,1,1,1)$. The [inflaton action in an expanding universe](../../../cosmic-inflation.md#inflaton-action-in-an-expanding-universe) becomes

$$
S=\int d\tau\,d^3x\left\{\frac{a^2}{2}(\phi')^2-\frac{a^2}{2}(\nabla\phi)^2-a^4V(\phi)\right\}.
$$

Vary $\phi$ with compact support, integrate the derivative terms by parts, and discard the boundary term. The [Euler-Lagrange field equation](../../../quantum-field-theory.md#euler-lagrange-field-equation) is

$$
(a^2\phi')'-a^2\nabla^2\phi+a^4V_{,\phi}=0.
$$

Dividing by $a^2$ proves

$$
\boxed{\phi''+2\frac{a'}a\phi'-\nabla^2\phi+a^2V_{,\phi}=0.}
$$

The factor two is the conformal-time form of [Hubble friction](../../../cosmology.md#hubble-friction). Using $d\tau=dt/a$ converts it to the usual [inflaton equation of motion](../../../cosmic-inflation.md#inflaton-equation-of-motion) $\ddot\phi+3H\dot\phi-a^{-2}\nabla^2\phi+V_{,\phi}=0$, providing a sign and normalization check.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Subtract the homogeneous background equation and linearize the [inflaton equation of motion](../../../cosmic-inflation.md#inflaton-equation-of-motion). The field perturbation satisfies

$$
\delta\phi''+2\frac{a'}a\delta\phi'-\nabla^2\delta\phi+a^2V_{,\phi\phi}(\bar\phi)\delta\phi=0.
$$

With $f=a\delta\phi$, direct differentiation cancels the first-derivative term and gives

$$
f''-\nabla^2f+\left(a^2V_{,\phi\phi}-\frac{a''}a\right)f=0.
$$

The [conformal-time quadratic action for an inflaton perturbation](../../../cosmic-inflation.md#conformal-time-quadratic-action-for-an-inflaton-perturbation), after a boundary term is discarded, is

$$
S^{(2)}=\frac12\int d\tau\,d^3x\left\{(f')^2-(\nabla f)^2+\left(\frac{a''}a-a^2V_{,\phi\phi}\right)f^2\right\}.
$$

For the specified [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) background, $a''/a=2/\tau^2=2a^2H^2$. The light-field approximation $|V_{,\phi\phi}|\ll2H^2$ therefore permits dropping the mass term. Taking a spatial [Fourier transform](../../../analysis.md#fourier-transform) yields the [Canonically rescaled de Sitter scalar mode](../../../cosmic-inflation.md#canonically-rescaled-de-sitter-scalar-mode) equation

$$
\boxed{f_{\mathbf k}''+\left(k^2-\frac{a''}a\right)f_{\mathbf k}=0,\qquad\frac{a''}a=\frac2{\tau^2}.}
$$

Its kinetic term is canonical, with momentum $\pi_f=f'$. Each independent real Fourier component consequently has the canonical coordinate/momentum algebra of a [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator), with time-dependent squared frequency $\omega_k^2=k^2-a''/a$. This is why [canonical quantization of a real scalar field](../../../scalar-field-theory.md#canonical-quantization-of-a-real-scalar-field) proceeds by oscillator creation and annihilation operators. On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale) the squared frequency is negative: the system is then an inverted time-dependent oscillator, not a stationary oscillator with a positive frequency. The canonical commutation relations remain valid.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use the Fourier normalization of the PDF. The [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) obey

$$
\boxed{[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}^\dagger]=\delta^3(\mathbf k-\mathbf k'),\qquad
[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}]=[\widehat a_{\mathbf k}^\dagger,\widehat a_{\mathbf k'}^\dagger]=0.}
$$

There is no $(2\pi)^3$ in this commutator because the expansion uses $(2\pi)^{-3/2}$. The [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) satisfies $\widehat a_{\mathbf k}|0\rangle=0$. Write $u_k=f_k^*$ for the coefficient of the annihilation operator. Only the contraction $\langle0|\widehat a_{\mathbf k}\widehat a_{\mathbf k'}^\dagger|0\rangle=\delta^3(\mathbf k-\mathbf k')$ contributes, so

$$
\boxed{\langle0|\widehat{\delta\phi}(\tau,\mathbf x)\widehat{\delta\phi}(\tau,\mathbf x+\mathbf r)|0\rangle
=\int\frac{d^3k}{(2\pi)^3}\frac{|u_k(\tau)|^2}{a^2}e^{-i\mathbf k\cdot\mathbf r}.}
$$

The given mode has

$$
|u_k|^2=\frac1{2k}\left(1+\frac1{k^2\tau^2}\right).
$$

Since $a^{-2}=H^2\tau^2$, the [equal-time two-point function of a de Sitter scalar](../../../cosmic-inflation.md#equal-time-two-point-function-of-a-de-sitter-scalar) therefore has dimensional power spectrum

$$
P_{\delta\phi}(k,\tau)=\frac{H^2}{2k^3}(1+k^2\tau^2).
$$

Comparing with the dimensionless power convention in the hint gives

$$
\boxed{\Delta_{\delta\phi}^2(k,\tau)=\frac{k^3}{2\pi^2}P_{\delta\phi}(k,\tau)
=\left(\frac{H}{2\pi}\right)^2(1+k^2\tau^2).}
$$

Equivalently, angular integration expresses the correlation as $\int_0^\infty(dk/k)\,\Delta_{\delta\phi}^2\sin(kr)/(kr)$, where $r=|\mathbf r|$.

On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), $k\ll aH$ is $|k\tau|\ll1$, and

$$
\boxed{\Delta_{\delta\phi}^2\longrightarrow\left(\frac H{2\pi}\right)^2.}
$$

This [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum) gives equal variance per logarithmic wavenumber interval. It is exactly scale invariant in the massless constant-$H$ approximation here; slow evolution of $H$ and small field mass produce a small [spectral tilt](../../../cosmic-inflation.md#scalar-spectral-index). Such quantum [primordial perturbations](../../../cosmic-inflation.md#primordial-perturbation) supply the initial fluctuations that subsequently seed cosmological structure after conversion to curvature and density perturbations. The curvature conversion itself requires the metric perturbations excluded from this calculation.

The continuum correlation is understood with the usual infrared regulator, such as finite volume or finite inflationary duration. The strictly massless infinite-volume model has a logarithmic infrared divergence. Coincident products also require ultraviolet regularization or smearing; the finite mode spectrum is unaffected by these qualifications.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Under the stated linear field expansion, the [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) is a centered Gaussian state. By [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem), vacuum correlators reduce to pair contractions; an odd product has no complete pairing. In particular,

$$
\boxed{\langle0|\widehat{\delta\phi}(\tau,\mathbf x)\widehat{\delta\phi}(\tau,\mathbf y)\widehat{\delta\phi}(\tau,\mathbf z)|0\rangle=0.}
$$

This holds for arbitrary spatial arguments as a regulated correlator or distribution. One can also use number parity: $\mathcal P=(-1)^{\widehat N}$ leaves the vacuum unchanged and sends every creation or annihilation operator, hence the linear field $\widehat f$, to its negative. An odd product consequently has expectation equal to its own negative. Thus [vanishing odd correlators of a free Gaussian field](../../../perturbative-quantum-field-theory.md#vanishing-odd-correlators-of-a-free-gaussian-field) gives

$$
\boxed{\langle0|[\widehat f(\tau,\mathbf0)]^{2n+1}|0\rangle=0\qquad(n=0,1,2,\ldots).}
$$

For a coincident product, impose a momentum regulator or smear the field before taking the expectation; the zero result holds for every such symmetry-preserving regulator. It is not a claim that the unregulated local power is an ordinary finite random variable. Interactions, a non-Gaussian state, or inclusion of a nonzero background mean can invalidate the odd-moment conclusion. Within this free perturbation calculation, the [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) vanishes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
