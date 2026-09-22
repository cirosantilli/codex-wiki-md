# Paper 1

↑ **Parent:** [2014](../2014.md)

Original public paper: [FOI release, physical pages 667–668; questions on page 668](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1).

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The detector is intended for arcsecond-scale [astronomical seeing](../../optics.md#astronomical-seeing), rather than the telescope's [diffraction limit](../../optics.md#diffraction-limit). A circular [aperture](../../optics.md#aperture) of this area has diameter $1.13\,\mathrm m$, giving a [Rayleigh criterion](../../point-spread-function.md#rayleigh-criterion) angle about $0.11$ arcsec at the observing [wavelength](../../wave-equation.md#wavelength). One-arcsecond pixels conventionally sample an [astronomical seeing](../../optics.md#astronomical-seeing) profile of roughly two arcseconds across with two samples; a one-arcsecond profile would be undersampled. **The pixel scale alone does not determine an exact [astronomical seeing](../../optics.md#astronomical-seeing) width.**

Use the supplied [surface brightness](../../astrophysics.md#surface-brightness) as [radiative flux](../../astrophysics.md#radiative-flux) integrated over the [photometric passband](../../astrophysics.md#photometric-passband): its units contain no inverse hertz. Treat $h\nu$ as the representative [photon energy](../../quantum-mechanics.md#photon-energy), and assume unit throughput and [quantum efficiency](../../optical-instrument.md#quantum-efficiency). A genuinely frequency-specific brightness would require a [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing). With angles measured consistently in arcseconds, an annulus has area $2\pi r\,dr$ square arcseconds, so

$$
F(r_m)=\int_0^{r_m}2\pi r\,a(1-kr)\,dr
=\boxed{2\pi a\left(\frac{r_m^2}{2}-\frac{kr_m^3}{3}\right)}.
$$

This is flux per collecting area; collected [energy](../../energy.md) is $AtF$. There is no extra conversion to [steradians](../../euclidean-geometry.md#steradian) when both brightness and angular area use square arcseconds.

For [Poisson photon counting](../../electrical-engineering.md#poisson-photon-counting), a pixel with expected count $N$ has [energy](../../energy.md) $e=Nh\nu$ and [standard deviation](../../variance.md#standard-deviation) $\sigma_e=h\nu\sqrt N$. Thus the local four-sigma rule gives $N=4\sqrt N$, or **16 [photons](../../quantum-mechanics.md#photon) at the boundary**. With pixel area $\Delta\Omega=1\,\mathrm{arcsec}^2$,

$$
h\nu=3.9756\times10^{-19}\,\mathrm J,\qquad
N(r)=\frac{At\Delta\Omega\,a}{h\nu}(1-kr)=32.6991(1-kr).
$$

Consequently $r_m=(1-16/32.6991)/k=10.2138$ arcsec and

$$
\boxed{E_m=AtF(r_m)=2.8100\times10^{-15}\,\mathrm J}.
$$

Integrating to the model's outer radius $R=1/k=20$ arcsec instead gives

$$
\boxed{F_{\rm total}=\frac{\pi a}{3k^2}=5.4454\times10^{-17}\,\mathrm{W\,m^{-2}}},
\qquad E_{\rm total}=5.4454\times10^{-15}\,\mathrm J.
$$

The pixel cut retains **51.6%** of this total. It is an imposed [isophotal photometry](../../astrophysics.md#isophotal-photometry) rule, not a fundamental limit: averaging annuli or fitting a justified profile can recover signal below the per-pixel cut.

<a id="1/image-original-photon-counting-profile-and-fraction-of-total-flux-inside-the-imposed-detection-radius"></a>
![](../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1-isophotal-flux.png)

**[Figure 1](#1/image-original-photon-counting-profile-and-fraction-of-total-flux-inside-the-imposed-detection-radius). Original photon-counting profile and fraction of total flux inside the imposed detection radius**.

In practice, [sky background](../../astrophysics.md#sky-brightness) [photons](../../quantum-mechanics.md#photon) add [shot noise](../../electrical-engineering.md#shot-noise) even after subtraction of the mean sky. [read noise](../../optical-instrument.md#read-noise), [dark current](../../optical-instrument.md#dark-current-physics), imperfect [flat-field correction](../../optical-instrument.md#flat-field-correction), throughput [calibration](../../differential-geometry.md#calibration-differential-geometry) and [atmospheric extinction](../../optics.md#atmospheric-extinction) also matter. At large radius the dominant uncertainty can be a tiny error in the sky level, scattered light or the wings of the [point spread function](../../point-spread-function.md), rather than source [photon](../../quantum-mechanics.md#photon) statistics. Mask foreground [stars](../../stellar-astrophysics.md#star) and background objects, compare blank-sky regions and dithered exposures, and check profile recovery by inserting artificial extended sources. [astronomical seeing](../../optics.md#astronomical-seeing) and finite pixels convolve the intrinsic profile; model that response when extrapolating the total.

The [luminosity convergence of an outer surface-brightness profile](../../astrophysics.md#luminosity-convergence-of-an-outer-surface-brightness-profile) follows directly: $I\propto r^{-p}$ contributes $dF\propto r^{1-p}dr$, hence $F(<R)\propto R^{2-p}$ at large radius for $p<2$. For either shallow index considered, ever larger annuli dominate: extending the law to infinity gives an unphysical divergent [luminosity](../../astrophysics.md#luminosity). Such a law must eventually steepen or truncate. Over a finite range, however, substantial light can lie below a [surface-brightness selection](../../causal-inference.md#surface-brightness-selection) threshold and be mistaken for sky. This biases [galaxy](../../galaxy.md) [luminosities](../../astrophysics.md#luminosity), the [luminosity function](../../astrophysics.md#luminosity-function-astronomy) and the inferred diffuse light budget; distant diffuse [galaxies](../../galaxy.md) become especially incomplete because bolometric [cosmological surface-brightness dimming](../../astrophysics.md#cosmological-surface-brightness-dimming) scales as $(1+z)^{-4}$. An assumed finite-aperture total is therefore a model-dependent quantity.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The observed population is the parent population filtered by an [astronomical selection function](../../astrophysics.md#astronomical-selection-function) and measurement errors. [Malmquist bias](../../astrophysics.md#malmquist-bias) arises because a [flux-limited galaxy selection](../../astrophysics.md#flux-limited-galaxy-selection) admits luminous objects from larger volumes: in Euclidean space $d_{\max}\propto L^{1/2}$ and $V_{\max}\propto L^{3/2}$. Thus observed [luminosity](../../astrophysics.md#luminosity) counts are weighted by $V_{\max}$. Even a nominal [standard candle](../../astrophysics.md#standard-candle) with intrinsic scatter is preferentially observed on its bright side near the limit; ignoring this can underestimate distances. A volume-limited sample or a justified $1/V_{\max}$ weighting helps, subject to completeness, geometry and evolution assumptions. Separately, [Eddington bias](../../causal-inference.md#eddington-bias) occurs when noise scatters a steeply rising population across a detection threshold: more faint objects enter than bright objects leave.

[Lutz-Kelker bias](../../astrophysics.md#lutz-kelker-bias) concerns noisy [stellar parallaxes](../../astrophysics.md#stellar-parallax) and population/selection weighting. Locally uniform spatial [density](../../fluid-mechanics.md#density) gives $p(r)\propto r^2$ and, by changing variables, $p(\varpi)\propto\varpi^{-4}$ over the model's valid finite range. More distant [stars](../../stellar-astrophysics.md#star) are available to scatter into a parallax-limited sample than nearby [stars](../../stellar-astrophysics.md#star) to scatter out. Inverting an uncertain parallax also introduces a distinct nonlinear-estimation problem. **There is no universal magnitude correction for every [star](../../stellar-astrophysics.md#star)**: spatial [density](../../fluid-mechanics.md#density), [luminosity](../../astrophysics.md#luminosity), [extinction](../../ecology.md#extinction) and how the sample was selected all matter. The classical treatment motivates this issue; it should not replace an explicit generative model.[PASP 85, 573–578; classical uniform-density calibration model](../../physics-bibliography.md#on-the-use-of-trigonometric-parallaxes-for-the-calibration-of-luminosity-systems-theory-by-t-e-lutz-and-d-h-kelker)

[Bayes' theorem](../../probability-theory.md#bayes-theorem) combines the measurement [likelihood function](../../maximum-likelihood-estimation.md#likelihood-function) with a justified [prior distribution](../../bayesian-statistics.md#prior-probability). For example, with a [Gaussian](../../probability-distribution.md#normal-distribution) parallax error and consistent distance/parallax units,

$$
p(r\mid\widehat\varpi)\propto
\exp\!\left[-\frac{(\widehat\varpi-1/r)^2}{2\sigma_\varpi^2}\right]p(r),\qquad r>0.
$$

A [proper distance prior for parallax inference](../../astrophysics.md#proper-distance-prior-for-parallax-inference) might have $p(r)\propto r^2e^{-r/L}$ with a justified scale $L$; extending $r^2$ to infinity gives an improper [posterior](../../bayesian-statistics.md#bayesian-posterior) here. Negative measured parallaxes remain valid noisy data. For [selection conditioning in Bayesian inference](../../bayesian-statistics.md#selection-conditioning-in-bayesian-inference), distinguish individual inference from population inference: if selection is determined entirely by the exact data already conditioned on, it adds no further information about that individual's parameters. For population parameters $\Lambda$, the selected-data [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) must instead include the detection normalization $\alpha(\Lambda)=\int S(d)p(d\mid\Lambda)\,dd$. Applying a cut twice is also an error.

Selection can depend on [surface brightness](../../astrophysics.md#surface-brightness), [angular resolution](../../astrophysics.md#angular-resolution), dust, sky coverage, colour and observing cadence as well as total flux. Crowding and unresolved binaries bias distance calibrators. Transit surveys favour large [planets](../../planetary-science.md#planet) and short periods, with an additional geometric transit probability approximately $R_\star/a$ for small [planets](../../planetary-science.md#planet) on circular orbits; injection/recovery tests quantify the remaining [transit survey completeness](../../exoplanet.md#transit-survey-completeness). Cluster catalogues select noisy mass proxies from a steep abundance distribution. Planck's 2013 SZ catalogue explicitly characterized detection completeness and reliability rather than identifying every detection with an unbiased mass census.[abstract and selection-function/completeness analysis, 2013 preprint](../../physics-bibliography.md#planck-2013-results-xxix-planck-catalogue-of-sunyaev-zeldovich-sources-by-planck-collaboration) Calibrators, artificial-source tests and a forward model of detection, measurement and follow-up are the practical checks on any correction.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [thermal Sunyaev-Zeldovich effect](../../cosmic-microwave-background.md#thermal-sunyaev-zeldovich-effect) is [inverse Compton scattering](../../mathematical-physics.md#inverse-compton-scattering) of [cosmic microwave background](../../cosmic-microwave-background.md) [photons](../../quantum-mechanics.md#photon) by hot cluster [electrons](../../physics.md#electron). For an [optically thin](../../astrophysics.md#optically-thin-medium), nonrelativistic thermal [plasma](../../physics.md#plasma-physics),

$$
y=\frac{\sigma_T}{m_ec^2}\int n_ek_BT_e\,dl,\qquad
\Delta I_\nu=I_0y\frac{x^4e^x}{(e^x-1)^2}\left[x\coth(x/2)-4\right],
\quad x=\frac{h\nu}{k_BT_{\rm CMB}},\quad I_0=\frac{2(k_BT_{\rm CMB})^3}{h^2c^2}.
$$

The [Compton y parameter](../../mathematical-physics.md#compton-y-parameter) measures the [electron](../../physics.md#electron) [pressure](../../pressure.md) column. The distortion is a decrement below roughly **217 GHz**, an increment above it, and has $\Delta T/T=-2y$ in the [Rayleigh-Jeans law](../../astrophysics.md#rayleigh-jeans-law) limit. Relativistic [electron](../../physics.md#electron) corrections modify the spectrum and null.[abstract and relativistic thermal-distortion calculation](../../physics-bibliography.md#relativistic-corrections-to-the-sunyaev-zel-dovich-effect-by-a-d-challinor-and-a-n-lasenby)

Multifrequency maps separate this spectrum from primary [Cosmic microwave background anisotropy](../../cosmic-microwave-background-anisotropy.md), radio sources and dust; atmospheric subtraction, beams and [calibration](../../differential-geometry.md#calibration-differential-geometry) require control. The [kinetic Sunyaev-Zeldovich effect](../../cosmic-microwave-background.md#kinetic-sunyaev-zeldovich-effect) has $\Delta T/T\simeq-\tau v_{\rm los}/c$ and a CMB-temperature-like spectrum, so it is both a contaminant and a peculiar-velocity probe. Planck demonstrated blind multifrequency cluster detection with external confirmation and a measured selection function.[abstract; multifrequency detection and catalogue validation](../../physics-bibliography.md#planck-2013-results-xxix-planck-catalogue-of-sunyaev-zeldovich-sources-by-planck-collaboration)

For a fixed physical [pressure](../../pressure.md) column, $y$ has **no ordinary [cosmological surface-brightness dimming](../../astrophysics.md#cosmological-surface-brightness-dimming)**: the distorted spectrum and CMB redshift together. The [integrated Compton parameter](../../mathematical-physics.md#integrated-compton-parameter) $Y=\int y\,d\Omega$ still scales as $D_A^{-2}$ for fixed integrated physical [pressure](../../pressure.md). SZ observations therefore find distant clusters and measure thermal [pressure](../../pressure.md); integrated $Y$ is a useful mass proxy, requiring [calibration](../../differential-geometry.md#calibration-differential-geometry) and a selection model for cosmological counts. X-ray emission scales approximately as $\int n_e^2\Lambda(T_e)dl$, while SZ scales as $\int n_eT_e dl$. Combining them and a measured [temperature](../../temperature.md) constrains [density](../../fluid-mechanics.md#density), depth and, with angular geometry, distance. [gas clumping factor](../../fluid-mechanics.md#gas-clumping-factor), asphericity, [temperature](../../temperature.md) structure and nonthermal support limit that inference.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An [astronomical interferometer](../../physical-optics.md#astronomical-interferometer) combines light from collectors separated by projected [interferometric baseline](../../astrophysics.md#interferometric-baseline) $\mathbf B$. For a distant, narrowband, spatially incoherent source, the [Van Cittert-Zernike theorem](../../physical-optics.md#van-cittert-zernike-theorem) gives normalized [complex visibility](../../astrophysics.md#complex-visibility)

$$
\mathcal V(\mathbf B/\lambda)=\frac{\int I(\boldsymbol\theta)e^{-2\pi i\mathbf B\cdot\boldsymbol\theta/\lambda}\,d^2\theta}{\int I(\boldsymbol\theta)\,d^2\theta}.
$$

The resolving scale is **$\lambda/B$**, while the individual collector and beam combiner restrict the field of view. Delay lines compensate geometric path differences. To see broadband fringes, residual [optical path length](../../physical-optics.md#optical-path-length) mismatch must lie within the [coherence length](../../physical-optics.md#optical-coherence-length) of order $\lambda^2/\Delta\lambda$; [fringe tracking](../../physical-optics.md#fringe-tracking) follows rapidly changing [atmospheric piston in interferometry](../../physical-optics.md#atmospheric-piston-in-interferometry). Baseline changes and [Earth-rotation aperture synthesis](../../astrophysics.md#earth-rotation-aperture-synthesis) sample additional [spatial frequencies](../../fourier-analysis.md#spatial-frequency).

For an ideal uniform circular [star](../../stellar-astrophysics.md#star) of full [angular diameter](../../geometry-and-topology.md#angular-diameter) $\Theta$,

$$
\mathcal V=\frac{2J_1(x)}x,\qquad x=\frac{\pi B\Theta}{\lambda},\qquad
\boxed{\Theta=1.2197\,\lambda/B_{\rm first\ null}}.
$$

Real [limb darkening](../../radiometry.md#limb-darkening) changes the conversion. Several baselines constrain binaries, [stellar radii](../../stellar-astrophysics.md#stellar-radius) and circumstellar structure; orbital angular separations combined with [radial velocities](../../euler-equations-for-an-inviscid-fluid.md#radial-velocity) can give physical orbital scales. [calibration](../../differential-geometry.md#calibration-differential-geometry) [stars](../../stellar-astrophysics.md#star) test contrast losses, alongside [wavelength](../../wave-equation.md#wavelength), photometric imbalance, [polarization](../../wave.md#polarization-waves) and [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) controls. For three collectors the [closure phase](../../physical-optics.md#closure-phase) cancels telescope-based phase errors: $\phi_{12}+\phi_{23}+\phi_{31}$ retains source asymmetry information. Sparse baseline coverage still leaves image/model ambiguities.

In [stellar intensity interferometry](../../quantum-optics.md#stellar-intensity-interferometry), thermal-light correlations instead give $g^{(2)}(0)-1=|g^{(1)}|^2$ for an ideal single-polarization resolved temporal mode. The Sirius experiment correlated separate detector outputs rather than optically combining the beams.[Nature 178, 1046–1048 (1956)](../../physics-bibliography.md#a-test-of-a-new-type-of-stellar-interferometer-on-sirius-by-robert-hanbury-brown-and-richard-quentin-twiss) Pure atmospheric phase shifts do not alter local [intensities](../../wave.md#intensity-physics), but finite detector [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) dilutes the correlation and [photon](../../quantum-mechanics.md#photon) statistics limit sensitivity; the two-detector observable also loses the complex phase.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[annual stellar parallax](../../astrophysics.md#stellar-parallax) uses the known Earth-orbit baseline, with **$d(\mathrm{pc})=1/\varpi(\mathrm{arcsec})$**. Repeated positions separate parallax from [proper motion](../../astronomy.md#proper-motion); [calibration](../../differential-geometry.md#calibration-differential-geometry) offsets, binarity and noisy-parallax selection require checks. Nearby [stars](../../stellar-astrophysics.md#star) calibrate absolute [luminosities](../../astrophysics.md#luminosity). Extinction-corrected [distance modulus](../../astrophysics.md#distance-modulus) then gives

$$
\boxed{m_\lambda-M_\lambda=5\log_{10}(d/10\,\mathrm{pc})+A_\lambda}.
$$

[main-sequence fitting](../../cosmology.md#main-sequence-fitting) compares a cluster sequence with nearby calibrated [stars](../../stellar-astrophysics.md#star); age, [metallicity](../../stellar-astrophysics.md#metallicity), reddening and unresolved binaries limit the match. [Cepheid variables](../../stellar-astrophysics.md#cepheid-variable) extend the range to nearby [galaxies](../../galaxy.md): measure periods and mean multiband magnitudes, calibrate the [Cepheid period-luminosity relation](../../stellar-astrophysics.md#cepheid-period-luminosity-relation), and correct for [extinction](../../ecology.md#extinction), [metallicity](../../stellar-astrophysics.md#metallicity), crowding and pulsation mode. [RR Lyrae stars](../../stellar-astrophysics.md#rr-lyrae-star) and the [tip of the red giant branch](../../cosmology.md#tip-of-the-red-giant-branch) provide complementary population-II routes with their own composition and [calibration](../../differential-geometry.md#calibration-differential-geometry) dependence.

Some anchors bypass intermediate rungs. An [eclipsing-binary distance](../../stellar-astrophysics.md#eclipsing-binary-distance) starts from a double-lined [eclipsing binary](../../stellar-astrophysics.md#eclipsing-binary): velocities give $a\sin i$; eclipses give inclination $i$ and relative radii $R/a$, hence physical radii. An independently calibrated surface-brightness/colour relation gives angular radii and distance; alternatively corrected bolometric flux satisfies $F_{\rm bol}=\sigma T_{\rm eff}^4(R/d)^2$ for a component. [temperature](../../temperature.md), [extinction](../../ecology.md#extinction), third light and surface-brightness [calibration](../../differential-geometry.md#calibration-differential-geometry) remain systematic errors. Eight late-type binaries gave a 2.2%-accuracy [LMC](../../galaxy.md#large-magellanic-cloud) anchor in 2013.[abstract, Nature 495, 76–79; photometric and orbital information](../../physics-bibliography.md#an-eclipsing-binary-distance-to-the-large-magellanic-cloud-accurate-to-two-per-cent-by-g-pietrzynski-and-others)

A [maser-disk geometric distance](../../cosmology.md#maser-disk-geometric-distance) uses water [masers](../../maser.md) orbiting in the nearly edge-on nuclear disk of [NGC 4258](../../galaxy.md#ngc-4258). [very-long-baseline interferometry](../../astrophysics.md#very-long-baseline-interferometry), Doppler velocities, [proper motions](../../astronomy.md#proper-motion) and accelerations constrain its orbit scale and distance. In an ideal circular, matched-radius example $R=v^2/a_{\rm orb}$ and $d=R/\theta$; real fits account for disk warp and different [maser](../../maser.md) locations. This geometric method calibrated an extragalactic distance independently of stellar [luminosities](../../astrophysics.md#luminosity).[abstract; orbital proper motions and accelerations, 1999](../../physics-bibliography.md#a-4-percent-geometric-distance-to-the-galaxy-ngc4258-from-orbital-motions-in-a-nuclear-gas-disk-by-j-r-herrnstein-and-others) These overlapping anchors cross-check the nearby-galaxy ladder; no Hubble-flow fit is needed here.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

[thermal bremsstrahlung](../../astrophysics.md#thermal-bremsstrahlung) is continuum radiation from [electrons](../../physics.md#electron) accelerated in ion electric fields. For [Maxwellian](../../boltzmann-equation.md#local-maxwellian) [electrons](../../physics.md#electron),

$$
j_\nu\propto n_e\sum_i Z_i^2n_i\,T_e^{-1/2}e^{-h\nu/(k_BT_e)}g_{\rm ff}.
$$

At high [frequency](../../wave.md#frequency) the exponential cutoff constrains $T_e$; X-ray fitting must also model foreground absorption, line emission, detector response and possible multitemperature or nonthermal components. At radio [frequencies](../../wave.md#frequency), $h\nu\ll k_BT_e$, an [optically thin](../../astrophysics.md#optically-thin-medium) free-free spectrum is almost flat, with the weak [frequency](../../wave.md#frequency) dependence set mainly by the [Gaunt factor](../../astrophysics.md#gaunt-factor).

For pure ionized hydrogen, radio [free-free opacity](../../stellar-structure.md#free-free-opacity) gives

$$
\tau_\nu\propto T_e^{-3/2}\nu^{-2}g_{\rm ff}\,\mathrm{EM},\qquad
\mathrm{EM}=\int n_e^2dl,\qquad
I_\nu=B_\nu(T_e)(1-e^{-\tau_\nu}).
$$

The turnover constrains [emission measure](../../astrophysics.md#emission-measure); a resolved, [optically thick](../../astrophysics.md#optically-thick-medium) source has [brightness temperature](../../exoplanet.md#brightness-temperature) approaching $T_e$. An unresolved source has an unknown beam [filling factor](../../quantum-theory.md#filling-factor-quantum-hall-effect), so its observed brightness need not equal its [electron](../../physics.md#electron) [temperature](../../temperature.md). Angular size and an independent distance give a geometric depth $L$; a uniform model then yields **$n_e=\sqrt{\mathrm{EM}/L}$**. Clumping instead measures a density-squared average, not the mean [density](../../fluid-mechanics.md#density).[chapter 4, equations (4.57)–(4.60); emission measure and thick/thin spectra](../../physics-bibliography.md#essential-radio-astronomy-by-james-j-condon-and-scott-m-ransom)

**A free-free spectrum alone does not uniquely determine [density](../../fluid-mechanics.md#density) and size.** The [density-depth degeneracy of free-free radiation](../../astrophysics.md#density-depth-degeneracy-of-free-free-radiation) is explicit: for a resolved uniform column, $n_e\mapsto qn_e$, $L\mapsto L/q^2$ leaves both emissivity-integrated brightness and [optical depth](../../astrophysics.md#optical-depth) unchanged at fixed [temperature](../../temperature.md). With independent SZ information and known $T_e$, the [electron](../../physics.md#electron) column is $N_e=ym_ec^2/(\sigma_Tk_BT_e)$; then

$$
\boxed{n_e=\mathrm{EM}/N_e,\qquad L=N_e^2/\mathrm{EM}}.
$$

These equalities require consistent composition and geometry, and uniform [density](../../fluid-mechanics.md#density) and [temperature](../../temperature.md). Relating $L$ to angular extent can give distance; asphericity and the [gas clumping factor](../../fluid-mechanics.md#gas-clumping-factor) are important limitations of this combined cluster method.

## ↑ Ancestors (11)

1. [2014](../2014.md)
2. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
3. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../university-of-cambridge.md#frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
