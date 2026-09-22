# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper73.pdf)

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
    - [a](#1/v/a)
      - [Solution](#1/v/a/solution)
    - [b](#1/v/b)
      - [Solution](#1/v/b/solution)
  - [vi](#1/vi)
    - [a](#1/vi/a)
      - [Solution](#1/vi/a/solution)
    - [b](#1/vi/b)
      - [Solution](#1/vi/b/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [a](#4/iii/a)
      - [Solution](#4/iii/a/solution)
    - [b](#4/iii/b)
      - [Solution](#4/iii/b/solution)
    - [c](#4/iii/c)
      - [Solution](#4/iii/c/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A [kinematic redshift](../../../physics.md#kinematic-redshift) is the [relativistic Doppler effect](../../../physics.md#relativistic-doppler-effect) arising from relative motion of emitter and receiver. In a local inertial frame, recession decreases the received [frequency](../../../physics.md#frequency) and approach increases it. A [cosmological redshift](../../../cosmology.md#cosmological-redshift) instead compares photons emitted and received by comoving observers at different [cosmic times](../../../cosmology.md#cosmic-time): expansion of the [scale factor](../../../cosmology.md#scale-factor-cosmology) stretches their [wavelengths](../../../wave-equation.md#wavelength). It exists even when both observers have zero [peculiar velocity](../../../cosmology.md#peculiar-velocity). Both are frequency ratios measured by observers, but a large [cosmological redshift](../../../cosmology.md#cosmological-redshift) should not be inserted into a flat-spacetime radial-speed formula to define the galaxy's unique recession speed.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Take $v>0$ for recession. By the definition of [kinematic redshift](../../../physics.md#kinematic-redshift), $1+z_{\rm kin}=\nu_e/\nu_0$. Inverting the supplied [relativistic Doppler effect](../../../physics.md#relativistic-doppler-effect) and expanding with $\beta=v/c$ gives

$$
1+z_{\rm kin}=\sqrt{\frac{1+\beta}{1-\beta}}
=(1+\tfrac12\beta+O(\beta^2))(1+\tfrac12\beta+O(\beta^2))
=1+\beta+O(\beta^2).
$$

Thus

$$
\boxed{z_{\rm kin}\simeq v/c\quad\text{for }|v|\ll c.}
$$

A negative radial [velocity](../../../classical-mechanics.md#velocity) gives a blueshift at this order.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For a [radial null geodesic in FLRW spacetime](../../../cosmology.md#radial-null-geodesic-in-flrw-spacetime), the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) gives $c\,dt/a(t)=\pm dr/\sqrt{1-kr^2}$. The emitter and receiver have fixed comoving coordinates, so two successive wave crests satisfy the same [comoving radial distance](../../../cosmology.md#comoving-radial-distance) relation:

$$
\int_{t_e}^{t_0}\frac{c\,dt}{a(t)}
=\int_{t_e+\delta t_e}^{t_0+\delta t_0}\frac{c\,dt}{a(t)}.
$$

Subtracting the two expressions in the short-wave-period limit yields $\delta t_e/a(t_e)=\delta t_0/a(t_0)$. Comoving observers measure these intervals as [proper time](../../../special-relativity.md#proper-time); since $\nu=1/\delta t$,

$$
\boxed{1+z_{\rm cosm}=\frac{\nu_e}{\nu_0}
=\frac{a(t_0)}{a(t_e)}.}
$$

For a fixed reception epoch, the [cosmological redshift](../../../cosmology.md#cosmological-redshift) factor is inversely proportional to the emission [scale factor](../../../cosmology.md#scale-factor-cosmology). This also shows the associated [cosmological time dilation](../../../cosmology.md#cosmological-time-dilation).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

In the intended comparison of emission and reception epochs, with negligible [peculiar velocities](../../../cosmology.md#peculiar-velocity), the Earth-observed [cosmological redshifts](../../../cosmology.md#cosmological-redshift) correspond to $a_A=a_0/2$ and $a_B=a_0/10$. A photon emitted at the B epoch and received at the A epoch consequently has

$$
\boxed{1+z_{B\to A}=\frac{a_A}{a_B}=\frac{10}{2}=5,
\qquad z_{B\to A}=4.}
$$

These factors divide, whereas the redshifts themselves do not subtract. There is a geometrical qualification to this usual answer: the two Earth-observed redshifts alone do not specify an arbitrary actual B-to-A observation. The assumed events must be connected by a [null geodesic](../../../special-relativity.md#null-geodesic), as when A is on the same radial photon path between B and Earth. If the galaxies have an unspecified angular separation, or A observes at a different [cosmic time](../../../cosmology.md#cosmic-time), the B emission event reaching A is different and its redshift is not determined by these two numbers alone.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The [combined kinematic and cosmological redshift](../../../cosmology.md#combined-kinematic-and-cosmological-redshift) is most cleanly found by passing through the emitter's local comoving frame. The distance estimate then requires an explicit approximation to the [Hubble law](../../../cosmology.md#hubble-s-law).

<h4 id="1/v/a">a</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/a/solution">Solution</h5>

↑ **Parent:** [A](#1/v/a)

Let $\nu_c$ be the photon [frequency](../../../physics.md#frequency) in the local comoving frame just after emission. The [kinematic redshift](../../../physics.md#kinematic-redshift) gives $\nu_e/\nu_c=1+z_{\rm kin}$, and propagation in the [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) gives $\nu_c/\nu_0=1+z_{\rm cosm}$. Multiplication gives

$$
\boxed{1+z_{\rm tot}=(1+z_{\rm cosm})(1+z_{\rm kin}).}
$$

Equivalently, $z_{\rm tot}=z_{\rm cosm}+z_{\rm kin}+z_{\rm cosm}z_{\rm kin}$. Both redshifts being small is what permits their approximate addition. Here the observer's own [peculiar velocity](../../../cosmology.md#peculiar-velocity) is assumed already corrected to the [Hubble flow](../../../cosmology.md#hubble-flow) frame.

<h4 id="1/v/b">b</h4>

↑ **Parent:** [V](#1/v)

<h5 id="1/v/b/solution">Solution</h5>

↑ **Parent:** [B](#1/v/b)

In the local, nonrelativistic [Hubble law](../../../cosmology.md#hubble-s-law) approximation, $cz_{\rm tot}\simeq H_0r+v_p$. Ignoring the [peculiar velocity](../../../cosmology.md#peculiar-velocity) gives an inferred distance $r_{\rm est}=r+v_p/H_0$, so

$$
\frac{|r_{\rm est}-r|}{r}\leq\frac{600}{100r}
=\frac{6\,\mathrm{Mpc}}{r}.
$$

The requested accuracy therefore requires

$$
\boxed{r>120\,\mathrm{Mpc},\qquad r_{\min}\simeq120\,\mathrm{Mpc}.}
$$

At exactly $120\,\mathrm{Mpc}$ the worst-case error is $5\%$, so “better than” requires a strictly larger distance. This is the conventional leading-order estimate. If one retains the exact Doppler factor and the product term while treating $r=cz_{\rm cosm}/H_0$ as exact, the positive-velocity case gives $|\Delta r|/r=(1+z_{\rm cosm})q/z_{\rm cosm}$, with $q=\sqrt{(1+600/c)/(1-600/c)}-1$. It requires $r>(c/H_0)q/(0.05-q)\simeq125\,\mathrm{Mpc}$. That small refinement is conditional on the distance-redshift prescription; the simple $120\,\mathrm{Mpc}$ answer uses the local approximation consistently.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/a">a</h4>

↑ **Parent:** [Vi](#1/vi)

<h5 id="1/vi/a/solution">Solution</h5>

↑ **Parent:** [A](#1/vi/a)

For [Planck law](../../../statistical-physics.md#planck-s-law) expressed per unit [frequency](../../../physics.md#frequency), put $x=h\nu/(k_BT)$. At fixed [temperature](../../../thermodynamics.md#temperature), the frequency dependence is $B_\nu\propto T^3x^3/(e^x-1)$. Differentiation gives

$$
\frac{d}{dx}\frac{x^3}{e^x-1}
=\frac{x^2[3(e^x-1)-xe^x]}{(e^x-1)^2}.
$$

The positive interior maximum therefore satisfies $3(1-e^{-x_*})=x_*$, with $x_*=2.821439\ldots$ independent of [temperature](../../../thermodynamics.md#temperature). The zero solution of the rearranged equation is a boundary, not the interior maximum. Hence the [frequency form of Wien's displacement law](../../../astrophysics.md#frequency-form-of-wien-s-displacement-law) is

$$
\boxed{\frac{\nu_{\max}}{T}=\frac{x_*k_B}{h}
\simeq5.88\times10^{10}\,\mathrm{Hz\,K^{-1}}.}
$$

This frequency peak is not $c$ divided by the peak wavelength of $B_\lambda$: the two spectral densities differ by the frequency-to-wavelength Jacobian.

<h4 id="1/vi/b">b</h4>

↑ **Parent:** [Vi](#1/vi)

<h5 id="1/vi/b/solution">Solution</h5>

↑ **Parent:** [B](#1/vi/b)

Motion toward incoming [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) radiation produces a blueshift. The photon occupation function of a [blackbody](../../../astrophysics.md#blackbody) depends on $h\nu/(k_BT)$, so the same Doppler factor multiplies both [frequency](../../../physics.md#frequency) and effective [temperature](../../../thermodynamics.md#temperature). Looking forward along the Sun's [peculiar velocity](../../../cosmology.md#peculiar-velocity), one obtains

$$
T_{\rm forward}=T_0\sqrt{\frac{1+\beta}{1-\beta}}
\simeq T_0(1+\beta),\qquad \beta\simeq300/(3\times10^5)=10^{-3}.
$$

Taking the mean [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) [temperature](../../../thermodynamics.md#temperature) as about $2.73\,\mathrm K$ gives

$$
\boxed{\Delta T_{\rm forward}\simeq2.7\,\mathrm{mK},
\qquad T_{\rm forward}\simeq2.733\,\mathrm K.}
$$

The numerical total inherits the rounded mean temperature; the robust estimate is the positive millikelvin dipole increment.

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

A [K correction](../../../astrophysics.md#k-correction) accounts for observing a redshifted spectrum through a fixed [photometric passband](../../../astrophysics.md#photometric-passband), rather than the corresponding emitted band. In the same R-band [astronomical magnitude](../../../astrophysics.md#astronomical-magnitude) convention,

$$
M_R=m_R-5\log_{10}(d_L/10\,\mathrm{pc})-K_R.
$$

The [luminosity distance](../../../cosmology.md#luminosity-distance) already incorporates bolometric dimming; the additional correction depends on spectral shape and band response. At $z=3$, observed R-band light at $660\,\mathrm{nm}$ was emitted at $165\,\mathrm{nm}$, in the far ultraviolet. It is not a direct measurement of rest-frame R-band luminosity.

To fix the sign, let $L_\nu$ be emitted spectral [luminosity](../../../astrophysics.md#luminosity) and approximate R as narrow. Counting photon energy, arrival time and the transformed frequency interval gives $F_{\nu_o}=(1+z)L_{(1+z)\nu_o}/(4\pi d_L^2)$. Thus

$$
K_R=-2.5\log_{10}\!\left[(1+z)
\frac{L_\nu((1+z)\nu_R)}{L_\nu(\nu_R)}\right],
\qquad M_{R,\rm ignored}-M_R=K_R.
$$

For an ordinary old [elliptical galaxy](../../../galaxy.md#elliptical-galaxy), the far-ultraviolet spectrum is weak relative to the optical, so typically $L_\nu(165\,\mathrm{nm})/L_\nu(660\,\mathrm{nm})<1/4$. Then $K_R>0$: **neglecting it overestimates the numerical absolute magnitude and underestimates the R-band luminosity**. For a young, unobscured [star-forming galaxy](../../../galaxy.md#star-forming-galaxy), hot stars make the far-ultraviolet strong, with an approximately flat $L_\nu$ spectrum often serving as a useful model. It gives $K_R=-2.5\log_{10}4\simeq-1.51$: **neglecting it underestimates the numerical absolute magnitude and overestimates the R-band luminosity**. Strong dust extinction or an unusual spectrum can reverse this latter sign; a galaxy label alone does not prove an exact correction. The band-integrated convention is given in [Hogg and collaborators' definition of the K-correction](https://arxiv.org/abs/astro-ph/0210394).

## 2

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Divide the [Friedmann equation](../../../cosmology.md#friedmann-equations) by $a^2$ and use $a=(1+z)^{-1}$. The [Hubble parameter](../../../cosmology.md#hubble-parameter) therefore satisfies

$$
\boxed{\frac{H(z)}{H_0}
=\sqrt{\Omega_{m,0}(1+z)^3+\Omega_{\Lambda,0}}.}
$$

The positive root describes the expanding branch. Spatial flatness and the neglect of [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology) imply $\Omega_{m,0}+\Omega_{\Lambda,0}=1$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [age of an FLRW universe](../../../cosmology.md#age-of-an-flrw-universe) at an epoch is the elapsed [cosmic time](../../../cosmology.md#cosmic-time) since the [Big Bang](../../../cosmology.md#big-bang), not the lookback time from today. For positive matter and positive [cosmological constant](../../../cosmology.md#cosmological-constant), integrating $dt=da/\dot a$ gives

$$
t(a)=\frac1{H_0}\int_0^a\frac{\sqrt{a'}\,da'}
{\sqrt{\Omega_{m,0}+\Omega_{\Lambda,0}a'^3}}.
$$

Put $u=\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a'^{3/2}$; then $du=(3/2)\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\sqrt{a'}\,da'$. The integral becomes the [age of a flat matter-Lambda universe](../../../cosmology.md#age-of-a-flat-matter-lambda-universe):

$$
t(a)=\frac{2}{3H_0\sqrt{\Omega_{\Lambda,0}}}
\int_0^{\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a^{3/2}}
\frac{du}{\sqrt{1+u^2}}
=\frac{2\operatorname{arsinh}\!\left(\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a^{3/2}\right)}
{3H_0\sqrt{\Omega_{\Lambda,0}}}.
$$

Choose $0<\theta<\pi/2$ such that $\tan\theta=\sqrt{\Omega_{m,0}/\Omega_{\Lambda,0}}\,a^{-3/2}$. The upper-limit value of $u$ is $\cot\theta$, and

$$
\operatorname{arsinh}(\cot\theta)
=\log(\cot\theta+\csc\theta)
=\log\frac{1+\cos\theta}{\sin\theta}.
$$

Consequently

$$
\boxed{t(z)=\frac{2}{3H_0\sqrt{\Omega_{\Lambda,0}}}
\log\frac{1+\cos\theta}{\sin\theta},
\qquad \tan\theta=\sqrt{\frac{\Omega_{m,0}}{\Omega_{\Lambda,0}}}(1+z)^{3/2}.}
$$

The integration constant is fixed by $t\to0$ as $z\to\infty$, where $\theta\to\pi/2$. Equivalently, differentiating $u=\cot\theta$ changes the last integral to $-\int d\theta/\sin\theta$, recovering the supplied trigonometric identity. The formula assumes positive $\Omega_{\Lambda,0}$ and $\Omega_{m,0}$; its zero-vacuum limit is regular even though this parametrization is singular.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

At $z=0$, spatial flatness gives $\tan\theta_0=\sqrt{(1-\Omega_{\Lambda,0})/\Omega_{\Lambda,0}}$, hence $\cos\theta_0=\sqrt{\Omega_{\Lambda,0}}$ and $\sin\theta_0=\sqrt{1-\Omega_{\Lambda,0}}$. Therefore

$$
\boxed{t_0=\frac{2}{3H_0\sqrt{\Omega_{\Lambda,0}}}
\log\left[\frac{1+\sqrt{\Omega_{\Lambda,0}}}
{\sqrt{1-\Omega_{\Lambda,0}}}\right].}
$$

For $\Omega_{\Lambda,0}\to0$, $\operatorname{arsinh}u\sim u$ in the previous integral gives $t_0\to2/(3H_0)$, the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) result. For $\Omega_{m,0}=0$, the positive-vacuum flat slicing has no finite-age [Big Bang](../../../cosmology.md#big-bang), explaining the other endpoint divergence.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $H(a)=H_0a^{-3/2}$, so direct integration of $dt=da/(aH)$ gives $t(a)=2a^{3/2}/(3H_0)$. At $z=8$, $a=1/9$ and $a^{3/2}=1/27$. The fraction of the present [age of an FLRW universe](../../../cosmology.md#age-of-an-flrw-universe) and the available formation interval are therefore

$$
\boxed{\frac{t(8)}{t_0}=\frac1{27}\simeq0.0370,
\qquad t(8)=\frac{2}{81H_0}
=2.47\times10^8h^{-1}\,\mathrm{yr}.}
$$

This is only about $3.7\%$ of the present age. The available interval is $t(8)$ itself, not $t_0-t(8)$, which would instead be the lookback time.

For $\Omega_{m,0}=0.3$ and $\Omega_{\Lambda,0}=0.7$, at the same [Hubble constant](../../../cosmology.md#hubble-constant), the exact integral gives

$$
t(8)=\frac{2}{3H_0\sqrt{0.7}}
\operatorname{arsinh}\!\left(\frac{\sqrt{0.7/0.3}}{27}\right)
\simeq0.04506H_0^{-1}
=4.51\times10^8h^{-1}\,\mathrm{yr}.
$$

Thus **the formation interval is longer, by about a factor of $1.83$**. There is also a direct comparison: for $0<a<1$, $0.3a^{-3}+0.7<a^{-3}$, so $H(a)$ is smaller than its [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) value at fixed $a$, and integrating $da/(aH)$ gives a greater age. At $z=8$ the leading matter-era result is $t\simeq2/[3H_0\sqrt{0.3}(1+z)^{3/2}]$; the smaller matter density, with the same $H_0$, explains nearly all the increase.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The neutral-hydrogen [column density](../../../statistical-physics.md#column-density) is $N_{\rm HI}=\int n_{\rm HI}\,d\ell$, with units $\mathrm{cm}^{-2}$. Define the [neutral-hydrogen column-density distribution](../../../physics.md#neutral-hydrogen-column-density-distribution) by

$$
f(N,z)=\frac{\partial^2\mathcal N}{\partial N\,\partial z},
\qquad d\mathcal N=f(N,z)\,dN\,dz.
$$

Here $\mathcal N$ counts absorption systems along a [quasar](../../../astrophysics.md#quasar) sightline. A histogram per logarithmic column interval instead measures $N\ln(10)f(N,z)$; forgetting this factor changes the inferred slope. Another common convention uses the [absorption distance](../../../physics.md#absorption-distance) $X$, with $dX/dz=H_0(1+z)^2/H(z)$, and $f_X=f/(dX/dz)$.

At a fixed epoch, weak [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) lines have an approximately falling power-law distribution, $f(N,z)\simeq A(z)N^{-\beta}$ with $\beta\simeq1.4$–$1.5$ over representative low-column ranges. Stronger absorbers deviate from one universal slope, and the normalization and fitted slopes depend on epoch and sample. The low-column fit is measured, for example, in [Kim and collaborators' forest survey](https://arxiv.org/abs/astro-ph/0101005). The sketch distinguishes that empirical low-column trend from an illustrative higher-column continuation.

<a id="3/i/image-neutral-hydrogen-column-density-distribution-with-forest-lyman-limit-and-damped-system-thresholds"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-73-column-distribution.png)

**[Figure 1](#3/i/image-neutral-hydrogen-column-density-distribution-with-forest-lyman-limit-and-damped-system-thresholds). Neutral-hydrogen column-density distribution with forest, Lyman-limit and damped-system thresholds**.

Ordinary [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) lines cover roughly $10^{12}\lesssim N_{\rm HI}\lesssim10^{17.2}\,\mathrm{cm}^{-2}$. They are numerous resonant [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption) features from intervening gas at different [cosmological redshifts](../../../cosmology.md#cosmological-redshift), collectively resembling a forest in a [quasar](../../../astrophysics.md#quasar) spectrum. Many are optically thin at the ionization edge even when their line centers are saturated.

A [Lyman limit system](../../../physics.md#lyman-limit-system) becomes optically thick at the $91.2\,\mathrm{nm}$ hydrogen ionization edge. With $\sigma_{912}\simeq6.3\times10^{-18}\,\mathrm{cm}^2$, $\tau_{912}=N_{\rm HI}\sigma_{912}\gtrsim1$ requires

$$
N_{\rm HI}\gtrsim1.6\times10^{17}\,\mathrm{cm}^{-2}\simeq10^{17.2}\,\mathrm{cm}^{-2}.
$$

Its spectrum consequently has a strong continuum decrement below the redshifted Lyman edge. In a classification separating the highest columns, [Lyman limit systems](../../../physics.md#lyman-limit-system) extend up to the damped-system boundary.

A [damped Lyman-alpha system](../../../physics.md#damped-lyman-alpha-system) conventionally has $N_{\rm HI}\gtrsim2\times10^{20}\,\mathrm{cm}^{-2}$. Its [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption) is sufficiently strong that the Lorentzian wings of the [Voigt profile](../../../stellar-astrophysics.md#voigt-profile) are prominent. “Damped” refers to the finite radiative lifetime of the atomic excited state, not an inference that the gas has a high [temperature](../../../thermodynamics.md#temperature). These systems trace substantial neutral reservoirs, usually associated with [galaxies](../../../galaxy.md).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

In the printed convention $\rho$ is energy density, since the gravitational source is $8\pi G\rho/(3c^2)$. For nonrelativistic [pressureless matter](../../../cosmology.md#pressureless-matter), $\rho_m=\rho_{m,0}(1+z)^3$. Define the [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) by

$$
\Omega_{m,0}=\frac{8\pi G\rho_{m,0}}{3c^2H_0^2},
\qquad \Omega_{k,0}=-\frac{kc^2}{a_0^2H_0^2},
\qquad \Omega_{\Lambda,0}=\frac{\Lambda c^2}{3H_0^2}.
$$

The [Friedmann equation](../../../cosmology.md#friedmann-equations) then gives

$$
H(z)=H_0E(z),\qquad E(z)=\sqrt{\Omega_{m,0}(1+z)^3+
\Omega_{k,0}(1+z)^2+\Omega_{\Lambda,0}}.
$$

Let $n_c$ be the constant [comoving number density](../../../cosmology.md#comoving-number-density) of absorbers, and let $\sigma_p$ be their fixed proper interception area. Their proper [number density](../../../statistical-physics.md#number-density) is $n_p(z)=n_c(1+z)^3$, with $a_0=1$. The [redshift-time relation](../../../cosmology.md#redshift-time-relation) gives a local proper photon-path increment

$$
d\ell=c|dt|=\frac{c\,dz}{(1+z)H(z)}.
$$

For an infinitesimal path, the expected number of interceptions, and to first order the probability of an interception, is $d\mathcal N=n_p\sigma_p\,d\ell$. Thus [absorber incidence and comoving number density](../../../physics.md#absorber-incidence-and-comoving-number-density) imply

$$
\boxed{\frac{d\mathcal N}{dz}
=\frac{n_c\sigma_pc}{H_0}\frac{(1+z)^2}{E(z)}.}
$$

Two factors survive: proper density brings three powers of $1+z$, whereas proper path length brings the inverse of one power. A fixed comoving area instead of the assumed fixed proper area would change the result. The formula is an incidence rate, not a probability bounded by one over a finite redshift interval; multiple interceptions can occur.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $E(z)=(1+z)^{3/2}$. Under the non-evolution assumptions of the previous part, the incidence above a fixed neutral-hydrogen [column density](../../../statistical-physics.md#column-density) threshold consequently scales as $(1+z)^{1/2}$. Between the two specified epochs,

$$
\boxed{\frac{[d\mathcal N/dz]_{z=4}}{[d\mathcal N/dz]_{z=1.5}}
=\sqrt{\frac5{2.5}}=\sqrt2\simeq1.41.}
$$

The higher-redshift rate would be about $41\%$ larger.

Observed [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) incidence above substantial column thresholds rises much more rapidly. For example, the survey at [Kim and collaborators' measurements](https://arxiv.org/abs/astro-ph/0101005) finds an exponent $2.19\pm0.27$ for $10^{13.64}\lesssim N_{\rm HI}\lesssim10^{16}\,\mathrm{cm}^{-2}$ over this redshift range, giving a representative increase $2^{2.19}\simeq4.56$, rather than $\sqrt2$. The empirical exponent is threshold dependent. The forest therefore cannot be treated as a conserved population of identical fixed-size neutral clouds: gas expansion, structure evolution and the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background) change neutral fractions, absorption strengths and the effective area above the threshold. In [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium), $n_{\rm HI}\Gamma\simeq\alpha(T)n_en_p$, so changing density or ionization rate changes a counted neutral column even without creating or destroying its baryons.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Use high-resolution [quasar](../../../astrophysics.md#quasar) spectra to fit [Voigt profiles](../../../stellar-astrophysics.md#voigt-profile) to [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) lines near $z=3$, where the transition appears near $121.6(1+3)\simeq486.4\,\mathrm{nm}$. Each fit estimates the neutral-hydrogen [column density](../../../statistical-physics.md#column-density) and the velocity-width parameter $b$. The one-dimensional [Maxwell-Boltzmann velocity distribution](../../../statistical-physics.md#maxwell-boltzmann-velocity-distribution) has variance $k_BT/m_{\rm H}$; consequently the thermal optical-depth profile is proportional to $\exp[-(v-v_0)^2/b^2]$, with the [thermal cutoff of Lyman-alpha line widths](../../../statistical-physics.md#thermal-cutoff-of-lyman-alpha-line-widths)

$$
\boxed{b_{\rm th}^2=\frac{2k_BT}{m_{\rm H}},
\qquad T=\frac{m_{\rm H}b_{\rm th}^2}{2k_B}.}
$$

For example, a purely thermal $b=20\,\mathrm{km\,s^{-1}}$ corresponds to $T\simeq2.4\times10^4\,\mathrm K$.

An observed broad line is not by itself a thermometer: [peculiar velocities](../../../cosmology.md#peculiar-velocity), bulk gradients, blending and instrumental resolution also broaden it. For independent Gaussian contributions, $b^2=b_{\rm th}^2+b_{\rm nonthermal}^2+b_{\rm inst}^2$. After modeling the instrumental response, an uncorrected total width gives an upper bound on the thermal [temperature](../../../thermodynamics.md#temperature), not a lower bound. The narrowest lines at each [column density](../../../statistical-physics.md#column-density) are least affected by additional broadening. Their lower envelope in the $b$–$N_{\rm HI}$ plane constrains the [temperature-density relation of photoionized intergalactic gas](../../../astrophysics.md#temperature-density-relation-of-photoionized-intergalactic-gas), often written $T=T_0(1+\delta)^{\gamma-1}$.

Calibrate the conversion between [column density](../../../statistical-physics.md#column-density), density and width with hydrodynamic models incorporating the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background), pressure smoothing, resolution and selection. It estimates $T_0$ and the slope rather than assigning one [temperature](../../../thermodynamics.md#temperature) to every absorber. Where aligned metal lines trace the same gas, comparing species of different atomic mass can separately estimate a common nonthermal contribution because thermal $b^2$ scales as $m^{-1}$. The forest lower-envelope method and its numerical calibration are developed in [Schaye and collaborators' temperature analysis](https://arxiv.org/abs/astro-ph/9906271).

## 4

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $n_n$ and $n_p$ count the available [neutrons](../../../physics.md#neutron) and [protons](../../../physics.md#proton) immediately before their incorporation into nuclei. In the usual [neutron-limited helium synthesis](../../../cosmology.md#neutron-limited-helium-synthesis) approximation, all surviving neutrons go into ${}^4\mathrm{He}$ and the remaining protons form ${}^1\mathrm H$. Each helium nucleus contains two neutrons and two protons, so

$$
n_{\rm He}=n_n/2,\qquad n_{\rm H}=n_p-n_n.
$$

Using the equal-nucleon-mass approximation and neglecting trace nuclei and binding-energy corrections, the [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) is

$$
\boxed{Y_p=\frac{4n_{\rm He}}{n_{\rm H}+4n_{\rm He}}
=\frac{2n_n}{n_p+n_n}
=2\left(1+\frac{n_p}{n_n}\right)^{-1}.}
$$

The ratio is the pre-assembly nucleon ratio, not the number ratio of free hydrogen nuclei to helium nuclei afterward. The derivation assumes enough protons to bind all the neutrons, as in standard [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis). The familiar $n_p/n_n\simeq7$ gives $Y_p\simeq1/4$ and [hydrogen mass fraction](../../../stellar-astrophysics.md#hydrogen-mass-fraction) $X_p\simeq3/4$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Under the usual interpretation that the extra force simply slows otherwise adiabatic expansion, without changing reaction rates or injecting particles, **the primordial hydrogen mass fraction would be larger**. A smaller [Hubble parameter](../../../cosmology.md#hubble-parameter) makes cooling slower, delays the end of the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck), and permits more [free-neutron decay after freeze-out](../../../cosmology.md#free-neutron-decay-after-freeze-out) before nuclear assembly. If the reduced expansion also keeps weak conversions effective longer, the lower eventual [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out) temperature further reduces the [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio). Both effects lower the [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) and raise the remaining [hydrogen mass fraction](../../../stellar-astrophysics.md#hydrogen-mass-fraction).

For fixed initial neutron fraction $x_{n,1}=n_n/(n_n+n_p)$, the post-freeze-out estimate is $x_n=x_{n,1}e^{-(t_N-t_1)/\tau_n}$, where $t_N$ is the onset of efficient nuclear assembly. Thus $Y_p\simeq2x_n$ decreases when cooling delays $t_N$. The extra time is the time to reach the nuclear-assembly temperature, not an increase in the specified clock interval $300-1$ seconds. An unspecified force that also reheats the plasma, changes weak rates or causes recollapse would require additional information; the simple expansion-only interpretation is essential to this expectation.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/a">a</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#4/iii/a)

A [primordial light-element abundance determination](../../../cosmology.md#primordial-light-element-abundance-determination) seeks gas or stars with little subsequent chemical processing. The three abundances require different observations and corrections.

For helium, measure helium and hydrogen recombination emission in metal-poor extragalactic ionized regions. Correct line ratios for electron [temperature](../../../thermodynamics.md#temperature), density, extinction, collisional excitation, underlying stellar absorption and unobserved ionization stages. Convert the number ratio $y=n_{\rm He}/n_{\rm H}$ to [helium mass fraction](../../../stellar-astrophysics.md#helium-mass-fraction) $Y\simeq4y/(1+4y)$, allowing for heavy elements when necessary. Since [stars](../../../stellar-astrophysics.md#star) produce helium and metals, extrapolate a sample toward zero [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) to infer $Y_p$. The sensitivity to atomic data and these corrections is illustrated by [Peimbert and collaborators' helium determination](https://arxiv.org/abs/astro-ph/0701580).

For deuterium, fit isotope-shifted hydrogen and deuterium [absorption lines](../../../stellar-astrophysics.md#absorption-line) in relatively simple, metal-poor [quasar](../../../astrophysics.md#quasar) absorption systems. The deuterium feature is displaced by about $-82\,\mathrm{km\,s^{-1}}$ from the corresponding hydrogen line. Multiple transitions and velocity components help distinguish deuterium from unrelated hydrogen contamination. The fitted neutral-column ratio estimates D/H in predominantly neutral gas. Since stellar processing destroys deuterium, low-metallicity, minimally processed absorbers are favored; the technique is exemplified by [Pettini and collaborators' deuterium measurement](https://academic.oup.com/mnras/article/391/4/1499/1079236).

For lithium, measure the ${}^7\mathrm{Li}$ absorption feature near $670.8\,\mathrm{nm}$ in warm, old, metal-poor halo stars. Stellar-atmosphere models convert line strength to Li/H. The [Spite plateau](../../../cosmology.md#spite-plateau) supplies a nearly constant low-metallicity level, but [stellar metallicity](../../../galaxy.md#stellar-metallicity) trends, atmospheric temperature scales, departures from local thermal equilibrium and stellar lithium depletion must be considered. Thus the photospheric level is not automatically the initial abundance. [Ryan and collaborators' halo lithium measurements](https://arxiv.org/abs/astro-ph/0010411) illustrate the measured abundance and chemical-evolution corrections.

<h4 id="4/iii/b">b</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#4/iii/b)

In standard [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), with the radiation content and reaction rates fixed, the main adjustable abundance parameter is the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) $\eta$. The [baryon-density consistency between nucleosynthesis and the microwave background](../../../cosmology.md#baryon-density-consistency-between-nucleosynthesis-and-the-microwave-background) uses

$$
\eta_{10}=10^{10}\eta\simeq274\,\Omega_{b,0}h^2,
\qquad H_0=100h\,\mathrm{km\,s^{-1}\,Mpc^{-1}}.
$$

Increasing [cosmological baryon density](../../../cosmology.md#cosmological-baryon-density) makes deuterium burn more efficiently, so D/H falls steeply. The [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction) grows only slowly, because its dominant control is the surviving neutron fraction. Near the observationally favored density, lithium-7 production, much of it initially as beryllium-7, rises with density. At lower densities the full lithium curve has a valley; the sketch focuses on the branch relevant to the baryon-density comparison.

For the historical meaning of “current” in this 2008 paper, representative 2007–2008 fits near $\eta_{10}\simeq6$ are

$$
10^5\mathrm{D/H}\simeq2.68(6/\eta_{10})^{1.6},
\qquad Y_p\simeq0.2483+0.0016(\eta_{10}-6),
\qquad 10^{10}\,{}^7\mathrm{Li/H}\simeq4.30(\eta_{10}/6)^2.
$$

These local fits, with nuclear-rate uncertainties, and representative D/H and lithium ranges are documented in [Steigman's 2007 nucleosynthesis analysis](https://arxiv.org/abs/0712.1100). They are not a replacement for a nuclear network outside their calibrated range.

<a id="4/iii/b/image-2007-2008-primordial-abundance-trends-and-observational-ranges-compared-with-the-wmap-baryon-density"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-73-nucleosynthesis.png)

**[Figure 2](#4/iii/b/image-2007-2008-primordial-abundance-trends-and-observational-ranges-compared-with-the-wmap-baryon-density). 2007–2008 primordial abundance trends and observational ranges compared with the WMAP baryon density**.

The [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) acoustic peak pattern measures baryon loading at recombination, independently of the abundance measurements. For example, [the five-year WMAP cosmological analysis](https://arxiv.org/abs/0803.0547) gives $\Omega_{b,0}h^2=0.02273\pm0.00062$ from WMAP alone, corresponding to $\eta_{10}\simeq6.23\pm0.17$. For $h\simeq0.7$, this is $\Omega_{b,0}\simeq0.046$. Galaxy-cluster baryon fractions combined with independent total-matter density provide another, more astrophysically model-dependent cross-check.

At $\eta_{10}\simeq6.2$, the fitted predictions are D/H $\simeq2.5\times10^{-5}$, $Y_p\simeq0.249$, and ${}^7\mathrm{Li/H}\simeq4.6\times10^{-10}$. A representative observed D/H range around $(2.7\pm0.3)\times10^{-5}$ overlaps the prediction; its inferred density $\eta_{10}\simeq6.0\pm0.4$ is compatible with the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background). The helium result $Y_p=0.2477\pm0.0029$ from [the 2007 helium analysis](https://arxiv.org/abs/astro-ph/0701580) also agrees. Other helium analyses had lower central values, illustrating why ionization and temperature systematics matter.

In contrast, a representative plateau estimate $12+\log_{10}({}^7\mathrm{Li/H})\simeq2.1\pm0.1$ corresponds to roughly $(1.0$–$1.6)\times10^{-10}$, a factor of several below the prediction at the same density. This is the [cosmological lithium problem](../../../cosmology.md#cosmological-lithium-problem). The three abundance ranges therefore should not all be described as exact simultaneous agreement: **deuterium and helium broadly support the independently measured baryon density, while lithium has a substantial discrepancy**. The plotted ranges explicitly refer to the 2007–2008 comparison, not present-day parameter estimates.

<h4 id="4/iii/c">c</h4>

↑ **Parent:** [Iii](#4/iii)

<h5 id="4/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#4/iii/c)

The agreement of the main light-element abundances with a hot early nuclear-burning phase, and the independent [baryon-density consistency between nucleosynthesis and the microwave background](../../../cosmology.md#baryon-density-consistency-between-nucleosynthesis-and-the-microwave-background), gives strong support to the hot [Big Bang](../../../cosmology.md#big-bang) framework. These measurements connect the first minutes to recombination, despite their very different [temperatures](../../../thermodynamics.md#temperature), densities and observables. In particular, the large primordial [helium mass fraction](../../../stellar-astrophysics.md#helium-mass-fraction) and residual deuterium are natural outputs of [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), rather than arbitrary products of subsequent [star formation](../../../stellar-astrophysics.md#star-formation).

The [cosmological lithium problem](../../../cosmology.md#cosmological-lithium-problem) prevents claiming that the simplest abundance calculation explains every observation without qualification. One must distinguish nuclear-rate uncertainties, stellar depletion, atmosphere and abundance systematics, and possible new particle physics. Thus **the broad hot Big Bang framework is strongly supported, while lithium tests the completeness of its simplest nucleosynthesis and stellar-abundance interpretation**. An unresolved lithium discrepancy alone does not erase the independent successes of deuterium, helium and the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
