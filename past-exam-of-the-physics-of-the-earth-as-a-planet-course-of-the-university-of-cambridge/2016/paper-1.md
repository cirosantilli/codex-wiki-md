# Paper 1

↑ **Parent:** [2016](../2016.md)

Original solutions to the released 2016 1/PEP paper. [Original public PDF, physical pages 790–793; questions on pages 791–793](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=790)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\hat x$ point to the equatorial meridian at zero [longitude](../../multivariable-calculus.md#longitude), $\hat y$ to the equator at $90^\circ$ E, and $\hat z$ to the north pole. Use a right-hand positive [Euler angular velocity vector](../../geophysics.md#euler-angular-velocity-vector). Relative [rotations](../../riemannian-geometry.md#rotation-mathematics) add as [vectors](../../vector-space.md#vector), not as geographic coordinates:

$$
\boldsymbol\omega_{B/C}=\boldsymbol\omega_{B/A}+\boldsymbol\omega_{A/C}=(5\hat x+12\hat y)\times10^{-9}\,\mathrm{rad\,yr^{-1}}.
$$

Consequently

$$
\boxed{|\boldsymbol\omega_{B/C}|=13\times10^{-9}\,\mathrm{rad\,yr^{-1}},\qquad (\phi,\lambda)=(0^\circ,67.380^\circ\mathrm E).}
$$

Here $\lambda=\tan^{-1}(12/5)$ is the [longitude](../../multivariable-calculus.md#longitude) of the positive [Euler pole](../../geophysics.md#euler-pole), and its [latitude](../../astrophysics.md#geographical-latitude) $\phi$ is zero. The antipodal pole with the opposite angular-velocity sign is an equivalent convention; mixing a pole reversal with an unchanged sign would give the wrong motion.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At [latitude](../../astrophysics.md#geographical-latitude) $\phi$ and [longitude](../../multivariable-calculus.md#longitude) $\lambda$, $\mathbf r=R(\cos\phi\cos\lambda,\cos\phi\sin\lambda,\sin\phi)$. Motion is $\mathbf v_{B/C}=\boldsymbol\omega_{B/C}\times\mathbf r$. A meridian boundary has horizontal normal $\hat e_\lambda=(-\sin\lambda,\cos\lambda,0)$, so its across-boundary [velocity](../../classical-mechanics.md#velocity) is

$$
\mathbf v_{B/C}\cdot\hat e_\lambda=-R\sin\phi\,(5\cos\lambda+12\sin\lambda)\times10^{-9}\,\mathrm{yr^{-1}}.
$$

For a [transform fault](../../geophysics.md#transform-fault) this must vanish along the whole meridian, not only at an isolated point. Thus $5\cos\lambda+12\sin\lambda=0$. Select the solution in the western hemisphere:

$$
\boxed{\lambda=-22.620^\circ=22.620^\circ\mathrm W.}
$$

The other solution is the antipodal meridian in the eastern hemisphere. Geometrically, the transform meridian is in a great-circle plane perpendicular to the [Euler angular velocity vector](../../geophysics.md#euler-angular-velocity-vector). Its outgoing tangent direction at either pole, expressed in the fixed $x,y$ axes, is $\hat t_F=(12,-5)/13$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At the south pole $\mathbf r=-R\hat z$. Choose plate C as the instantaneous [reference frame](../../mathematical-physics.md#reference-frame). Since $R=4\times10^9$ mm, the two components of relative angular [speed](../../classical-mechanics.md#speed) give 20 and 48 mm/year. The plate [velocities](../../classical-mechanics.md#velocity) in the fixed tangent-plane axes are

$$
\mathbf v_C=(0,0),\qquad\mathbf v_A=(-48,0),\qquad\mathbf v_B=(-48,20)\quad\mathrm{mm\,yr^{-1}}.
$$

The [plate velocity triangle](../../geophysics.md#plate-velocity-triangle) therefore has sides

$$
\boxed{|\mathbf v_B-\mathbf v_A|=20,\quad|\mathbf v_A-\mathbf v_C|=48,\quad|\mathbf v_B-\mathbf v_C|=52\quad\mathrm{mm\,yr^{-1}}.}
$$

The physical boundary rays point along $+x$ for AB, $+y$ for AC and $(12,-5)$ for BC. Plate A occupies the quadrant between the first two rays, B the narrow wedge between AB and BC, and C the remainder. The stated overriding relations make AB and AC [subduction trenches](../../geophysics.md#subduction-trench), while BC remains a [transform fault](../../geophysics.md#transform-fault): this is a [trench-trench-transform triple junction](../../geophysics.md#trench-trench-transform-triple-junction). Put the [subduction](../../geophysics.md#subduction) teeth on B's side of AB and A's side of AC, identifying B above A and A above C.

For kinematic stability there must be a single junction [velocity](../../classical-mechanics.md#velocity) $\mathbf U$ compatible with all three boundary-normal motions. Use the standard idealization that each trench's normal [velocity](../../classical-mechanics.md#velocity) is that of its [overriding plate](../../geophysics.md#overriding-plate), with no independent rollback. AB is parallel to $x$, so $U_y=v_{B,y}=20$. AC is parallel to $y$, so $U_x=v_{A,x}=-48$. The transform requires $\mathbf U-\mathbf v_C$ to be parallel to $(12,-5)$, which is true for this intersection. Hence

$$
\boxed{\mathbf U_S=(-48,20)\,\mathrm{mm\,yr^{-1}}=\mathbf v_B\quad\text{in the C frame}.}
$$

**The southern [triple junction](../../geophysics.md#triple-junction) is instantaneously kinematically stable.** It is stationary relative to B, migrates along AB relative to A, and migrates along BC relative to C. This compatibility result does not promise long-term stability if plate [rotations](../../riemannian-geometry.md#rotation-mathematics) or trench rollback change. Notice that the three relative [velocities](../../classical-mechanics.md#velocity) close even though the overriding order is not a statement that all three plates move toward one common stationary point.

<a id="1/c/image-original-polar-boundary-geometry-and-plate-velocity-triangles-dashed-velocity-space-constraints-locate-compatible-south-and-north-junction-velocities"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2016/paper-1-polar-junctions.png)

**[Figure 1](#1/c/image-original-polar-boundary-geometry-and-plate-velocity-triangles-dashed-velocity-space-constraints-locate-compatible-south-and-north-junction-velocities). Original polar boundary geometry and plate velocity triangles; dashed velocity-space constraints locate compatible south and north junction velocities**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

At the north pole $\mathbf r=+R\hat z$, so the [velocities](../../classical-mechanics.md#velocity) reverse:

$$
\mathbf v_C=(0,0),\qquad\mathbf v_A=(48,0),\qquad\mathbf v_B=(48,-20)\quad\mathrm{mm\,yr^{-1}}.
$$

The triangle still has side lengths 20, 48 and 52 mm/year. Across AB, A moves toward positive $y$ relative to B; across AC, A moves toward positive $x$ relative to C. Both boundaries therefore open and are [spreading ridges](../../geophysics.md#spreading-ridge), with full opening [speeds](../../classical-mechanics.md#speed) 20 and 48 mm/year. Together with BC they form a [ridge-ridge-transform triple junction](../../geophysics.md#ridge-ridge-transform-triple-junction).

In the symmetric normal-spreading model, a ridge's normal [velocity](../../classical-mechanics.md#velocity) is the mean normal [velocity](../../classical-mechanics.md#velocity) of its two plates. AB gives $U_y=(0-20)/2=-10$, and AC gives $U_x=(48+0)/2=24$. Their intersection lies on the BC transform [velocity](../../classical-mechanics.md#velocity) line:

$$
\boxed{\mathbf U_N=(24,-10)\,\mathrm{mm\,yr^{-1}}=\frac{\mathbf v_B+\mathbf v_C}{2}.}
$$

**This northern junction is also instantaneously kinematically stable.** The diagrams use the same fixed geocentric tangent axes at both poles; reversing [velocities](../../classical-mechanics.md#velocity) is not the same operation as reflecting a map drawn from an exterior observer's viewpoint.

Not every ridge-ridge-transform geometry works. For pure normal spreading, each ridge [velocity](../../classical-mechanics.md#velocity) line is the [perpendicular bisector](../../euclidean-geometry.md#perpendicular-bisector) of the corresponding side of the [plate velocity triangle](../../geophysics.md#plate-velocity-triangle). Their intersection is the triangle's [circumcenter](../../euclidean-geometry.md#circumcenter). A transform junction must also lie on the third side's line. A nondegenerate triangle's [circumcenter](../../euclidean-geometry.md#circumcenter) lies there only at that side's midpoint, so the opposite angle is a right angle. Equivalently, $\big(\mathbf v_B-\mathbf v_A\big)\cdot\big(\mathbf v_C-\mathbf v_A\big)=0$. The two ridge directions are then perpendicular, as they are here. **RRF junctions are conditionally stable, with the right-angle ridge geometry in this symmetric pure-normal model; they are not all stable.** Oblique or asymmetric accretion changes the velocity-line assumptions and must be specified separately.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Assume an Earth-like reversing planetary [magnetic field](../../magnetic-field.md) and magnetizable crust that acquires [thermoremanent magnetization](../../geophysics.md#thermoremanent-magnetization) on cooling. Alternating polarity intervals then produce [marine magnetic stripes](../../geophysics.md#marine-magnetic-stripe) parallel to each [spreading ridge](../../geophysics.md#spreading-ridge), with matching age/polarity sequences on its two sides. AB has [half-spreading rate](../../geophysics.md#half-spreading-rate) 10 mm/year, whereas AC has [half-spreading rate](../../geophysics.md#half-spreading-rate) 24 mm/year. Thus the same polarity interval $\Delta t$ produces widths $10\Delta t$ and $24\Delta t$ mm when time is in years: the AC stripes are 2.4 times wider. Age increases away from each ridge. The transform produces no new crust; bands end or are displaced at it, rather than forming a third symmetric stripe sequence centred on BC. This is the remanent-magnetization/spreading mechanism developed from marine magnetic observations.[pp. 947–949, alternating remanent magnetization and the spreading interpretation](../../physics-bibliography.md#magnetic-anomalies-over-oceanic-ridges-by-f-j-vine-and-d-h-matthews)

A more precise local sketch can be made in the northern junction frame. Let $x,y$ be distances in kilometres along the fixed tangent axes and $t$ the crustal age in Myr; numerically, mm/year equals km/Myr. Relative to the moving junction, the [velocities](../../classical-mechanics.md#velocity) are $\mathbf w_A=(24,10)$, $\mathbf w_B=(24,-10)$ and $\mathbf w_C=(-24,10)$. In A the steady age field is $t_A=\min(x/24,y/10)$, since backwards advection first reaches either the AC or AB ridge. Equal-age bands therefore join as right-angle corners within A, with the corners migrating along the ray $(24,10)$. In the B wedge, $t_B=-y/10$ and the stripes meet the transform. On the C flank directly supplied from AC, $t_C=-x/24$; other parts of C carry older crust whose inherited pattern requires earlier boundary history.

<a id="1/e/image-original-conditional-remanent-polarity-sketch-in-the-north-junction-frame-reversal-intervals-are-illustrative-and-unsupplied-older-crust-is-left-unassigned"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2016/paper-1-magnetic-stripes.png)

**[Figure 2](#1/e/image-original-conditional-remanent-polarity-sketch-in-the-north-junction-frame-reversal-intervals-are-illustrative-and-unsupplied-older-crust-is-left-unassigned). Original conditional remanent-polarity sketch in the north-junction frame; reversal intervals are illustrative and unsupplied older crust is left unassigned**.

The sketch displays [magnetization](../../electromagnetism.md#magnetization) polarity, not a computed total-field anomaly amplitude. Actual anomalies depend on the planetary field direction, source depth, [magnetization](../../electromagnetism.md#magnetization) strength and observation geometry. The paper supplies no field history, so a numerical reversal chronology or an absolute positive/negative anomaly sequence cannot be inferred. Without field reversals, ridge accretion alone does not imply alternating polarity stripes.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**[gravity](../../physics.md#gravity) and [surface topography](../../optics.md#surface-topography).** [gravity](../../physics.md#gravity) responds to all [density](../../fluid-mechanics.md#density) structure, while [surface topography](../../optics.md#surface-topography) records both load and support. First specify the reference field and measurement height. [latitude](../../astrophysics.md#geographical-latitude) and planetary [rotation](../../riemannian-geometry.md#rotation-mathematics) affect normal [gravity](../../physics.md#gravity). At elevation $h$, the reference field decreases approximately by $2gh/R$; a [free-air gravity anomaly](../../geophysics.md#free-air-gravity-anomaly) restores this elevation effect but retains topographic [mass](../../classical-mechanics.md#mass). A [Bouguer gravity anomaly](../../geophysics.md#bouguer-gravity-anomaly) additionally subtracts an approximate topographic slab contribution $2\pi G\rho_ch$. [terrain correction](../../geophysics.md#terrain-correction) replaces the unrealistic slab near valleys and ridges, and spherical geometry matters over large areas. A [density](../../fluid-mechanics.md#density) choice is required for these reductions; a numerical crustal [density](../../fluid-mechanics.md#density) is not provided here.

In [Airy isostasy](../../geophysics.md#airy-isostasy), [surface topography](../../optics.md#surface-topography) of height $h$ and crustal [density](../../fluid-mechanics.md#density) $\rho_c$ is compensated by a root of thickness $b$ replacing mantle of [density](../../fluid-mechanics.md#density) $\rho_m>\rho_c$. Equal column [masses](../../classical-mechanics.md#mass) give $\rho_ch=(\rho_m-\rho_c)b$. The positive [gravity](../../physics.md#gravity) of the relief is partly cancelled by the negative [density](../../fluid-mechanics.md#density) contrast of the root. At long wavelengths a compensated mountain can therefore have a modest free-air anomaly and a negative Bouguer anomaly. [Pratt isostasy](../../geophysics.md#pratt-isostasy) instead varies column [density](../../fluid-mechanics.md#density) at a roughly common compensation depth. Neither model says that [surface topography](../../optics.md#surface-topography) itself exerts no [gravity](../../physics.md#gravity).

Potential-field depth filtering makes wavelength crucial. In a planar Fourier approximation, a [density](../../fluid-mechanics.md#density) interface at depth $z$ is attenuated by $e^{-kz}$ at horizontal [wavenumber](../../wave-equation.md#wavenumber) $k$. For a small Airy-compensated height perturbation and a compensation interface at depth $D$, the [gravity-topography admittance](../../geophysics.md#gravity-topography-admittance) is approximately

$$
Z_{\rm FA}(k)=2\pi G\rho_c(1-e^{-kD}),\qquad Z_{\rm B}(k)=-2\pi G\rho_ce^{-kD}.
$$

Long wavelengths allow strong cancellation between load and root. At short wavelengths the root's [gravity](../../physics.md#gravity) is filtered out, so the observed near-surface [mass](../../classical-mechanics.md#mass) can dominate even if the column is compensated. In a [flexural isostasy](../../geophysics.md#flexural-isostasy) model, an elastic [lithosphere](../../geophysics.md#lithosphere) supports and spreads the load; for downward deflection $w$ and imposed load $q$, $D_f\nabla^4w+\Delta\rho g w=q$, with $D_f=ET_e^3/[12(1-\nu^2)]$. Thus $w_k=q_k/(D_fk^4+\Delta\rho g)$, and the effective elastic thickness controls the support scale.

Estimate admittance from cross-spectra of [gravity](../../physics.md#gravity) and [surface topography](../../optics.md#surface-topography), and compare its wavelength dependence and coherence with local-compensation, elastic-flexure and subsurface-load models. A primary Atlantic study sampled ship-track free-air [gravity](../../physics.md#gravity) and bathymetry and compared their Fourier-domain relationship with compensation models, illustrating this observational route rather than inferring a root from the sign of one [gravity](../../physics.md#gravity) value.[pp. 1903–1915, ship-track sampling, spectral transfer estimates and wavelength-dependent compensation](../../physics-bibliography.md#the-relationship-between-bathymetry-and-gravity-in-the-atlantic-ocean-by-dan-mckenzie-and-carl-bowin) Check navigation, instrument drift, terrain/[density](../../fluid-mechanics.md#density) reductions, sediment and water loads, and independent seismic crustal constraints. Density-depth trade-offs and mantle dynamic support make the [inverse problem](../../inverse-problem.md) nonunique; [surface topography](../../optics.md#surface-topography) and [gravity](../../physics.md#gravity) together constrain support, but do not uniquely map every [density](../../fluid-mechanics.md#density) anomaly.

**[mantle viscosity](../../planetary-science.md#mantle-viscosity).** A second, independent route concerns deformation rates rather than static compensation. [glacial isostatic adjustment](../../geophysics.md#glacial-isostatic-adjustment) follows loading and unloading of a deformable [Earth](../../planetary-science.md#earth): an ice sheet depresses the surface, and subsequent removal leaves time-dependent uplift, horizontal [displacement](../../classical-mechanics.md#displacement), sea-level and [gravity](../../physics.md#gravity) changes. Fit dated relative sea-level indicators and raised shorelines together with geodetic [displacement](../../classical-mechanics.md#displacement) rates and a reconstructed ice/water load history to a viscoelastic [Earth](../../planetary-science.md#earth) model. Relative sea level includes solid-surface motion, changing [geoid](../../geophysics.md#geoid) and redistribution of ocean water; treating it only as local vertical rock motion biases the inference.

For scale, a sinusoidal surface perturbation of [wavenumber](../../wave-equation.md#wavenumber) $k$ on a uniform incompressible viscous half-space relaxes under [gravity](../../physics.md#gravity) with $\tau_k\sim2\eta k/(\rho g)$. A Maxwell material separately has a stress-relaxation scale $\tau_M=\eta/\mu$. These are different experiments and generally different times: rebound modes also involve [gravity](../../physics.md#gravity), spherical geometry, a layered mantle and elastic [lithosphere](../../geophysics.md#lithosphere). Fit a family of relaxation modes or a full load-history convolution, rather than equating every observed rebound time to $\eta/\mu$.

Use independent ice-margin, exposure-age and sea-level constraints to reduce the trade-off between ice history and [viscosity](../../dynamic-viscosity.md); compare horizontal as well as vertical [GNSS](../../geophysics.md#gnss) motions, and separate present ice loss, groundwater changes and tectonic signals from the older loading response. A primary global analysis jointly tested ice-history and mantle-response predictions against space-geodetic observations, rather than treating a local uplift rate as a unique [viscosity](../../dynamic-viscosity.md) measurement.[abstract and pp. 450–487, joint ice-history/GIA model and space-geodetic constraints](../../physics-bibliography.md#space-geodesy-constrains-ice-age-terminal-deglaciation-the-global-ice-6g-c-vm5a-model-by-w-r-peltier-and-others)

[postseismic relaxation](../../planetary-science.md#postseismic-relaxation) probes shallower or faster relaxation after a [stress](../../continuum-mechanics.md#stress) perturbation, but must be distinguished from afterslip and poroelastic deformation. Long-wavelength [geoid](../../geophysics.md#geoid) and mantle-flow models provide complementary constraints when [density](../../fluid-mechanics.md#density) structure is estimated independently from seismic structure and mineral physics; unknown density-to-velocity conversion and boundary [tractions](../../continuum-mechanics.md#traction) remain trade-offs. Laboratory creep experiments constrain constitutive laws as functions of [temperature](../../temperature.md), [stress](../../continuum-mechanics.md#stress) and grain size, but require a large extrapolation to geological conditions. **Combine spatially and temporally distinct observations; there is no single directly measured [mantle viscosity](../../planetary-science.md#mantle-viscosity) independent of depth, [rheology](../../rheology.md) and loading assumptions.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**First-motion source mechanisms.** Locate an [earthquake](../../geophysics.md#earthquake) from arrival times and use a seismic [velocity](../../classical-mechanics.md#velocity) model to calculate each station's source takeoff direction. Measure the initial direct [P wave](../../wave-equation.md#p-wave) polarity after checking instrument sign, component orientation, timing and phase identification. An upward trace at an instrument is not automatically a source compression without the propagation and component convention. Plot the inferred source radiation signs on a [focal sphere](../../wave-equation.md#focal-sphere), commonly using a lower-hemisphere equal-area projection, and seek nodal planes separating positive and negative observations.

For a shear dislocation with orthogonal unit slip and fault-normal [vectors](../../vector-space.md#vector) $\mathbf s,\mathbf n$, the [double-couple fault source](../../wave-equation.md#double-couple-fault-source) has $M=M_0(\mathbf s\mathbf n^{\mathsf T}+\mathbf n\mathbf s^{\mathsf T})$. Its far-field P radiation sign is that of

$$
A_P(\hat{\mathbf r})\propto\hat{\mathbf r}^{\mathsf T}M\hat{\mathbf r}=2M_0(\hat{\mathbf r}\cdot\mathbf s)(\hat{\mathbf r}\cdot\mathbf n).
$$

The two zeros are orthogonal nodal planes; the four quadrants alternate between outward and inward initial radiation. Their orientations and quadrant signs determine candidate strike, dip and rake. Normal, reverse and strike-slip mechanisms give different projected patterns. The [earthquake pressure and tension axes](../../wave-equation.md#earthquake-pressure-and-tension-axes) are the negative and positive moment-tensor principal directions, respectively; they do not by themselves measure the complete regional [stress tensor](../../continuum-mechanics.md#cauchy-stress-tensor).

<a id="2/b/image-original-lower-hemisphere-equal-area-p-radiation-polarity-examples-for-ideal-strike-slip-normal-and-reverse-double-couples"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2016/paper-1-focal-mechanisms.png)

**[Figure 3](#2/b/image-original-lower-hemisphere-equal-area-p-radiation-polarity-examples-for-ideal-strike-slip-normal-and-reverse-double-couples). Original lower-hemisphere equal-area P-radiation polarity examples for ideal strike-slip, normal and reverse double couples**.

There is a fundamental [fault-plane ambiguity](../../wave-equation.md#fault-plane-ambiguity): exchanging $\mathbf s$ and $\mathbf n$ leaves the radiation tensor unchanged. First motions therefore give a fault plane and an auxiliary plane without saying which actually slipped. Use mapped rupture, [aftershock](../../geophysics.md#aftershock) geometry or independent geodetic [displacement](../../classical-mechanics.md#displacement) to select the physical fault where possible. Polarity signs alone do not measure scalar seismic moment, source duration or rupture extent. A poorly sampled [focal sphere](../../wave-equation.md#focal-sphere) or many near-nodal observations can admit several mechanisms rather than one defensible beachball.

Propagate uncertainty in event depth, [velocity](../../classical-mechanics.md#velocity) gradients and takeoff angles, allow for mispicked or reversed polarities, and report the range of mechanisms consistent with the observations. A primary method did this by testing alternative locations and [velocity](../../classical-mechanics.md#velocity) models and validated its uncertainty estimates using noisy synthetic data and clusters of events with similar waveforms.[pp. 2264–2266 and abstract, first-motion construction, polarity/takeoff uncertainty and independent validation tests](../../physics-bibliography.md#a-new-method-for-determining-first-motion-focal-mechanisms-by-jeanne-l-hardebeck-and-peter-m-shearer) Broadband waveforms and amplitude ratios add information, especially for non-double-couple sources, but they are additional measurements rather than a way to extract amplitude information from a sign-only data set.

**Radial [density](../../fluid-mechanics.md#density) structure.** In an [isotropic](../../continuum-mechanics.md#isotropy) adiabatic material, the [seismic parameter](../../geophysics.md#seismic-parameter) is

$$
\Phi(r)=\frac{K_S}{\rho}=\alpha(r)^2-\frac43\beta(r)^2.
$$

For a chemically homogeneous region whose background stratification is adiabatic, $d\rho/dP=\rho/K_S=1/\Phi$. Combine this with spherical hydrostatic balance and [mass](../../classical-mechanics.md#mass) conservation to obtain the [Adams-Williamson equations](../../geophysics.md#adams-williamson-equation)

$$
\boxed{\frac{d\rho}{dr}=-\frac{\rho g}{\Phi},\qquad\frac{dm}{dr}=4\pi r^2\rho,\qquad g=\frac{Gm}{r^2},\qquad\frac{dP}{dr}=-\rho g.}
$$

The inward [density](../../fluid-mechanics.md#density) increase follows [compressibility](../../thermodynamics.md#compressibility) under the increasing [pressure](../../pressure.md). A specified starting [density](../../fluid-mechanics.md#density) and measured $\Phi(r)$ allow integration within a homogeneous adiabatic layer. Seismic [velocities](../../classical-mechanics.md#velocity) alone, however, do not determine that [density](../../fluid-mechanics.md#density) normalization, since they contain ratios of moduli to [density](../../fluid-mechanics.md#density). Chemical boundaries, phase transitions, nonadiabatic thermal gradients and [anisotropy](../../continuum-mechanics.md#anisotropy) require additional modeling; a composition jump is not obtained by blindly integrating the smooth relation across it.

Use travel times and surface waves to constrain elastic [velocities](../../classical-mechanics.md#velocity), reflected/converted phases to locate interfaces, and normal-mode frequencies to constrain [density](../../fluid-mechanics.md#density) as well as elastic structure through their sensitivity kernels. Impose independently known total [mass](../../classical-mechanics.md#mass) and [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia):

$$
M=4\pi\int_0^R\rho(r)r^2\,dr,\qquad I=\frac{8\pi}{3}\int_0^R\rho(r)r^4\,dr.
$$

Because these weight depth differently, they help distinguish admissible profiles, but two integrals alone do not specify an arbitrary radial function. Laboratory equations of state and mineral physics restrict composition, [compressibility](../../thermodynamics.md#compressibility) and [density](../../fluid-mechanics.md#density) jumps. [pressure](../../pressure.md) and enclosed [mass](../../classical-mechanics.md#mass) are matched across interfaces, while [density](../../fluid-mechanics.md#density) may jump. In a liquid region $\beta=0$ and $\Phi=\alpha^2$, so the shear-wave absence constrains phase state without itself providing a direct [density](../../fluid-mechanics.md#density) measurement.

The [Preliminary Reference Earth Model](../../geophysics.md#preliminary-reference-earth-model) is a concrete joint inversion of seismic travel times, [normal modes](../../wave-equation.md#normal-mode), [mass](../../classical-mechanics.md#mass) and inertia, including [density](../../fluid-mechanics.md#density) and attenuation along with elastic structure. The original analysis combined these complementary data rather than deriving [density](../../fluid-mechanics.md#density) uniquely from [P wave](../../wave-equation.md#p-wave) [speed](../../classical-mechanics.md#speed).[abstract and pp. 297–300, data classes and coupled radial reference-model inversion](../../physics-bibliography.md#preliminary-reference-earth-model-by-adam-m-dziewonski-and-don-l-anderson) **A defensible radial [density](../../fluid-mechanics.md#density) model combines hydrostatic/thermodynamic relations with seismic and global integral constraints, and states where homogeneity and adiabaticity fail.**

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For uniform [density](../../fluid-mechanics.md#density) $\rho>0$ and stiffness, linear momentum balance without [body force](../../fluid-mechanics.md#body-force) is $\rho\ddot u_i=\partial_j\sigma_{ij}$. The minor elastic symmetries make the two symmetric-strain terms equal, so $\partial_j\sigma_{ij}=c_{ijkl}u_{k,lj}$. Write $s=ct-\hat p_jx_j$ and $u_i=a_if(s)$. Then $\ddot u_i=c^2a_if''$ and $u_{k,lj}=a_k\hat p_l\hat p_jf''$. Thus a nontrivial plane-wave profile satisfies

$$
\rho c^2a_i=c_{ijkl}\hat p_j\hat p_la_k.
$$

The density-normalized [elastic acoustic tensor](../../elasticity-physics.md#acoustic-tensor) is consequently

$$
\boxed{B_{ij}=\frac1\rho c_{ikjl}\hat p_k\hat p_l,\qquad B_{ij}a_j=c^2a_i.}
$$

The alternative dummy-index form $B_{ik}=\rho^{-1}c_{ijkl}\hat p_j\hat p_l$ is identical. In ordinary conservative [elasticity](../../elasticity-physics.md), major symmetry $c_{ikjl}=c_{jlik}$ gives $B_{ji}=B_{ij}$ after interchanging the dummy indices. This symmetry comes from a strain-energy [density](../../fluid-mechanics.md#density); it is an assumption of the ordinary elastic tensor, not a consequence of homogeneity alone.

For any such eigenpair the profile $f$ is arbitrary, since both sides carry the same $f''$. This nondispersive result uses linear, local, time-independent [elasticity](../../elasticity-physics.md) without attenuation or spatial dispersion. A profile with $f''=0$ is a trivial uniform or affine [displacement](../../classical-mechanics.md#displacement) field and cannot be used by itself to infer the wave-speed [eigenvalue](../../linear-operator-theory.md#eigenvalue) condition.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A real symmetric $3\times3$ [matrix](../../vector-space.md#matrix) has three real [eigenvalues](../../linear-operator-theory.md#eigenvalue) and a complete [orthonormal basis](../../inner-product.md#orthonormal-basis) of [eigenvectors](../../linear-operator-theory.md#eigenvector). For a stable elastic material, [strong ellipticity](../../elasticity-physics.md#strong-ellipticity) makes $\mathbf a^{\mathsf T}B\mathbf a>0$ for every nonzero [polarization](../../wave.md#polarization-waves), so its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are positive squared wave [speeds](../../classical-mechanics.md#speed). There are therefore three orthogonal plane-wave [polarizations](../../wave.md#polarization-waves) in a given direction, with three potentially distinct [speeds](../../classical-mechanics.md#speed) in an anisotropic medium. Degenerate [eigenvalues](../../linear-operator-theory.md#eigenvalue) allow arbitrary orthonormal combinations within their eigenspace; they do not remove [polarization](../../wave.md#polarization-waves) degrees of freedom. General anisotropic modes need not be exactly longitudinal or transverse.

For an [isotropic](../../continuum-mechanics.md#isotropy) medium let $\lambda=\kappa-2\mu/3$. Contract the [isotropic](../../continuum-mechanics.md#isotropy) stiffness with $\hat p_k\hat p_l$:

$$
B_{ij}=\frac1\rho\big[(\lambda+\mu)\hat p_i\hat p_j+\mu\delta_{ij}\big].
$$

Using

$$
\alpha^2=\frac{\kappa+4\mu/3}{\rho}=\frac{\lambda+2\mu}{\rho},\qquad\beta^2=\frac\mu\rho,
$$

gives

$$
\boxed{B_{ij}=(\alpha^2-\beta^2)\hat p_i\hat p_j+\beta^2\delta_{ij}.}
$$

For $\mathbf a\parallel\hat{\mathbf p}$ the longitudinal projector has [eigenvalue](../../linear-operator-theory.md#eigenvalue) one, so $B\mathbf a=\alpha^2\mathbf a$: this is the [P wave](../../wave-equation.md#p-wave). For either of two independent $\mathbf a\perp\hat{\mathbf p}$ the projector vanishes, so $B\mathbf a=\beta^2\mathbf a$: these are two degenerate transverse [S wave](../../wave-equation.md#s-wave) [polarizations](../../wave.md#polarization-waves). **An [isotropic](../../continuum-mechanics.md#isotropy) solid has one P [speed](../../classical-mechanics.md#speed) and one S [speed](../../classical-mechanics.md#speed), but three [polarization](../../wave.md#polarization-waves) modes: one longitudinal and two transverse.** A fluid limit with zero [shear modulus](../../elasticity-physics.md#shear-modulus) has no propagating [S wave](../../wave-equation.md#s-wave), so the positive-speed conclusion requires a solid with positive shear stiffness.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use geometric rays for body-wave arrivals and a traction-free upper surface. A compact [isotropic explosion source](../../wave-equation.md#isotropic-explosion-source) has moment tensor proportional to $\delta_{ij}$ and produces direct P body radiation in a homogeneous [isotropic](../../continuum-mechanics.md#isotropy) medium. Thus the basic near-offset arrival is the direct upper-layer [P wave](../../wave-equation.md#p-wave), with time $X/\alpha_1$. A pure explosion is not a shear fault: it does not automatically emit a direct [S wave](../../wave-equation.md#s-wave) of comparable strength. Interfaces can nevertheless convert its P [energy](../../energy.md) into SV motion, and the free surface can support [Rayleigh waves](../../wave-equation.md#rayleigh-wave).

Downward P [energy](../../energy.md) reflects from the interface to give a PP [reflection](../../linear-algebra.md#reflection-mathematics) returning to the receiver; for a horizontal interface its ray is symmetric and its time is $\sqrt{X^2+4H^2}/\alpha_1$. Other transmitted P [energy](../../energy.md) enters the faster half-space. At $\sin i_c=\alpha_1/\alpha_2$, a critical ray travels along the interface and feeds an upgoing [seismic head wave](../../wave-equation.md#seismic-head-wave), often labeled Pn in this simplified crustal model. Its ideal travel-time branch is

$$
t_{\rm head}=\frac{X}{\alpha_2}+\frac{2H\cos i_c}{\alpha_1}.
$$

It requires enough offset for the two inclined upper-layer legs, $X\ge2H\tan i_c$. Once $X$ exceeds the larger [first-arrival crossover distance](../../wave-equation.md#first-arrival-crossover-distance) $X_c=2H\sqrt{(\alpha_2+\alpha_1)/(\alpha_2-\alpha_1)}$, this branch arrives before the direct upper-layer wave because it spends most of the path in faster material. A transmitted ray descending into an otherwise uniform infinite half-space does not return as a separate [reflection](../../linear-algebra.md#reflection-mathematics) without an additional reflector.

<a id="3/c/image-original-two-layer-p-ray-sketches-and-illustrative-direct-reflected-and-critically-refracted-travel-time-branches"></a>
![](../../past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2016/paper-1-seismic-phases.png)

**[Figure 4](#3/c/image-original-two-layer-p-ray-sketches-and-illustrative-direct-reflected-and-critically-refracted-travel-time-branches). Original two-layer P-ray sketches and illustrative direct, reflected and critically refracted travel-time branches**.

At oblique incidence, the bonded-interface conditions couple P and SV [polarizations](../../wave.md#polarization-waves). A downgoing P ray can return as a converted SV [reflection](../../linear-algebra.md#reflection-mathematics) in the upper layer, with common horizontal slowness $p=\sin i_P/\alpha_1=\sin i_S/\beta_1$. There are transmitted P/SV branches and, after further interaction with the free surface or interface, mixed-mode [reflections](../../linear-algebra.md#reflection-mathematics) and [layer reverberations](../../geophysics.md#layer-reverberation). Conversion coefficients depend on [density](../../fluid-mechanics.md#density) and impedance as well as wave [speeds](../../classical-mechanics.md#speed), and some vanish at normal incidence. The supplied inequalities do not order $\beta_2$ against $\alpha_1$, so one cannot universally draw a P-incident critical head ray travelling at the lower-layer S [speed](../../classical-mechanics.md#speed): that direct conversion construction requires $\beta_2>\alpha_1$. A shear head-wave phase can be present if the appropriate SV [energy](../../energy.md) and ray conditions are available, but is not an inevitable direct explosion arrival from the stated data alone.

At later times a shallow explosion can excite dispersive Rayleigh-wave trains, with coupled P-SV motion decaying with depth. Short wavelengths mainly sample the slow upper layer, whereas long wavelengths penetrate the lower half-space; group and phase [speeds](../../classical-mechanics.md#speed) need not be equal. Multiple reflected/converted body waves can overlap this coda. The shear-speed contrast also permits Love-wave modes structurally, but SH motion is decoupled from P-SV in this flat [isotropic](../../continuum-mechanics.md#isotropy) model. **An ideal [isotropic](../../continuum-mechanics.md#isotropy) explosion does not excite [Love waves](../../wave-equation.md#love-wave) here; appreciable SH/Love [energy](../../energy.md) would require source asymmetry, scattering or a broken symmetry of the model.**

Exact amplitudes, resolved arrival separation and attenuation cannot be calculated without [densities](../../fluid-mechanics.md#density), source spectrum, damping and instrument response. The qualitative robust features are a near-offset direct P arrival, reflected and converted phases, a faster-lower-layer P head wave that can become first at long range, reverberations and P-SV surface-wave [energy](../../energy.md). The ray diagram uses declared illustrative [speed](../../classical-mechanics.md#speed) ratios solely to show the geometry; they are not additional supplied material constants.

## ↑ Ancestors (11)

1. [2016](../2016.md)
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
