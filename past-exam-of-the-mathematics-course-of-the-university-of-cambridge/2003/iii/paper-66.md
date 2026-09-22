# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The strongest evidence for large-scale [cosmological isotropy](../../../cosmology.md#cosmological-isotropy) is the nearly direction-independent blackbody temperature of the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background). After removing the dipole associated mainly with our [peculiar velocity](../../../cosmology.md#peculiar-velocity), its residual temperature fluctuations are of order $10^{-5}$. Nearly isotropic counts of distant radio sources and [galaxies](../../../galaxy.md), after correcting for sky coverage and selection effects, provide independent evidence. Local [galaxies](../../../galaxy.md), clusters and voids clearly are not isotropic structures; the claim concerns a statistical description on sufficiently large scales.

Large redshift surveys show that the mean [galaxy](../../../galaxy.md) density stabilizes as increasingly large volumes are sampled, and that the excess pair correlations weaken at large separations. This supports [statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) beyond the characteristic clustering scales. The consistency of large-scale observations in different directions and the success of a common [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) description are additional checks.

[Isotropy](../../../continuum-mechanics.md#isotropy) around one observer does not alone prove [spatial homogeneity](../../../cosmology.md#spatial-homogeneity): a radially varying distribution centered on that observer could look isotropic. The [Copernican principle](../../../cosmology.md#copernican-principle) supplies the assumption that we occupy no preferred position; comparable isotropy about typical locations then supports the [cosmological principle](../../../cosmology.md#cosmological-principle). Surveys observe a finite [past light cone](../../../special-relativity.md#past-light-cone), with source evolution and selection, so they cannot establish homogeneity everywhere on a simultaneous spatial slice. **The evidence supports large-scale statistical isotropy and homogeneity, with substantial small-scale structure and an explicit typical-observer assumption.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use a radial [null geodesic](../../../special-relativity.md#null-geodesic) of the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) in the form $ds^2=-dt^2+a(t)^2d\chi^2$ along a fixed spatial direction, with $c=1$. For an emitter and observer at fixed [comoving coordinates](../../../cosmology.md#comoving-coordinate), the comoving separation is

$$
\chi_o-\chi_e=\int_{t_e}^{t_o}\frac{dt}{a(t)}.
$$

Apply this to two adjacent wave crests. Since their endpoint separation is the same, subtraction to first order gives $\delta t_o/a(t_o)=\delta t_e/a(t_e)$. These intervals are the local periods measured by the [comoving observers](../../../cosmology.md#comoving-observer), so the received wavelength is stretched by $a(t_o)/a(t_e)$. Consequently the [cosmological redshift](../../../cosmology.md#cosmological-redshift) obeys

$$
\boxed{1+z=\frac{\lambda_o}{\lambda_e}=\frac{a(t_o)}{a(t_e)}=\frac1{a(t_e)}}
$$

when $a(t_o)=1$. This relation assumes comoving emitter and observer; additional [peculiar velocities](../../../cosmology.md#peculiar-velocity) supply kinematic redshift factors.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A [comoving coordinate](../../../cosmology.md#comoving-coordinate) labels a location in the expanding background and is constant for an object moving with the [Hubble flow](../../../cosmology.md#hubble-flow). For example, a radial comoving geodesic coordinate $\chi$ gives [proper distance in cosmology](../../../cosmology.md#proper-distance-in-cosmology) $d(t)=a(t)\chi$ along the constant-cosmic-time slice. In a flat background one can write physical coordinates $\mathbf r=a(t)\mathbf x$ and split the physical velocity as

$$
\boxed{\dot{\mathbf r}=H\mathbf r+\mathbf v_{\rm pec},\qquad\mathbf v_{\rm pec}=a\dot{\mathbf x}.}
$$

Thus [proper distance in cosmology](../../../cosmology.md#proper-distance-in-cosmology) is measured using the spatial metric at a specified epoch, whereas a [comoving distance](../../../cosmology.md#comoving-radial-distance) factors out the overall expansion. A proper distance on a simultaneous spatial slice is not automatically the [luminosity distance](../../../cosmology.md#luminosity-distance) or a distance directly inferred from light received today. In a curved spatial geometry $a\chi$ is the radial proper distance, while the sphere's circumference involves the corresponding curved radial function.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) gives the gravitational deceleration from a uniform pressureless matter density, plus the acceleration from a [cosmological constant](../../../cosmology.md#cosmological-constant). Here $\rho$ is the matter mass density, $G$ is the [gravitational constant](../../../classical-mechanics.md#gravitational-constant), $H=\dot a/a$ is the [Hubble parameter](../../../cosmology.md#hubble-parameter), and $k$ is the constant spatial-curvature coefficient in the chosen normalization of $a$. The [Friedmann equation](../../../cosmology.md#friedmann-equations) is the first integral relating expansion to density, curvature and vacuum energy. With $c=1$, the matter, curvature and cosmological-constant contributions to $H^2$ are $8\pi G\rho/3$, $-k/a^2$ and $\Lambda/3$. The [cosmological constant](../../../cosmology.md#cosmological-constant) has effective density $\Lambda/(8\pi G)$ and [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) $w=-1$; its negative pressure explains its positive acceleration contribution when $\Lambda>0$.

For the Newtonian derivation with $\Lambda=0$, follow a test mass on the edge of a uniform sphere of physical radius $R=a\chi$. Conservation of the enclosed matter gives $M=4\pi\rho R^3/3$ constant. The [shell theorem](../../../physics.md#spherical-shell-theorem) removes the force of external spherical shells and gives

$$
\ddot R=-\frac{GM}{R^2}=-\frac{4\pi G}{3}\rho R,
\qquad
\boxed{\frac{\ddot a}{a}=-\frac{4\pi G}{3}\rho.}
$$

Integrating the force equation once gives the conserved specific [mechanical energy](../../../classical-mechanics.md#mechanical-energy)

$$
\varepsilon=\frac12\dot R^2-\frac{GM}{R}.
$$

Divide by $R^2/2=a^2\chi^2/2$ to obtain

$$
H^2=\frac{8\pi G}{3}\rho+\frac{2\varepsilon}{a^2\chi^2}
=\frac{8\pi G}{3}\rho-\frac{k}{a^2},\qquad k=-\frac{2\varepsilon}{\chi^2}.
$$

Homologous motion makes $\varepsilon/\chi^2$ constant between shells. Newtonian mechanics supplies this energy integration constant; its interpretation as intrinsic spatial curvature belongs to the relativistic [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric).

An outward acceleration $\Lambda\mathbf r/3$ comes from the Newtonian potential per unit mass

$$
\boxed{\Phi_\Lambda(\mathbf r)=-\frac{\Lambda r^2}{6}+\text{constant},}
$$

since $-\nabla\Phi_\Lambda=\Lambda\mathbf r/3$. With conventional dimensional $\Lambda$, restore $c^2$ in this potential and the corresponding acceleration and Friedmann terms.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A genuine nondegenerate bounce has $\dot a_*=0$ and $\ddot a_*>0$; using $\ddot a_*\geq0$ also includes the limiting stationary case. Put $s=a_*^{-1}=1+z_*$, and define the present [matter density parameter](../../../cosmology.md#matter-density-parameter) $\Omega_m=8\pi G\rho_0/(3H_0^2)$, $\Omega_\Lambda=\Lambda/(3H_0^2)$ and $\Omega_k=-k/H_0^2$. The dust-plus-cosmological-constant [Friedmann equation](../../../cosmology.md#friedmann-equations) and its acceleration equation become

$$
\frac{H^2}{H_0^2}=\Omega_m a^{-3}+\Omega_k a^{-2}+\Omega_\Lambda,
\qquad
\frac{\ddot a}{aH_0^2}=-\frac12\Omega_m a^{-3}+\Omega_\Lambda,
\qquad \Omega_m+\Omega_k+\Omega_\Lambda=1.
$$

At the bounce these give

$$
\Omega_m s^3+\Omega_k s^2+\Omega_\Lambda=0,
\qquad \Omega_\Lambda\geq\frac12\Omega_m s^3.
$$

For a past bounce with $s>1$, eliminate $\Omega_k$ from the first equation:

$$
\Omega_\Lambda=\frac{s^2+\Omega_m(s^3-s^2)}{s^2-1}.
$$

Subtracting $\Omega_m s^3/2$ and multiplying by the positive denominator gives

$$
0\leq s^2\left[1-\frac{\Omega_m}{2}(s^3-3s+2)\right]
=s^2\left[1-\frac{\Omega_m}{2}(s-1)^2(s+2)\right].
$$

Thus the [matter bound from a Friedmann bounce](../../../cosmology.md#matter-bound-from-a-friedmann-bounce) is

$$
\boxed{\Omega_m\leq\frac{2}{z_*^2(z_*+3)}.}
$$

Strict positive bounce acceleration makes this inequality strict. The zero of the Friedmann equation also requires positive curvature for positive matter and positive $\Lambda$.

An observed source at $z=6$ has $a_e=1/7$. Since the minimum scale factor cannot exceed the scale factor at emission, $z_*\geq6$. The denominator of the bound increases with positive $z_*$, so

$$
\boxed{\Omega_m\leq\frac{2}{6^2(6+3)}=\frac1{162}\simeq0.00617.}
$$

The observational lower bound is much larger. Cluster [mass-to-light ratios](../../../galaxy.md#mass-to-light-ratio), inferred independently from motions, gas temperatures and [gravitational lensing](../../../general-relativity.md#gravitational-lensing), combined with the observed luminosity density imply substantial cosmic mass density. Measurements of the [cosmic baryon fraction](../../../cosmology.md#cosmic-baryon-fraction) from representative clusters, combined with the baryon [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) inferred from [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), provide another estimate: $\Omega_m\simeq\Omega_b/f_b$. Large-scale clustering and [peculiar velocities](../../../cosmology.md#peculiar-velocity) provide independent dynamical checks, although their interpretation must account for galaxy bias. These methods support matter densities of order a few tenths, rather than below one percent. **The dust-plus-cosmological-constant bouncing model is incompatible with both a quasar at redshift six and the stated observational evidence for $\Omega_m\gtrsim0.2$.**

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a flat universe containing only the stated fluid, the [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) is $\dot\rho+3H(\rho+P)=0$. A constant [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) $w$ therefore gives $\rho=\rho_0(a/a_0)^{-3(1+w)}$. Combine this with the [Friedmann equation](../../../cosmology.md#friedmann-equations) $H^2=8\pi G\rho/3$ to find

$$
\dot H=-\frac32(1+w)H^2.
$$

On the expanding branch, specifying $H(t_0)=H_0>0$ yields

$$
\boxed{H(t)=\frac{H_0}{1+\frac32(1+w)H_0(t-t_0)},\qquad
\rho(t)=\frac{3H(t)^2}{8\pi G},\qquad q=-\frac{\ddot a}{aH^2}=\frac{1+3w}{2}.}
$$

The solution is used only where its denominator is positive. For $w\ne-1$, integration also gives

$$
\frac{a(t)}{a_0}=\left[1+\frac32(1+w)H_0(t-t_0)\right]^{2/[3(1+w)]}.
$$

For $w>-1$, choosing the zero of time at the initial singularity gives $H=2/[3(1+w)t]$ and $\rho=1/[6\pi G(1+w)^2t^2]$. For $w=-1$, $H=H_0$, $\rho$ is constant and $a=a_0e^{H_0(t-t_0)}$. For $w<-1$, the displayed initial-value solution instead grows towards a future finite-time singularity; it is not the ordinary positive-time Big Bang branch. With positive density, **accelerated expansion requires $w<-1/3$.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Adding and subtracting the canonical [scalar field](../../../quantum-field-theory.md#scalar-field) density and pressure gives

$$
\dot\phi^2=(1+w)\rho_\phi,\qquad V=\frac{1-w}{2}\rho_\phi.
$$

A real scalar with positive kinetic energy consequently needs $w\geq-1$. On the expanding scalar-dominated branch, divide $\dot\phi$ by $H$ and use the [Friedmann equation](../../../cosmology.md#friedmann-equations):

$$
\frac{d\phi}{d\log a}=\frac{\dot\phi}{H}
=\pm\sqrt{\frac{3(1+w)}{8\pi G}}.
$$

Choose the positive rolling sign. Integration and elimination of $a$ using $\rho_\phi=\rho^0_\phi(a/a_0)^{-3(1+w)}$ give the [scalar-field reconstruction for a constant equation of state](../../../cosmology.md#scalar-field-reconstruction-for-a-constant-equation-of-state):

$$
\boxed{\phi(a)=\phi_0+\sqrt{\frac{3(1+w)}{8\pi G}}\log\frac a{a_0},}
$$



$$
\boxed{V(\phi)=\frac{1-w}{2}\rho^0_\phi
\exp\left[-\sqrt{24\pi G(1+w)}(\phi-\phi_0)\right].}
$$

Changing the rolling sign reverses the exponential slope. At $w=-1$, $\phi$ is constant and $V=\rho^0_\phi$; elimination by an invertible $\phi(a)$ then degenerates. The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) gives $\ddot\phi+3H\dot\phi+V_{,\phi}=0$ whenever $\dot\phi\ne0$, so the reconstruction satisfies the field equation as well as the Friedmann equation.

Compare the reconstructed exponent with $V_0e^{-\lambda\sqrt{8\pi G}\phi}$. In this constant-$w$, scalar-dominated scaling solution,

$$
\lambda^2=3(1+w),\qquad w=-1+\frac{\lambda^2}{3},\qquad a\propto t^{2/\lambda^2}.
$$

Strict $\rho_\phi+P_\phi>0$ requires $w>-1$, and acceleration requires $w<-1/3$. Hence

$$
\boxed{0<\lambda<\sqrt2.}
$$

The accelerating branch has $V_0>0$. The zero-slope limit is a constant potential with $\rho+P=0$, so it does not meet the strict inequality. This result characterizes the [exponential-potential power-law inflation](../../../cosmic-inflation.md#exponential-potential-power-law-inflation) solution; an arbitrary trajectory with the same potential need not have constant $w$ throughout its evolution.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For equal intrinsic bolometric luminosities $L$, the observed fluxes are $F(z)=L/[4\pi d_L(z)^2]$. In the flat model, a [null geodesic](../../../special-relativity.md#null-geodesic) gives the [comoving distance](../../../cosmology.md#comoving-radial-distance) $\chi(z)=c\int_0^z dz'/H(z')$. Photon energies and arrival rates each bring one factor of $1+z$, yielding the [luminosity distance](../../../cosmology.md#luminosity-distance) $d_L=(1+z)\chi$. Thus

$$
\boxed{\frac{F(z_1)}{F(z_2)}=
\left[\frac{(1+z_2)\int_0^{z_2}dz'/H(z')}
{(1+z_1)\int_0^{z_1}dz'/H(z')}\right]^2.}
$$

For the one-component constant-$w$ universe, $H(z)=H_0(1+z)^{3(1+w)/2}$. Its [luminosity distance](../../../cosmology.md#luminosity-distance) is

$$
d_L(z)=\frac{2c(1+z)}{H_0(1+3w)}
\left[1-(1+z)^{-(1+3w)/2}\right]\quad(w\ne-1/3),
$$

with the continuous limit $d_L=c(1+z)\log(1+z)/H_0$ for $w=-1/3$. Measurements spanning several redshifts fit the shape of this relation and hence $w$; the common luminosity and $H_0$ cancel in the flux ratio. Equivalently, the relative distance modulus is $5\log_{10}[d_L(z_2)/d_L(z_1)]$.

Actual [Type Ia supernovae](../../../stellar-astrophysics.md#type-ia-supernova) are standardized through their light-curve shape and color rather than being identical [standard candles](../../../astrophysics.md#standard-candle). Scatter, dust extinction, changes in progenitor populations, photometric calibration, spectral corrections between observed bands, flux-limited selection, lensing magnification and low-redshift [peculiar velocities](../../../cosmology.md#peculiar-velocity) all affect inferred distances. The assumed cosmological model is another uncertainty: with a separate matter component, $H^2/H_0^2=\Omega_m(1+z)^3+(1-\Omega_m)(1+z)^{3(1+w)}$ in the flat case, so $w$ is partly degenerate with $\Omega_m$; allowing spatial curvature or varying $w$ adds degeneracies. **Flux ratios constrain the expansion history through an integral of $1/H(z)$, rather than measuring $w$ directly without model assumptions.**

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For pressureless matter with curvature and a possible constant [cosmological constant](../../../cosmology.md#cosmological-constant), write the background [Friedmann equation](../../../cosmology.md#friedmann-equations) as

$$
H^2=Aa^{-3}+Ba^{-2}+C,\qquad A=H_0^2\Omega_m,\quad B=-k,\quad C=\Lambda/3.
$$

Differentiating on the expanding branch gives

$$
\dot H=-\frac32Aa^{-3}-Ba^{-2},\qquad
\ddot H=H\left(\frac92Aa^{-3}+2Ba^{-2}\right).
$$

Consequently

$$
\ddot H+2H\dot H-\frac32Aa^{-3}H
=H\left[\left(\frac92-3-\frac32\right)Aa^{-3}+(2-2)Ba^{-2}\right]=0.
$$

This proves that the [Hubble parameter as a solution of the dust growth equation](../../../linear-cosmological-density-perturbation.md#hubble-parameter-as-a-solution-of-the-dust-growth-equation) is valid, including constant-$\Lambda$ and curvature contributions to the background. It does not extend without change to a radiation background or arbitrary dynamical dark energy.

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $a\propto t^{2/3}$, $H=2/(3t)$ and $4\pi G\bar\rho=2/(3t^2)$. The [linear matter perturbation growth equation](../../../linear-cosmological-density-perturbation.md#linear-matter-perturbation-growth-equation) becomes

$$
\ddot D+\frac4{3t}\dot D-\frac2{3t^2}D=0.
$$

Substitute $D=t^p$. The indicial equation is $p(p-1)+4p/3-2/3=0$, with roots $2/3$ and $-1$. Therefore

$$
\boxed{D(t)=C_+t^{2/3}+C_-t^{-1},\qquad D_+\propto a,\quad D_-\propto H\propto a^{-3/2}.}
$$

**The Hubble-parameter solution is the decaying mode in the Einstein-de Sitter universe.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
\delta(\mathbf x)=\int\frac{d^3k}{(2\pi)^3}\delta_{\mathbf k}e^{-i\mathbf k\cdot\mathbf x},
\qquad
\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta_D^{(3)}(\mathbf k-\mathbf k')P(k).
$$

[Statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) makes the Fourier covariance diagonal, and isotropy makes the [matter power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) depend only on $k=|\mathbf k|$. The [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) $\xi(r)=\langle\delta(\mathbf x)\delta(\mathbf x+\mathbf r)\rangle$ follows by inserting the transform and using this covariance:

$$
\xi(r)=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
$$

Integrating the polar angle relative to $\mathbf r$ gives $\int d\Omega_k\,e^{ikr\cos\theta}=4\pi\sin(kr)/(kr)$. Hence

$$
\boxed{\xi(r)=\frac1{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin(kr)}{kr}\,dk.}
$$

The inverse isotropic transform is $P(k)=4\pi\int_0^\infty r^2\xi(r)\sin(kr)/(kr)\,dr$ whenever these transforms exist, with distributions or regularization otherwise.

For a spherical average of comoving radius $R$, the [spherical top-hat window function](../../../linear-cosmological-density-perturbation.md#spherical-top-hat-window-function) is

$$
W(kR)=\frac{3[\sin(kR)-kR\cos(kR)]}{(kR)^3}.
$$

At a fixed epoch let $P(k)=Ak^n$. The [scale-free smoothed density variance](../../../large-scale-structure-of-the-universe.md#scale-free-smoothed-density-variance) is

$$
\sigma_\delta^2(R)=\frac{A}{2\pi^2}\int_0^\infty k^{n+2}W(kR)^2dk
=\frac{A R^{-(n+3)}}{2\pi^2}\int_0^\infty y^{n+2}W(y)^2dy.
$$

Thus the RMS fractional mass fluctuation scales as $R^{-(n+3)/2}$; the RMS mass fluctuation itself scales as $\bar\rho R^3\sigma_\delta\propto R^{(3-n)/2}$ at fixed epoch.

The comoving [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives $\Phi_{\mathbf k}=-4\pi G a^2\bar\rho\,\delta_{\mathbf k}/k^2$. For the growing irrotational mode the [linearized cosmological continuity equation](../../../linear-cosmological-density-perturbation.md#linearized-cosmological-continuity-equation) gives $\mathbf v_{\mathbf k}=-iaHf\,\mathbf k\delta_{\mathbf k}/k^2$, where $f=d\log D_+/d\log a$. The averaged-potential and bulk-velocity variances are therefore

$$
\sigma_\Phi^2=\frac{A(4\pi Ga^2\bar\rho)^2}{2\pi^2}\int_0^\infty k^{n-2}W(kR)^2dk,
\qquad
\langle|\mathbf V_R|^2\rangle=\frac{A(aHf)^2}{2\pi^2}\int_0^\infty k^nW(kR)^2dk.
$$

For a single Cartesian component of the isotropic bulk velocity, divide its variance by three. Rescaling $kR$ gives

$$
\boxed{\sigma_\delta\propto R^{-(n+3)/2},\qquad
\sigma_\Phi\propto R^{(1-n)/2},\qquad
\sigma_V\propto R^{-(n+1)/2}.}
$$

These are dimensional scaling laws, with an important convergence qualification. Since $W(y)\to1$ at small $y$ and has large-$y$ envelope $O(y^{-2})$, the density average converges for $-3<n<1$, the absolute potential average for $1<n<5$, and the bulk velocity for $-1<n<3$. No one unbroken power law makes all three absolute averages finite on the entire range $0<k<\infty$. In particular, long-wavelength modes can dominate the potential. Physical infrared/ultraviolet cutoffs, potential differences, or fluctuation amplitudes in a band around $k\sim R^{-1}$ resolve the relevant divergences; with cutoffs the simple powers need not describe the full integrated variance. The [scale-free potential and bulk-flow variance](../../../large-scale-structure-of-the-universe.md#scale-free-potential-and-bulk-flow-variance) laws should be understood with these conditions, not as a claim that divergent RMS integrals are finite.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the same negative-exponent [Fourier transform](../../../analysis.md#fourier-transform) as in the preceding part and let $f=d\log D_+/d\log a$. In linear theory, $\dot\delta=Hf\delta$, and the [linearized cosmological continuity equation](../../../linear-cosmological-density-perturbation.md#linearized-cosmological-continuity-equation) is $\dot\delta+a^{-1}\nabla_x\cdot\mathbf v=0$. Its irrotational solution is

$$
\mathbf v_{\mathbf k}=-iaHf\frac{\mathbf k}{k^2}\delta_{\mathbf k},
\qquad
\mathbf v(\mathbf r)=aHf\nabla_r\int\frac{d^3k}{(2\pi)^3}\frac{\delta_{\mathbf k}}{k^2}e^{-i\mathbf k\cdot\mathbf r}.
$$

Here $\mathbf r$ labels the comoving spatial position for the Fourier expansion. The quantity being differentiated is also $-\Phi/(4\pi Ga^2\bar\rho)$, by the [Poisson equation](../../../partial-differential-equation.md#poisson-equation); thus this explicitly obtains the velocity from the Fourier components of the [peculiar gravitational potential](../../../linear-cosmological-density-perturbation.md#peculiar-gravitational-potential).

Conjugating the [Rayleigh plane-wave expansion](../../../analysis.md#rayleigh-plane-wave-expansion), and using the symmetric addition formula for [spherical harmonics](../../../analysis.md#spherical-harmonic), gives

$$
e^{-i\mathbf k\cdot\mathbf r}=4\pi\sum_{\ell m}(-i)^\ell j_\ell(kr)Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).
$$

For the radial component $U=\mathbf v\cdot\hat r$, differentiate at fixed angular position. Only the [Spherical Bessel function](../../../analysis.md#spherical-bessel-function) depends on $r$, and $d j_\ell(kr)/dr=k j_\ell'(kr)$. Therefore the [radial peculiar velocity in spherical harmonics](../../../cosmology.md#radial-peculiar-velocity-in-spherical-harmonics) is

$$
\boxed{U(\mathbf r)=\frac{aHf}{2\pi^2}\sum_{\ell m}(-i)^\ell
\int d^3k\,\frac{\delta_{\mathbf k}}{k}\frac{d j_\ell(kr)}{d(kr)}
Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).}
$$

The coefficient is $4\pi/(2\pi)^3=1/(2\pi^2)$, and $(-i)^\ell=(i^\ell)^*$, so the phase and conjugation agree with the requested expression. At the present epoch, $a=1$ and $H=H_0$. Adopting the traditional approximation $f\simeq\Omega_m^{0.6}$ gives

$$
\frac{U}{H_0}\simeq\frac{\Omega_m^{0.6}}{2\pi^2}\sum_{\ell m}(i^\ell)^*
\int d^3k\,\frac{\delta_{\mathbf k}}{k}j_\ell'(kr)
Y_{\ell m}(\hat k)Y_{\ell m}^*(\hat r).
$$

The printed expression is therefore the present-epoch result in units with $H_0=1$, or with its velocity interpreted as $U/H_0$. For distances and velocities in ordinary physical units, it needs the factor $H_0$; at a general epoch it needs $aH$. The approximation $f\simeq\Omega_m^{0.6}$ is exact in the Einstein-de Sitter limit but is not an exact growth formula for arbitrary cosmologies.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For a relaxed cluster, galaxy motions act as tracers of its [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass). The [virial theorem](../../../classical-mechanics.md#virial-theorem) gives a dynamical mass of order

$$
\boxed{M_{\rm dyn}\sim\frac{R\sigma_v^2}{G},}
$$

with a profile-dependent coefficient and a projection correction because the observed [velocity dispersion](../../../galaxy.md#velocity-dispersion) is usually only the line-of-sight component. For an isotropic uniform-sphere estimate using its one-dimensional dispersion, $T=3M\sigma_v^2/2$ and $W=-3GM^2/(5R)$ give $M=5R\sigma_v^2/G$. Measured dispersions require much more gravitating mass than the luminous [galaxies](../../../galaxy.md) provide, hence large cluster [mass-to-light ratios](../../../galaxy.md#mass-to-light-ratio). Interlopers, orbital anisotropy and departures from equilibrium are systematic uncertainties, so the independent gas and lensing measurements matter.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The hot intracluster gas emits X-rays, which constrain its temperature and density profile. If its pressure is predominantly thermal and it is in [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium),

$$
\frac{dP}{dr}=-\rho_g\frac{GM(<r)}{r^2},\qquad P=\frac{\rho_g k_BT}{\mu m_p}.
$$

Eliminating the pressure gives

$$
\boxed{M(<r)=-\frac{k_BT(r)r}{G\mu m_p}
\left(\frac{d\log\rho_g}{d\log r}+\frac{d\log T}{d\log r}\right).}
$$

Here $\mu m_p$ is the mean mass per gas particle. A gas at the observed cluster temperatures would not remain confined without a deep [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass); the inferred total mass exceeds the gas and stellar mass together. Nonthermal pressure, mergers, gas clumping and temperature-profile errors can bias this estimate, but do not turn X-ray luminosity itself into a direct measurement of total mass.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

[Gravitational lensing](../../../general-relativity.md#gravitational-lensing) probes the cluster's projected mass through the deflection of background light. [Strong gravitational lensing](../../../general-relativity.md#strong-gravitational-lensing) produces arcs and multiple images; [weak gravitational lensing](../../../general-relativity.md#weak-gravitational-lensing) measures coherent distortions of many background [galaxies](../../../galaxy.md). The lensing convergence is $\kappa=\Sigma/\Sigma_{\rm crit}$, with

$$
\Sigma_{\rm crit}=\frac{c^2}{4\pi G}\frac{D_s}{D_lD_{ls}}.
$$

Thus the image geometry and shear constrain the projected surface density $\Sigma$ without assuming the cluster is in dynamical or [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium). The reconstructed total mass again exceeds the visible stellar and gas contribution. Source-distance errors, line-of-sight structures and the [mass-sheet degeneracy](../../../general-relativity.md#mass-sheet-degeneracy) affect the reconstruction, but the independent agreement of lensing, galaxy motions and gas confinement is strong evidence for cluster [dark matter](../../../cosmology.md#dark-matter).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

An initially overdense spherical region first expands approximately with the background, but its self-gravity slows it more strongly. It reaches [turnaround of spherical collapse](../../../large-scale-structure-of-the-universe.md#turnaround-of-spherical-collapse) at its maximum radius, recollapses, and forms a bound approximately stationary object when infall energy is redistributed into random motions. An exactly cold, uniform pressureless solution would instead collapse to zero radius; virialization replaces that formal endpoint.

For fixed mass $M$ and no [cosmological constant](../../../cosmology.md#cosmological-constant), integrate $\ddot R=-GM/R^2$ for a bound shell. Its specific energy can be written $\varepsilon=-GM/(2A)$, and the cycloidal parametrization is

$$
R=A(1-\cos\theta),\qquad t=B(\theta-\sin\theta),\qquad A^3=GMB^2.
$$

Substitution in $\dot R^2/2-GM/R=\varepsilon$ verifies this parametrization. At $\theta=\pi$, $R_{\rm ta}=2A$ and $t_{\rm ta}=\pi B$; formal collapse occurs at $\theta=2\pi$, so $t_{\rm coll}=2t_{\rm ta}$.

<a id="4/b/image-expansion-turnaround-and-idealized-virialization-of-a-spherical-overdensity-compared-with-formal-cold-collapse"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-66-spherical-collapse.png)

**[Figure 1](#4/b/image-expansion-turnaround-and-idealized-virialization-of-a-spherical-overdensity-compared-with-formal-cold-collapse). Expansion, turnaround and idealized virialization of a spherical overdensity, compared with formal cold collapse**.

For a uniform sphere, $W=-3GM^2/(5R)$. At turnaround the coherent kinetic energy vanishes, so $E=W_{\rm ta}$. At the final equilibrium, the [virial theorem](../../../classical-mechanics.md#virial-theorem) gives $2T_{\rm vir}+W_{\rm vir}=0$, whence $E=W_{\rm vir}/2$. [Conservation of energy](../../../physics.md#conservation-of-energy) therefore implies

$$
\boxed{R_{\rm vir}=\frac{R_{\rm ta}}2,\qquad\rho_{\rm vir}=8\rho_{\rm ta}.}
$$

This [virial radius from turnaround energy](../../../large-scale-structure-of-the-universe.md#virial-radius-from-turnaround-energy) assumes conserved mass and energy, negligible surface-pressure/tidal terms, and the same gravitational profile coefficient. The sketch's settling segment is qualitative; the cycloid is the exact pre-virialization cold model, not a dissipative relaxation solution.

To compare with the cosmological density, use $\bar\rho(t)=1/(6\pi Gt^2)$ in an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe). The turnaround sphere has

$$
\rho_{\rm ta}=\frac{3M}{4\pi(2A)^3}=\frac3{32\pi GB^2},
\qquad
\frac{\rho_{\rm ta}}{\bar\rho(t_{\rm ta})}=\frac{9\pi^2}{16}.
$$

Since the background density falls by four between $t_{\rm ta}$ and $t_{\rm coll}$, the [Einstein-de Sitter virial overdensity](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-virial-overdensity) is

$$
\boxed{\frac{\rho_{\rm vir}}{\bar\rho(t_{\rm coll})}=32\frac{9\pi^2}{16}=18\pi^2.}
$$

Finally $\bar\rho(z)=\rho_0(1+z)^3$, so assigning the nominal collapse redshift gives

$$
\boxed{\rho_{\rm vir}(z_{\rm coll})=18\pi^2\rho_0(1+z_{\rm coll})^3.}
$$

The density ratio eight compares the same object's physical densities at turnaround and virialization; $18\pi^2$ compares its final density with the background at the later collapse epoch.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Follow a conserved mass element from its [Lagrangian coordinate](../../../continuum-mechanics.md#lagrangian-coordinate) $\mathbf q$ to its [Eulerian coordinate](../../../continuum-mechanics.md#eulerian-coordinate) $\mathbf x=\mathbf q+b\mathbf p$. The integrated [continuity equation](../../../physics.md#continuity-equation) gives

$$
\rho(\mathbf r,t)a^3\,d^3x=\rho_0\,d^3q,
\qquad
1+\delta=\frac{\rho}{\bar\rho}=
\frac1{J},\qquad J=\det\left(\delta_{ij}+b\frac{\partial p_i}{\partial q_j}\right),
$$

where $\bar\rho=\rho_0/a^3$ and the Lagrangian labels are chosen with uniform reference mass per $d^3q$. These equations hold before [shell crossing](../../../large-scale-structure-of-the-universe.md#shell-crossing), when the oriented determinant is positive. If $\mu_i$ are the eigenvalues of $\partial p_i/\partial q_j$, then

$$
\boxed{1+\delta=\prod_{i=1}^3(1+b\mu_i)^{-1}.}
$$

For an irrotational displacement the deformation matrix is symmetric, so these eigenvalues are real. Using the conventional positive collapse eigenvalues $\lambda_i=-\mu_i$, equivalently the eigenvalues of $-\partial p_i/\partial q_j$, gives

$$
\boxed{1+\delta=\prod_{i=1}^3(1-b\lambda_i)^{-1}.}
$$

There is a sign mismatch in the printed pairing of this last expression with eigenvalues of $+\partial p_i/\partial q_j$: for the displayed plus-sign displacement map, those eigenvalues give plus signs in the determinant. For example, $p_1=cq_1$, $p_2=p_3=0$ makes $x_1=(1+bc)q_1$, so mass conservation gives $1+\delta=(1+bc)^{-1}$, not $(1-bc)^{-1}$. The corrected eigenvalue convention restores the intended formula without changing the map.

Now take $\mathbf p=(p(q_1),0,0)$ and $J=1+bp'$. The physical trajectory is $\mathbf r=a\mathbf x$. Differentiating at fixed $\mathbf q$ gives

$$
\ddot{\mathbf r}=\frac{\ddot a}{a}\mathbf r+
 a(\ddot b+2H\dot b)\mathbf p
=\frac{\ddot a}{a}\mathbf r+4\pi Ga\bar\rho b\mathbf p.
$$

The physical derivative in the perturbed direction is $\partial/\partial r_1=[a(1+bp')]^{-1}\partial/\partial q_1$. The two transverse directions still have the background acceleration. Therefore

$$
\nabla_r\cdot\ddot{\mathbf r}
=3\frac{\ddot a}{a}+4\pi G\bar\rho\frac{bp'}{1+bp'}.
$$

Use the pressureless, $\Lambda=0$ background acceleration equation $3\ddot a/a=-4\pi G\bar\rho$ to obtain

$$
\boxed{\nabla_r\cdot\ddot{\mathbf r}
=-\frac{4\pi G\bar\rho}{1+bp'}=-4\pi G\rho(\mathbf r,t).}
$$

This proves the [planar exactness of the Zeldovich approximation](../../../large-scale-structure-of-the-universe.md#planar-exactness-of-the-zeldovich-approximation) for the requested full force-divergence equation. The displacement depends on only one coordinate, but the divergence includes all three physical directions; discarding the transverse background terms would give the wrong result. The proof is valid until [shell crossing](../../../large-scale-structure-of-the-universe.md#shell-crossing). With the planar gravitational boundary condition fixing the possible spatially uniform force, it is the exact single-stream dust evolution; it does not describe the multistream density by a single invertible map after crossing.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
