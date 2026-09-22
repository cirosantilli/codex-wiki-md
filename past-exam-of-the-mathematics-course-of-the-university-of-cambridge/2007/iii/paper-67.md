# Paper 67

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper67.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper67.pdf)

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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A [comoving coordinate](../../../cosmology.md#comoving-coordinate) labels a position relative to the homogeneous expansion. For two nearby comoving positions separated by $\Delta\chi$, their [proper distance in cosmology](../../../cosmology.md#proper-distance-in-cosmology) at time $t$ is $a(t)\Delta\chi$. Thus a fixed comoving separation expands physically with the [scale factor](../../../cosmology.md#scale-factor-cosmology), while a fixed proper separation corresponds to a shrinking comoving separation. Normalize $a_0=1$, so $a(z)=1/(1+z)$.

At a common [cosmological redshift](../../../cosmology.md#cosmological-redshift), a transverse proper size $l$ subtends $\theta\simeq l/D_A$, where $D_A$ is the [angular diameter distance](../../../cosmology.md#angular-diameter-distance). At $z=3$, a $5$ comoving Mpc separation has proper size $5/(1+3)=1.25$ Mpc. Hence

$$
\boxed{\theta_{5\,\mathrm{proper\ Mpc}}=4\,\theta_{5\,\mathrm{comoving\ Mpc}}.}
$$

**The proper-size object has the larger angular size, by a factor of four.** This comparison does not require a numerical [angular diameter distance](../../../cosmology.md#angular-diameter-distance), since it cancels.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Pressureless matter obeys the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation), $\dot\rho_m+3H\rho_m=0$. Integrating gives $\rho_m=\rho_{m,0}(a_0/a)^3$. Define the present [critical density](../../../cosmology.md#critical-density) and [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) by

$$
\rho_{\mathrm{crit},0}=\frac{3H_0^2}{8\pi G},\qquad
\Omega_{m,0}=\frac{\rho_{m,0}}{\rho_{\mathrm{crit},0}},\qquad
\Omega_{\Lambda,0}=\frac{\Lambda}{3H_0^2},\qquad
\Omega_{k,0}=-\frac{k}{H_0^2a_0^2}.
$$

Here $c=1$ and the curvature contribution is an effective density parameter, not an additional matter fluid. Substitution into the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
H^2=H_0^2\left[\Omega_{m,0}\left(\frac{a_0}{a}\right)^3+\Omega_{k,0}\left(\frac{a_0}{a}\right)^2+\Omega_{\Lambda,0}\right].
$$

Using the [Hubble parameter](../../../cosmology.md#hubble-parameter) $H=\dot a/a$ therefore yields

$$
\boxed{\dot a^2=H_0^2\left(\frac{\Omega_{m,0}a_0^3}{a}+\Omega_{k,0}a_0^2+\Omega_{\Lambda,0}a^2\right).}
$$

At $a=a_0$ the same equation implies $\Omega_{m,0}+\Omega_{k,0}+\Omega_{\Lambda,0}=1$. The power in the matter term is $a_0^3$; the converted TeX's $a_0^2$ is an error not present in the original PDF.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

On an expanding branch with $\dot a>0$, minimizing $\dot a$ is equivalent to minimizing its square. Differentiating the preceding [Friedmann equation](../../../cosmology.md#friedmann-equations) with respect to $a$ gives

$$
\frac{d\dot a^2}{da}=H_0^2\left(-\frac{\Omega_{m,0}a_0^3}{a^2}+2\Omega_{\Lambda,0}a\right).
$$

For positive matter density and a positive [cosmological constant](../../../cosmology.md#cosmological-constant), it vanishes uniquely at

$$
\boxed{a_{\min}=a_0\left(\frac{\Omega_{m,0}}{2\Omega_{\Lambda,0}}\right)^{1/3}.}
$$

The second derivative is $H_0^2[2\Omega_{m,0}a_0^3/a^3+2\Omega_{\Lambda,0}]>0$. Thus this is the [minimum expansion speed in a matter-Lambda universe](../../../cosmology.md#minimum-expansion-speed-in-a-matter-lambda-universe). The matter and vacuum densities satisfy $\rho_m=2\rho_\Lambda$ there, precisely the transition from deceleration to acceleration in the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation).

The conclusion concerns an expanding branch that actually reaches this value of $a$. A sufficiently closed model can recollapse before reaching it; positive $\Lambda$ alone does not rule that out. In flat or open models with the stated positive densities the minimum is reached. The degenerate zero-speed limiting case requires separate treatment and does not describe a finite-time passage through a positive-speed minimum.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The stationary-point relation is $\Omega_{m,0}a_0^3/a_{\min}=2\Omega_{\Lambda,0}a_{\min}^2$. Consequently

$$
\dot a_{\min}^2=H_0^2\left(3\Omega_{\Lambda,0}a_{\min}^2+\Omega_{k,0}a_0^2\right).
$$

Taking the positive root on the expanding branch and eliminating $a_0$ with the result of part (iii),

$$
\boxed{\dot a_{\min}=H_0a_{\min}\left[3\Omega_{\Lambda,0}+\Omega_{k,0}\left(\frac{2\Omega_{\Lambda,0}}{\Omega_{m,0}}\right)^{2/3}\right]^{1/2}.}
$$

The bracket must be positive for a genuine passage through this [minimum expansion speed in a matter-Lambda universe](../../../cosmology.md#minimum-expansion-speed-in-a-matter-lambda-universe). Negative values mean that this formal value of the [scale factor](../../../cosmology.md#scale-factor-cosmology) is not accessible on the corresponding physical expanding solution.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

For a spatially flat model, $\Omega_{k,0}=0$, so $\dot a_{\min}^2/a_{\min}^2=3H_0^2\Omega_{\Lambda,0}$. With the squared definition of $E$ used in the paper,

$$
\boxed{E(z_{\min})=\left[\frac{H(z_{\min})}{H_0}\right]^2=3\Omega_{\Lambda,0}.}
$$

Equivalently $1+z_{\min}=a_0/a_{\min}=(2\Omega_{\Lambda,0}/\Omega_{m,0})^{1/3}$, and substitution into $H^2/H_0^2=\Omega_{m,0}(1+z)^3+\Omega_{\Lambda,0}$ gives the same answer. The minimum is in $\dot a$, not in the [Hubble parameter](../../../cosmology.md#hubble-parameter) $H$, which continues to decrease towards $H_0\sqrt{\Omega_{\Lambda,0}}$.

## 2

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

In a spatially flat [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), a radial [null geodesic](../../../special-relativity.md#null-geodesic) satisfies $d\chi=c\,dt/a(t)$. Normalize $a_0=1$. The [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) at time $t$ is therefore $r_h=c\int_0^t dt'/a(t')$, using the initial singularity as the time origin. The [cosmological redshift](../../../cosmology.md#cosmological-redshift) relation $1+z=1/a$ gives

$$
\frac{dz}{dt}=-(1+z)H(z),\qquad \frac{dt}{a(t)}=-\frac{dz}{H(z)}.
$$

For matter and a [cosmological constant](../../../cosmology.md#cosmological-constant) in a spatially flat model, the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $H(z)=H_0[\Omega_{m,0}(1+z)^3+\Omega_{\Lambda,0}]^{1/2}$. The initial singularity corresponds to $z\to\infty$, so reversing the integration limits yields

$$
\boxed{r_h(z)=\frac c{H_0}\int_z^\infty\frac{dz'}{[\Omega_{m,0}(1+z')^3+\Omega_{\Lambda,0}]^{1/2}}.}
$$

This is a [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon), not a distance to the source currently observed at redshift $z$, and not a future-directed [cosmological event horizon](../../../general-relativity.md#cosmological-event-horizon). The corresponding proper horizon radius at that epoch is $r_h(z)/(1+z)$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), the [Hubble parameter](../../../cosmology.md#hubble-parameter) is $H(z)=H_0(1+z)^{3/2}$. The [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) becomes

$$
r_h(z)=\frac c{H_0}\int_z^\infty(1+z')^{-3/2}\,dz'
=\frac c{H_0}\left[-2(1+z')^{-1/2}\right]_z^\infty.
$$

Thus

$$
\boxed{r_h(z)=\frac{2c}{H_0\sqrt{1+z}}.}
$$

It tends to zero towards the initial singularity and increases without bound as $z\to-1$ in the infinite future. At the present time it is $2c/H_0=3ct_0$, since the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) has age $t_0=2/(3H_0)$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Use the stipulated common normalization $A=H_0\Omega_{m,0}$ and plot $R=A r_h/c$. The [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) has $H_{0,E}=A$, whereas the $(\Omega_{m,0},\Omega_{\Lambda,0})=(0.3,0.7)$ model has $H_{0,\Lambda}=A/0.3$. Their [comoving particle horizons](../../../cosmology.md#comoving-particle-horizon) are therefore

$$
R_E(z)=\frac2{\sqrt{1+z}},\qquad
R_\Lambda(z)=0.3\int_z^\infty\frac{dz'}{\sqrt{0.3(1+z')^3+0.7}}.
$$

Both decrease with increasing $z$, or increase with cosmic time. The [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) curve diverges at $z=-1$ and has $R_E(0)=2$, $R_E(2)=2/\sqrt3$. The matter-plus-vacuum curve remains finite at $z=-1$: the integrand approaches a constant there, and its high-redshift tail is integrable. Moreover it lies below the Einstein-de Sitter curve for this particular normalization, since, with $u=1+z'>0$,

$$
\frac{0.3}{\sqrt{0.3u^3+0.7}}<\frac1{u^{3/2}}.
$$

The high-redshift ratio of the two curves tends to $\sqrt{0.3}$, not one. Holding $H_0\sqrt{\Omega_{m,0}}$ fixed would give a different comparison; it is $H_0\Omega_{m,0}$ that the original question specifies.

<a id="2/iii/image-comoving-particle-horizons-with-the-same-value-of-hubble-parameter-times-matter-density-parameter"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-67-horizons.png)

**[Figure 1](#2/iii/image-comoving-particle-horizons-with-the-same-value-of-hubble-parameter-times-matter-density-parameter). Comoving particle horizons with the same value of Hubble parameter times matter density parameter**.

A positive [cosmological constant](../../../cosmology.md#cosmological-constant) eventually makes the [scale factor](../../../cosmology.md#scale-factor-cosmology) grow exponentially. The future integral $\int_t^\infty c\,dt'/a(t')$ then converges, so the remaining [conformal time](../../../cosmology.md#conformal-time) is finite. The [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) approaches a finite limiting visibility radius; it does not shrink. The remaining distance to that limit is the comoving radius of the [cosmological event horizon](../../../general-relativity.md#cosmological-event-horizon). Thus a signal emitted sufficiently far away today can never reach us, even though the proper particle-horizon radius continues to grow. This is the [total conformal lifetime of a flat matter-Lambda universe](../../../cosmology.md#total-conformal-lifetime-of-a-flat-matter-lambda-universe).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Normalize the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe) by $a(t_0)=1$, giving $a(t)=(t/t_0)^{2/3}$. A photon emitted inward today at the current [comoving particle horizon](../../../cosmology.md#comoving-particle-horizon) starts at $\chi_0=3ct_0$. By time $t$ it has traversed the comoving distance

$$
\int_{t_0}^{t}\frac{c\,dt'}{a(t')}=3ct_0\left[\left(\frac{t}{t_0}\right)^{1/3}-1\right].
$$

At arrival at Earth this equals $\chi_0$, hence $(t/t_0)^{1/3}=2$ and

$$
\boxed{t_{\mathrm{arrival}}=8t_0,\qquad t_{\mathrm{travel}}=7t_0.}
$$

The emitting point is at the horizon location today, not a photon already arriving today from the initial singularity. The calculation of [photon arrival from an Einstein-de Sitter particle horizon](../../../cosmology.md#photon-arrival-from-an-einstein-de-sitter-particle-horizon) follows the future inward [null geodesic](../../../special-relativity.md#null-geodesic) from that event.

## 3

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a radial [null geodesic](../../../special-relativity.md#null-geodesic) in a spatially flat universe, the [comoving radial distance](../../../cosmology.md#comoving-radial-distance) increment is $d\chi=c\,dz/H(z)$. If the cloud and [quasar](../../../astrophysics.md#quasar) redshifts differ only slightly, take $H$ at their common approximate epoch $z_*$, giving

$$
\Delta\chi\simeq\frac{c\,\delta z}{H(z_*)},\qquad H(z_*)=H_0\sqrt{\Omega_{m,0}(1+z_*)^3+\Omega_{\Lambda,0}}.
$$

Multiplying by the [scale factor](../../../cosmology.md#scale-factor-cosmology) at that epoch gives the local [proper distance in cosmology](../../../cosmology.md#proper-distance-in-cosmology) relevant to the quasar's radiation flux:

$$
\boxed{d_{cq}\simeq\frac{c\,\delta z}{H_0(1+z_*)\sqrt{\Omega_{m,0}(1+z_*)^3+\Omega_{\Lambda,0}}}.}
$$

If distance is instead expressed in comoving units, it is $(1+z_*)d_{cq}$. Equivalently the small rest-frame velocity difference is $\delta v=c\,\delta z/(1+z_*)$, and $d_{cq}\simeq\delta v/H(z_*)$. This [quasar-cloud redshift separation](../../../cosmology.md#quasar-cloud-redshift-separation) assumes the redshift difference is due to homogeneous expansion, with negligible [peculiar velocities](../../../cosmology.md#peculiar-velocity). Since the two observations lie on a light cone, the proper separation is understood as the short separation on a nearly common cosmic-time slice; specifying the epoch matters at higher order.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $H(z)=100h(1+z)^{3/2}\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$. At the cloud's approximate epoch $z_*=3$, $H=800h\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$, and $\delta z=0.1$ corresponds to $\delta v\simeq7500\,\mathrm{km\,s^{-1}}$. Therefore

$$
\boxed{d_{cq}\simeq9.4\,h^{-1}\mathrm{Mpc}\quad\text{proper},\qquad \Delta\chi\simeq37.5\,h^{-1}\mathrm{Mpc}\quad\text{comoving}.}
$$

Choosing the midpoint $z_*=3.05$ instead gives $9.1\,h^{-1}\mathrm{Mpc}$ proper. Thus the intended approximate proper distance is about **$9\,h^{-1}\mathrm{Mpc}$**; the small variation reflects the epoch choice in the local expansion, not a factor-of-four physical discrepancy. For example the exact comoving separation is $2cH_0^{-1}[(1+z_c)^{-1/2}-(1+z_q)^{-1/2}]$, whose conversion at the midpoint agrees with that estimate.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

At the same accuracy as the small-separation conversion, its coefficient is fixed at the cloud's well-determined epoch. Since $d_{cq}$ is proportional to $\delta z=z_q-z_c$ and $\Delta z_c$ is negligible,

$$
\frac{\Delta d_{cq}}{d_{cq}}\simeq\frac{\Delta(\delta z)}{\delta z}\simeq\frac{\Delta z_q}{0.1}.
$$

The given emission-redshift error corresponds near $z=3$ to $\Delta z_q\simeq(1+z)1000/c\simeq0.0133$. Hence

$$
\boxed{\frac{\Delta d_{cq}}{d_{cq}}\simeq\pm0.13\quad\text{or about }\pm13\%.}
$$

The uncertainty is about $1.2\,h^{-1}\mathrm{Mpc}$ in proper distance. Using $1+z_q=4.1$ instead changes the percentage only to $13.7\%$. More precise propagation would also specify the reference epoch and its change in the [Hubble parameter](../../../cosmology.md#hubble-parameter); these are higher-order details of the approximate [quasar-cloud redshift separation](../../../cosmology.md#quasar-cloud-redshift-separation).

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The [Lyman-alpha forest](../../../astrophysics.md#lyman-alpha-forest) is the multitude of [Lyman-alpha absorption](../../../physics.md#lyman-alpha-absorption) lines blueward of the broad emission line in a distant [quasar](../../../astrophysics.md#quasar) spectrum. Neutral hydrogen along the line of sight absorbs at its rest wavelength $\lambda_\alpha\simeq1216\,\mathrm{\mathring A}$, so each absorber appears at $\lambda_{\rm obs}=(1+z_c)\lambda_\alpha$. Much of the ordinary forest traces modest overdensities in the mostly ionized [intergalactic medium](../../../astrophysics.md#intergalactic-medium), rather than compact objects made primarily of neutral gas. Strong self-shielded systems form a distinct absorption regime. Line strengths constrain neutral-hydrogen [column density](../../../statistical-physics.md#column-density), while line widths contain thermal and velocity information.

The [redshift evolution of the Lyman-alpha forest](../../../astrophysics.md#redshift-evolution-of-the-lyman-alpha-forest) is normally described, for a fixed line selection, by an incidence $d\mathcal N/dz=A(1+z)^\gamma$. At redshifts of a few the line incidence and mean absorption increase rapidly with redshift; typical selected populations have $\gamma$ of order $2$–$3$, not a universal exponent. Low-redshift evolution is appreciably flatter. Geometry alone cannot explain the full change: for a fixed comoving abundance and fixed proper cross section one obtains $d\mathcal N/dz\propto(1+z)^2/H(z)$, only $(1+z)^{1/2}$ in matter domination. Density evolution, thermal evolution and the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background) change how many structures exceed the chosen absorption threshold. In optically thin [photoionization equilibrium](../../../galaxy.md#photoionization-equilibrium),

$$
n_{\rm HI}\Gamma_{\rm HI}=n_en_p\alpha(T),
$$

so for roughly fixed overdensity the rising cosmic density alone makes $n_{\rm HI}$ scale approximately as $\alpha(T)(1+z)^6/\Gamma_{\rm HI}$. At low redshift, the declining ionizing radiation partly offsets the decrease in gas density. Near the end of [reionization](../../../cosmology.md#reionization) the forest becomes very opaque and the simple individual-line description ceases to suffice.

The [quasar proximity effect](../../../astrophysics.md#proximity-effect-astrophysics) is the statistically reduced absorption near the quasar's own redshift, contrary to the general increase of absorption towards higher redshift. It results from additional ionizing radiation from the nearby quasar. At fixed density and temperature the local [photoionization rate](../../../physics.md#photoionization-rate) becomes $\Gamma_{\rm bg}+\Gamma_Q$. Accordingly

$$
N_{\rm HI}=\frac{N_{\rm HI}^{(0)}}{1+\omega},\qquad\omega=\frac{\Gamma_Q}{\Gamma_{\rm bg}},
$$

where $N_{\rm HI}^{(0)}$ is the value with the background alone. Lines weaken and some fall below the detection threshold; the absorbers need not have been physically removed. This gives the [proximity-effect estimator of the ionizing background](../../../astrophysics.md#proximity-effect-estimator-of-the-ionizing-background).

For an approximately isotropic quasar and a nearby cloud at proper distance $d$, calculate its flux from $F_{\nu,Q}\simeq L_{\nu,Q}/(4\pi d^2)$, allowing for absorption and relative redshift if necessary. The quasar and isotropic background ionization rates are

$$
\Gamma_Q=\int_{\nu_0}^\infty\frac{F_{\nu,Q}\sigma_{\rm HI}(\nu)}{h_P\nu}\,d\nu,\qquad
\Gamma_{\rm bg}=4\pi\int_{\nu_0}^\infty\frac{J_\nu\sigma_{\rm HI}(\nu)}{h_P\nu}\,d\nu,
$$

where $\nu_0$ is the hydrogen ionization threshold, $h_P$ is the [Planck constant](../../../quantum-mechanics.md#planck-constant) and $J_\nu$ is the background [specific intensity](../../../astrophysics.md#specific-intensity). Establish the ordinary absorption statistics far from quasars, then fit their reduction as a function of distance and known quasar luminosity. The scale at which $\omega\sim1$ gives the background rate; an assumed spectral shape converts this to an intensity near the ionization threshold. For matching spectral shapes, $\omega\simeq L_{\nu_0,Q}/(16\pi^2d^2J_{\nu_0})$. A column-density distribution proportional to $N^{-p}$ gives a line-incidence suppression $(1+\omega)^{1-p}$ above a fixed threshold, by shifting that threshold to $(1+\omega)N_{\min}$ in the unperturbed distribution. This is the physical measurement principle established in [https://adsabs.harvard.edu/pdf/1988ApJ...327..570B](https://adsabs.harvard.edu/pdf/1988ApJ...327..570B) .

The inference is statistical. Quasars live in overdense environments, which enhance absorption and can mask extra ionization. Emission-redshift errors smear the effect, as part (iii) demonstrates. Finite source lifetimes, anisotropic emission, variability and departures from ionization equilibrium can also alter the radial profile. These effects must be modeled rather than attributed entirely to the [cosmic ionizing background](../../../astrophysics.md#cosmic-ionizing-background).

The background is produced mainly by ionizing radiation from accretion-powered [quasars](../../../astrophysics.md#quasar) and hot massive stars in star-forming [galaxies](../../../galaxy.md). Their relative importance changes with redshift. Quasars have hard spectra and can ionize helium as well as hydrogen; stellar photons depend strongly on their [ionizing photon escape fraction](../../../galaxy.md#ionizing-photon-escape-fraction) from galaxies. Integrating source luminosities over the [luminosity function](../../../astrophysics.md#luminosity-function-astronomy) and propagating radiation through absorbing gas gives the background. At high redshift the observed quasar population alone need not supply the required hydrogen ionization, so star-forming galaxies can be essential, as discussed in [https://arxiv.org/abs/0807.4177](https://arxiv.org/abs/0807.4177) . Diffuse recombination radiation can contribute, but a residual primordial radiation field is not an adequate ionizing source.

## 4

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A complete [Einstein ring](../../../general-relativity.md#einstein-ring) requires an axisymmetric [gravitational lens](../../../general-relativity.md#gravitational-lens) and exact alignment of the source with the lens centre and observer: $\beta=0$. A finite aligned circular source gives a ring of finite width. The background source must lie behind the lens, so the lensing distance factor is positive.

With $\beta=0$ the [thin gravitational lens equation](../../../general-relativity.md#thin-gravitational-lens-equation) gives

$$
\boxed{\theta_E^2=\frac{4G}{c^2}\frac{D_{ds}}{D_sD_d}\,M(<D_d\theta_E).}
$$

The [Einstein radius](../../../general-relativity.md#einstein-radius) here is angular, and the mass is projected inside the corresponding aperture. For an extended mass distribution the equation is implicit because the enclosed mass depends on $\theta_E$.

Using the supplied approximations, $D_{ds}/(D_sD_d)=1/(3\times10^{25}\,\mathrm m)$ and $\theta_E=3\times10^{-4}$, the inferred mass is

$$
M=\frac{\theta_E^2c^2}{4G}\frac{D_sD_d}{D_{ds}}
=\frac{(3\times10^{-4})^2(3\times10^8)^2(3\times10^{25})}{4(7\times10^{-11})}\,\mathrm{kg}
\simeq8.7\times10^{44}\,\mathrm{kg}.
$$

Thus

$$
\boxed{M(<\theta_E)\simeq4.3\times10^{14}M_\odot.}
$$

This measures the projected aperture mass without requiring the [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere) model used subsequently.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For the [singular isothermal sphere](../../../galaxy.md#singular-isothermal-sphere), integrate its [projected surface mass density](../../../fluid-mechanics.md#projected-surface-mass-density) inside a circle of proper radius $\xi$:

$$
M_{\rm proj}(<\xi)=2\pi\int_0^\xi\frac{\sigma^2}{2G\xi'}\xi'\,d\xi'
=\frac{\pi\sigma^2\xi}{G}.
$$

With $\xi=D_d\theta$ this gives the reduced deflection magnitude

$$
\frac{D_{ds}}{D_sD_d}\frac{4GM_{\rm proj}(<D_d\theta)}{c^2\theta}
=4\pi\frac{\sigma^2}{c^2}\frac{D_{ds}}{D_s},
$$

independent of $\theta$. Hence the [singular isothermal sphere lens](../../../galaxy.md#singular-isothermal-sphere-lens) has

$$
\boxed{\theta_E=4\pi\left(\frac\sigma c\right)^2\frac{D_{ds}}{D_s}.}
$$

The spherical three-dimensional mass $2\sigma^2r/G$ would give the wrong coefficient here; the [thin gravitational lens equation](../../../general-relativity.md#thin-gravitational-lens-equation) needs the projected cylindrical mass.

Using the same $\theta_E=3\times10^{-4}$ and $D_{ds}/D_s=0.5$, the one-dimensional [velocity dispersion](../../../galaxy.md#velocity-dispersion) is

$$
\sigma=c\sqrt{\frac{\theta_E}{4\pi(D_{ds}/D_s)}}
=3\times10^8\sqrt{\frac{3\times10^{-4}}{2\pi}}\,\mathrm{m\,s^{-1}}
\simeq2.1\times10^6\,\mathrm{m\,s^{-1}}.
$$

Thus **$\sigma\simeq2100\,\mathrm{km\,s^{-1}}$** within the idealized [SIS](../../../galaxy.md#singular-isothermal-sphere) model.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Choose a signed angular coordinate along the source-lens line. The [singular isothermal sphere lens](../../../galaxy.md#singular-isothermal-sphere-lens) equation is

$$
\beta=\theta-\theta_E\operatorname{sgn}\theta.
$$

For $\beta>0$, the positive image is $\theta_+=\beta+\theta_E$. A negative image would require $\theta_-=\beta-\theta_E<0$, which is possible only for $\beta<\theta_E$. Here $\beta=4$ arcmin and $\theta_E=1$ arcmin, so **there is only one image, at $\theta=5$ arcmin**. Formally using the negative-image formula would produce a positive value, inconsistent with the branch from which it was obtained.

The paper defines its vector deflection as source minus image angle, $\boldsymbol\alpha_{\rm paper}=(\beta-\theta)\hat{\boldsymbol\theta}$. This is the negative of the usual reduced deflection in $\boldsymbol\beta=\boldsymbol\theta-\boldsymbol\alpha_{\rm standard}$. Therefore its relation to [lensing convergence](../../../general-relativity.md#lensing-convergence) is

$$
\boxed{\kappa=-\frac12\nabla_\theta\cdot\boldsymbol\alpha_{\rm paper}.}
$$

For the [SIS](../../../galaxy.md#singular-isothermal-sphere), $\boldsymbol\alpha_{\rm paper}=-\theta_E\hat{\boldsymbol\theta}$. The two-dimensional polar-coordinate divergence gives

$$
\nabla_\theta\cdot\boldsymbol\alpha_{\rm paper}
=\frac1\theta\frac{d}{d\theta}(-\theta_E\theta)=-\frac{\theta_E}{\theta},
\qquad \boxed{\kappa=\frac{\theta_E}{2\theta}.}
$$

Using a plus sign with the printed inward deflection would incorrectly give negative convergence.

For a small intrinsically circular source, differentiate the [thin gravitational lens equation](../../../general-relativity.md#thin-gravitational-lens-equation). The radial and tangential source-image [Jacobian matrix](../../../calculus.md#jacobian-matrix) eigenvalues are

$$
\lambda_r=1,\qquad \lambda_t=1-\frac{\theta_E}{\theta}.
$$

Thus the image is stretched tangentially around the lens centre, with no radial stretch in this idealized model. At $\theta=5$ arcmin, $\lambda_t=4/5$; the image is an ellipse with tangential-to-radial axis ratio $5/4$. It is not a complete ring. This local description assumes a source small enough that the Jacobian is nearly constant across it.

The signed [lensing magnification](../../../general-relativity.md#lensing-magnification) is

$$
\mu=\frac1{(1-\kappa)^2-|\gamma|^2}.
$$

Since the [lensing shear](../../../general-relativity.md#lensing-shear) magnitude equals $\kappa$, it reduces to $\mu=(1-2\kappa)^{-1}$. At the image, $\kappa=\theta_E/(2\theta)=1/10$, hence

$$
\boxed{\mu=\frac1{1-1/5}=\frac54=1.25.}
$$

The image has positive parity and is $25\%$ brighter for the same intrinsic source. [Gravitational lensing](../../../general-relativity.md#gravitational-lensing) preserves [surface brightness](../../../astrophysics.md#surface-brightness), so this flux amplification follows from its larger apparent solid angle. In evaluating the convergence, use the image angle $5$ arcmin, not the source angle $4$ arcmin.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

[Cosmic shear](../../../general-relativity.md#cosmic-shear) is the small, statistically correlated distortion of distant galaxy images by [weak gravitational lensing](../../../general-relativity.md#weak-gravitational-lensing) from intervening large-scale matter inhomogeneities. An individual galaxy has an unknown intrinsic shape, so the signal is measured through ensemble shape correlations rather than by assuming every source is circular. The angular and redshift dependence of these correlations probes the projected matter fluctuations, their growth and the [angular diameter distance](../../../cosmology.md#angular-diameter-distance) relation, constraining [dark matter](../../../cosmology.md#dark-matter), [cosmological density parameters](../../../cosmology.md#cosmological-density-parameter) and [dark energy](../../../cosmology.md#dark-energy). [Gravitational lensing](../../../general-relativity.md#gravitational-lensing) responds to all gravitating matter rather than just luminous tracers. Intrinsic alignments and shape-measurement biases must be modeled separately from the lensing signal; the physical and statistical basis is described in [https://arxiv.org/abs/1411.0115](https://arxiv.org/abs/1411.0115) .

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
