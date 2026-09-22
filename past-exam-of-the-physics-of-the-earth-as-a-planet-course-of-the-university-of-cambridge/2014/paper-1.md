# Paper 1

↑ **Parent:** [2014](../2014.md)

[Original public PDF, physical pages 643–646; examination dated 15 January 2014](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=643)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [hypocentre](../../geophysics.md#hypocenter) is the point where rupture begins. The [epicentre](../../geophysics.md#epicenter) is its projection onto the [Earth](../../planetary-science.md#earth)'s surface. An [earthquake centroid](../../geophysics.md#earthquake-centroid) is an effective spatial average of moment release over the rupture, with a corresponding mean release time. **Initiation and average release need not occur at the same place or time**, especially for an extended, asymmetric rupture.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Identify the event and pick calibrated [P wave](../../wave-equation.md#p-wave) and, where available, [S wave](../../wave-equation.md#s-wave) arrivals at stations of known position. Associate each pick with a [seismic phase](../../geophysics.md#seismic-phase) and uncertainty. An [earthquake location by arrival times](../../geophysics.md#earthquake-location-by-arrival-times) fits

$$
t_i^{\rm obs}=t_0+T_i(\mathbf x)+\epsilon_i
$$

for the three [hypocentre](../../geophysics.md#hypocenter) coordinates and [earthquake origin time](../../geophysics.md#earthquake-origin-time), using [travel times](../../dispersion-relation.md#travel-time) from a specified [velocity](../../classical-mechanics.md#velocity) model. A grid search can initialize iterative [weighted least squares](../../normal-linear-model.md#weighted-least-squares) or a probabilistic inversion. Station coverage must constrain depth as well as horizontal position; merely having four observations does not ensure a well-conditioned solution.

Errors include uncertain or misidentified onsets, clock and station-coordinate errors, wrong velocities or neglected three-dimensional structure, poor azimuthal coverage, inadequate station distances and depth–origin-time tradeoffs. Examine residual patterns and resolution, not only the minimum residual. A small formal [covariance](../../variance.md#covariance) within a wrong [velocity](../../classical-mechanics.md#velocity) model can accompany a systematically biased [hypocentre](../../geophysics.md#hypocenter).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a [double-couple seismic source](../../wave-equation.md#double-couple-seismic-source), measure [P-wave first-motion polarity](../../wave-equation.md#p-wave-first-motion-polarity) signs and use source-to-station takeoff angles from the location and [velocity](../../classical-mechanics.md#velocity) model to plot them on a [focal sphere](../../wave-equation.md#focal-sphere). Fit the alternating radiation-sign quadrants, optionally adding amplitude ratios and waveform information. The two nodal planes determine a [focal mechanism](../../wave-equation.md#focal-mechanism), conventionally expressed by [fault strike](../../geophysics.md#fault-strike), [fault dip](../../geophysics.md#fault-dip) and [fault rake](../../geophysics.md#fault-rake).

A more general waveform inversion fits a [seismic moment tensor](../../wave-equation.md#seismic-moment-tensor) to several components and stations. Its double-couple part supplies candidate slip and normal [vectors](../../vector-space.md#vector), but a general moment [tensor](../../multilinear-algebra.md#tensor) should not be forced to be double-couple without justification. Polarity calibration, near-nodal observations, path effects and takeoff-angle errors limit the result.

**Point-source radiation alone interchanges the [fault plane](../../geophysics.md#fault-plane) and auxiliary plane without changing the double couple.** Resolve this [fault-plane ambiguity](../../wave-equation.md#fault-plane-ambiguity) using mapped rupture, aftershock geometry, [geodesy](../../geophysics.md#geodesy) or finite-rupture directivity. A dense set of polarity picks does not by itself remove that fundamental ambiguity.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Linearized arrivals contain $\delta t_i=\delta t_0+(\partial T_i/\partial z)\delta z+\cdots$. When the stations have similar depth sensitivities, a depth change shifts nearly all predicted times together and an origin-time change compensates it. Distant stations can also have very weak depth sensitivity. **Improve the range of takeoff angles and station distances**, especially with nearby or borehole stations, and include S–P or depth-phase differences such as pP–P that cancel origin time while retaining depth information. Accurate phase identification and the [velocity](../../classical-mechanics.md#velocity) model remain necessary.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Nearby events observed at the same station share most of their propagation path, so common model and station errors cancel in differential arrival times. Waveform [cross-correlation](../../fourier-analysis.md#cross-correlation) can also determine their relative timing more precisely than separate onset picks. [Double-difference earthquake relocation](../../geophysics.md#double-difference-earthquake-relocation) fits

$$
(t_{ik}-t_{jk})_{\rm obs}-[T_k(\mathbf x_i)-T_k(\mathbf x_j)]
$$

along with the difference in origin times. **The relative cluster geometry can be precise while the entire cluster remains displaced.** Absolute anchoring still needs a well-calibrated [velocity](../../classical-mechanics.md#velocity) model or a source of known position.[2000, method and common-path rationale](../../physics-bibliography.md#a-double-difference-earthquake-location-algorithm-method-and-application-to-the-northern-hayward-fault-california-by-f-waldhauser-and-w-ellsworth)

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Let the [seismic moment tensor](../../wave-equation.md#seismic-moment-tensor) of a [double-couple seismic source](../../wave-equation.md#double-couple-seismic-source) be $M=M_0(\mathbf s\otimes\mathbf n+\mathbf n\otimes\mathbf s)$ for perpendicular unit slip and normal [vectors](../../vector-space.md#vector). Its T axis is $\mathbf T=(\mathbf s+\mathbf n)/\sqrt2$, with [eigenvalue](../../linear-operator-theory.md#eigenvalue) $+M_0$, and its P axis is $\mathbf P=(\mathbf s-\mathbf n)/\sqrt2$, with [eigenvalue](../../linear-operator-theory.md#eigenvalue) $-M_0$. They bisect the fault-plane and auxiliary-plane quadrants.

These [earthquake pressure and tension axes](../../wave-equation.md#earthquake-pressure-and-tension-axes) describe the source deformation. **They are not generally the [principal axes](../../rigid-body-dynamics.md#principal-axis) of the ambient [stress tensor](../../continuum-mechanics.md#cauchy-stress-tensor).** [Friction](../../newtonian-mechanics.md#friction), inherited fault orientation and local [stress](../../continuum-mechanics.md#stress) changes can rotate their relationship to that [tensor](../../multilinear-algebra.md#tensor); a [stress](../../continuum-mechanics.md#stress) inversion requires further assumptions and multiple mechanisms.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

A dense array does not correct an incorrect [velocity](../../classical-mechanics.md#velocity) model. The faster southwest block permits shorter [travel times](../../dispersion-relation.md#travel-time) than an assumed uniform medium, with [refraction](../../optics.md#refraction) favouring paths through fast rock. First arrivals may include refracted or [seismic head wave](../../wave-equation.md#seismic-head-wave) paths rather than the assumed direct straight paths. Fitting those arrivals with one constant [speed](../../classical-mechanics.md#speed) can make an [earthquake](../../geophysics.md#earthquake) on the fault appear closer to southwest stations and farther from northeast stations.

The sign follows even from a two-station [linearization](../../algebra.md#linearization). Put southwest and northeast stations at $x=-L,+L$, and the true event at $x=0$ with depth $h$. In a constant-speed model,

$$
\delta(t_{\rm SW}-t_{\rm NE})
\simeq\frac{2L}{v\sqrt{L^2+h^2}}\,\delta x.
$$

A negative observed differential residual therefore produces **$\delta x<0$, an apparent southwest displacement**. A common origin-time adjustment cannot remove this directional residual. The stated kilometre-scale offset is a model bias, not proof that the fault dips towards the apparent [epicentres](../../geophysics.md#epicenter). Its exact magnitude cannot be predicted without the actual velocities and station geometry; the question supplies that magnitude as an observation.

The relevant contrast is independently documented at Parkfield: higher velocities lie southwest of the fault, with lower velocities northeast.[Velocity-structure discussion, higher speeds southwest and lower speeds northeast](../../physics-bibliography.md#scientific-advances-at-parkfield-by-united-states-geological-survey) Account for the lateral structure and correct phases, then relocate and test whether the bias remains.

<a id="1/g/image-illustrative-velocity-contrast-and-the-direction-of-a-constant-speed-location-bias"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2014/paper-1-pep-location-bias.png)

**[Figure 1](#1/g/image-illustrative-velocity-contrast-and-the-direction-of-a-constant-speed-location-bias). Illustrative velocity contrast and the direction of a constant-speed location bias**.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Ice accumulation adds a load that produces an immediate elastic response and slower viscous displacement of the [mantle](../../geophysics.md#planetary-mantle) away from the loaded region. The depressed interior may be accompanied by a peripheral forebulge. A long-lived load approaches an approximately compensated state. Melting removes the load, giving rapid elastic recovery followed by [mantle](../../geophysics.md#planetary-mantle) return flow and gradual uplift. The forebulge can subside while the formerly loaded centre rises.

**[Postglacial rebound](../../geophysics.md#postglacial-rebound) can continue long after the ice disappears**, because [mantle](../../geophysics.md#planetary-mantle) relaxation is slow. Raised shorelines, changing relative sea level, vertical geodetic motion and [gravity](../../physics.md#gravity) changes record [glacial isostatic adjustment](../../geophysics.md#glacial-isostatic-adjustment). Present motion depends on the whole loading and melting history, [mantle](../../geophysics.md#planetary-mantle) rheology and lithospheric stiffness, not only the current absence of ice.

<a id="2/image-ice-loading-mantle-displacement-and-continuing-rebound-after-melting-schematic-stages"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2014/paper-1-pep-glacial-rebound.png)

**[Figure 2](#2/image-ice-loading-mantle-displacement-and-continuing-rebound-after-melting-schematic-stages). Ice loading, mantle displacement and continuing rebound after melting; schematic stages**.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Subtract the background [hydrostatic pressure](../../fluid-mechanics.md#hydrostatic-pressure). A relief amplitude $h$ produces a restoring [pressure](../../pressure.md) perturbation $p'\sim\rho gh$ and horizontal [gradient](../../multivariable-calculus.md#gradient) $\rho gh/\lambda$. [Incompressibility](../../fluid-mechanics.md#incompressible-flow) makes the disturbance penetrate a depth of order its horizontal scale. For [sinusoidal viscous rebound](../../geophysics.md#sinusoidal-viscous-rebound), with relaxation [speed](../../classical-mechanics.md#speed) $v\sim h/\tau$, the viscous [force density](../../force.md#force-density) is $\eta v/\lambda^2$. Balancing gives

$$
\eta\frac{h}{\tau\lambda^2}\sim\frac{\rho gh}{\lambda},
\qquad\boxed{\tau\sim\frac{\eta}{\rho g\lambda}.}
$$

This is a small-amplitude viscous half-space estimate; numerical factors from the sinusoidal geometry are absent from a scaling argument.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Unsteady inertial [force density](../../force.md#force-density) scales as $\rho v/\tau$, whereas viscous [force density](../../force.md#force-density) scales as $\eta v/\lambda^2$. Using the preceding timescale gives

$$
\boxed{\frac{\text{unsteady inertia}}{\text{viscosity}}
\sim\frac{\rho\lambda^2}{\eta\tau}
\sim\frac{\rho^2g\lambda^3}{\eta^2}.}
$$

Convective [inertia](../../classical-mechanics.md#inertia) has ratio $\rho v\lambda/\eta$. Since $v\sim h/\tau$, this is smaller by $h/\lambda$ for small relief. Thus the displayed estimate controls the larger inertial contribution in this model.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Assume the original ice sheet had time to reach local isostatic compensation, melted rapidly relative to subsequent rebound, and left one exponentially relaxing depression mode. Neglect elastic layering and assign the whole present [gravity](../../physics.md#gravity) deficit to that unrelaxed depression. Load balance gives

$$
h_0\simeq\frac{\rho_i}{\rho_m}H_i=900\,\mathrm m.
$$

The supplied sheet-gravity approximation gives the residual amplitude

$$
h(t)=\frac{|\Delta g|}{2\pi G\rho_m}
=\frac{2.0\times10^{-4}}{2\pi(6.67\times10^{-11})(3000)}
\simeq159\,\mathrm m.
$$

From $h(t)=h_0e^{-t/\tau}$,

$$
\boxed{\tau=\frac{10^4\,\mathrm{yr}}{\ln(900/159)}
\simeq5.77\times10^3\,\mathrm{yr}.}
$$

For an order-of-magnitude single-mode estimate, choose the ice-sheet diameter as [wavelength](../../wave-equation.md#wavelength), $\lambda\simeq2R=6000\,\mathrm{km}$. Taking $g=9.81\,\mathrm{m\,s^{-2}}$, the more accurate specified relation then gives

$$
\boxed{\eta=\frac{\rho_mg\lambda\tau}{4\pi}
\simeq2.6\times10^{21}\,\mathrm{Pa\,s}.}
$$

A circular load has a spectrum, not one uniquely specified [wavelength](../../wave-equation.md#wavelength). Choosing $\lambda\sim R$ instead gives about $1.3\times10^{21}\,\mathrm{Pa\,s}$; another [wavelength](../../wave-equation.md#wavelength) convention rescales the answer linearly. **The robust inference is [viscosity](../../dynamic-viscosity.md) of order $10^{21}\,\mathrm{Pa\,s}$ within this simple model.** A realistic estimate would also model gradual melting, other [gravity](../../physics.md#gravity) anomalies, [density](../../fluid-mechanics.md#density) interfaces, [lithospheric flexure](../../geophysics.md#lithospheric-flexure) and depth-dependent [mantle viscosity](../../planetary-science.md#mantle-viscosity).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Using the same diameter convention and [viscosity](../../dynamic-viscosity.md) estimate,

$$
\boxed{\frac{\rho^2g\lambda^3}{\eta^2}
\simeq\frac{(3000)^2(9.81)(6.0\times10^6)^3}
{(2.56\times10^{21})^2}
\simeq2.9\times10^{-15}.}
$$

Geometrical factors omitted in the scaling do not affect the conclusion: **[inertia](../../classical-mechanics.md#inertia) is negligible**. Convective [inertia](../../classical-mechanics.md#inertia) is smaller still by the small relief-to-wavelength ratio. [Mantle](../../geophysics.md#planetary-mantle) creep is extremely slow despite the large length scale.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

**[Elastic rebound](../../geophysics.md#elastic-rebound-model).** Tectonic motion loads a fault whose shallow portion is locked. Rock on either side deforms and stores elastic [strain](../../continuum-mechanics.md#strain) [energy](../../energy.md) while slip is inhibited. When failure permits rapid slip, part of the stored [energy](../../energy.md) becomes seismic radiation and part is dissipated in [friction](../../newtonian-mechanics.md#friction) and damage. The adjacent rock partly relaxes, while a permanent displacement remains across the fault. Geodetic [strain](../../continuum-mechanics.md#strain) accumulation and coseismic offsets support this loading–release picture.[Explanation of accumulated elastic strain, release and permanent fault offset](../../physics-bibliography.md#reid-s-elastic-rebound-theory-by-united-states-geological-survey)

The model is useful for brittle crustal faulting but is not a prediction of precise recurrence, rupture size or frictional evolution. Aseismic creep can release deformation without a large sudden event. Viscoelastic flow, afterslip, fluid-pressure changes and interacting fault segments complicate a simple locked-fault cycle. Deep-focus [earthquakes](../../geophysics.md#earthquake) and non-shear source components require additional physics; not every [earthquake](../../geophysics.md#earthquake) source is adequately described by a shallow brittle double couple. Rebound also need not release all the pre-existing [stress](../../continuum-mechanics.md#stress).

<a id="3/a/image-original-displacement-profile-schematic-of-locked-loading-and-permanent-slip-after-relaxation"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2014/paper-1-pep-elastic-rebound.png)

**[Figure 3](#3/a/image-original-displacement-profile-schematic-of-locked-loading-and-permanent-slip-after-relaxation). Original displacement-profile schematic of locked loading and permanent slip after relaxation**.

**A thin negative-gradient [velocity](../../classical-mechanics.md#velocity) zone.** In horizontal layering, use the [seismic ray parameter](../../geophysics.md#seismic-ray-parameter-in-horizontal-layering) $p=\sin i/v$, the conserved horizontal [slowness](../../wave-equation.md#slowness). A ray turns when $pv=1$. Downward passage through decreasing [speed](../../classical-mechanics.md#speed) makes $pv$ smaller, so a surface ray cannot turn in the negative-gradient interior. Rays either turn above the zone or penetrate it and turn below where [speed](../../classical-mechanics.md#speed) has recovered sufficiently. This produces missing turning depths and a [seismic shadow range from a low-velocity zone](../../geophysics.md#seismic-shadow-range-from-a-low-velocity-zone) in the ideal ray model.

Retain all branches using

$$
x(p)=2\int_0^{z_t}\frac{pv(z)}{\sqrt{1-p^2v(z)^2}}\,dz,
\qquad
T(p)=2\int_0^{z_t}\frac{dz}{v(z)\sqrt{1-p^2v(z)^2}}.
$$

The travel-time slope is $dT/dx=p$. Just below the critical value that permits passage beyond the upper [speed](../../classical-mechanics.md#speed) maximum, the ray makes a finite extra excursion through the low-velocity region. Range can jump, and the deep branch can fold back before resuming its normal trend, giving multiple arrivals outside the shadow. A first-arrival curve alone hides some of these branches. Define the [seismic intercept time](../../geophysics.md#seismic-intercept-time) by

$$
\boxed{\tau(p)=T(p)-px(p),\qquad\frac{d\tau}{dp}=-x(p).}
$$

The $x$–$p$ representation displays the gap and fold; the $\tau$–$p$ representation has separate shallow and deep branches and a branch jump at the critical ray parameter for the piecewise-linear cusp model. Do not join them by invented turning rays. [Diffraction](../../quantum-scattering.md#diffraction) and finite-frequency [energy](../../energy.md) soften a purely geometrical shadow.

The figures use an explicit illustrative profile, not measured [Earth](../../planetary-science.md#earth) parameters: [speed](../../classical-mechanics.md#speed) rises from 1 to 2 over depths 0 to 1, falls to 1.8 by depth 1.2, then rises with its original [gradient](../../multivariable-calculus.md#gradient). The [asthenosphere](../../geophysics.md#asthenosphere) beneath oceanic [lithosphere](../../geophysics.md#lithosphere) is an important setting for a [low-velocity zone](../../geophysics.md#low-velocity-zone). A major P-wave [speed](../../classical-mechanics.md#speed) reduction also occurs at the boundary between the [mantle](../../geophysics.md#planetary-mantle) and the [outer core of the Earth](../../geophysics.md#outer-core-of-the-earth); [S waves](../../wave-equation.md#s-wave) do not propagate through the liquid [outer core of the Earth](../../geophysics.md#outer-core-of-the-earth).[Chapter 4, printed pages 169–170, low-velocity-zone rays, shadow range and Earth examples](../../physics-bibliography.md#essentials-of-geophysics-seismology-by-r-d-van-der-hilst)

<a id="3/a/image-analytically-traced-illustrative-velocity-reversal-rays-travel-times-range-slowness-and-intercept-time"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2014/paper-1-pep-low-velocity-rays.png)

**[Figure 4](#3/a/image-analytically-traced-illustrative-velocity-reversal-rays-travel-times-range-slowness-and-intercept-time). Analytically traced illustrative velocity reversal: rays, travel times, range–slowness and intercept time**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

**[Oceanic thermal subsidence](../../geophysics.md#oceanic-thermal-subsidence).** Newly formed oceanic [lithosphere](../../geophysics.md#lithosphere) is hot and buoyant. Cooling increases its column [density](../../fluid-mechanics.md#density), causing subsidence by [isostasy](../../geophysics.md#isostasy) as it moves away from a ridge. The [half-space cooling model](../../geophysics.md#half-space-cooling-model) has profile is

$$
T(z,t)=T_s+(T_m-T_s)\operatorname{erf}\left(\frac{z}{2\sqrt{\kappa t}}\right).
$$

With volumetric [thermal expansion](../../thermodynamics.md#thermal-expansion) coefficient $\alpha$, the excess column [mass](../../classical-mechanics.md#mass) relative to hot [mantle](../../geophysics.md#planetary-mantle) is

$$
\Delta\Sigma\simeq\rho_m\alpha\int_0^\infty(T_m-T)\,dz
=2\rho_m\alpha(T_m-T_s)\sqrt{\frac{\kappa t}{\pi}}.
$$

Compensation with seawater [density](../../fluid-mechanics.md#density) $\rho_w$ gives

$$
\boxed{d(t)=d_r+
\frac{2\rho_m\alpha(T_m-T_s)}{\rho_m-\rho_w}
\sqrt{\frac{\kappa t}{\pi}}.}
$$

Thus young-to-intermediate-age seafloor generally deepens approximately as the square root of age. At old ages, finite thermal-plate thickness and basal [heat](../../heat.md) supply flatten this trend; indefinite half-space deepening is inappropriate. Sediments, variable [crust](../../geophysics.md#planetary-crust), volcanic swells and [dynamic topography](../../geophysics.md#dynamic-topography) also perturb bathymetry. Ocean-floor depth and [heat](../../heat.md) flow jointly constrain cooling models.[1977, half-space cooling, bathymetric age trend and finite-plate alternative](../../physics-bibliography.md#an-analysis-of-the-variation-of-ocean-floor-bathymetry-and-heat-flow-with-age-by-barry-parsons-and-john-g-sclater)

**[Effective elastic thickness](../../geophysics.md#effective-elastic-thickness).** This is the thickness of a homogeneous elastic plate with the observed effective [flexural rigidity](../../elasticity-physics.md#bending-stiffness), not necessarily the crustal or thermal lithospheric thickness:

$$
\boxed{D=\frac{ET_e^3}{12(1-\nu^2)}.}
$$

Infer it by modelling deflection around known loads, such as seamounts or trenches, or fitting [gravity-topography admittance](../../geophysics.md#gravity-topography-admittance) and [gravity-topography coherence](../../geophysics.md#gravity-topography-coherence) across wavelengths. A simple Fourier balance is $(Dk^4+\Delta\rho g)w_k=q_k$ for a signed transverse load. The transition from buoyancy-dominated to bending-dominated behaviour constrains $D$; then assumed [Young's modulus](../../elasticity-physics.md#young-s-modulus) $E$ and [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio) $\nu$ give $T_e$.

Good inference includes load geometry and [density](../../fluid-mechanics.md#density), buried interfaces, sediment and internal loading, [boundary conditions](../../differential-equation.md#boundary-condition) and data resolution. These can trade off with rigidity. Plastic yielding, faulting, mechanical layering and creep make $T_e$ an effective, timescale- and stress-dependent quantity. Older, colder [lithosphere](../../geophysics.md#lithosphere) is often stronger, but age at loading and subsequent relaxation matter; a single universal age-to-$T_e$ conversion is unjustified.

<a id="3/b/image-square-root-cooling-versus-finite-plate-saturation-and-stiffness-sensitivity-of-the-flexural-response"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2014/paper-1-pep-thermal-flexure.png)

**[Figure 5](#3/b/image-square-root-cooling-versus-finite-plate-saturation-and-stiffness-sensitivity-of-the-flexural-response). Square-root cooling versus finite-plate saturation, and stiffness sensitivity of the flexural response**.

## ↑ Ancestors (11)

1. [2014](../2014.md)
2. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
3. [Physics of the Earth as a Planet course of the University of Cambridge](../../university-of-cambridge.md#physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
