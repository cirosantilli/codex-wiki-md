# Paper 1

↑ **Parent:** [2016](../2016.md)

Original source: [Cambridge FOI 2023/399 released PDF, physical pages 807–809](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=807).

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Choose the baseline vector from the first [antenna](../../electrical-engineering.md#antenna-radio) to the second. Apart from a sign convention for receiver delay, the [geometric delay](../../astrophysics.md#geometric-delay) is $\tau_g=\mathbf b\cdot\mathbf s/c$, and the phase difference is $\phi=2\pi\nu\tau_g$. For equal received source powers $P_a$, adding the voltages and averaging over many wave periods gives

$$
P(t)=2P_a\{1+\cos[2\pi\nu\tau_g(t)+\phi_0]\}.
$$

Uncorrelated receiver noise adds a mean level but not the source's coherent cross term. For an east-west baseline and one choice of hour-angle sign, $\tau_g=(b/c)\cos\delta\sin H(t)$. Earth rotation therefore sweeps the phase; locally the fringe [frequency](../../wave.md#frequency) is $(b/\lambda)\cos\delta\cos H\,\dot H$. Tracking the [antenna](../../electrical-engineering.md#antenna-radio) pointing keeps the source in the [primary beam](../../astrophysics.md#primary-beam). Electronic [fringe stopping](../../astrophysics.md#fringe-stopping) is a separate operation: it can remove this phase evolution, making a source at the [phase centre](../../astrophysics.md#phase-centre) constant in the corrected [complex visibility](../../astrophysics.md#complex-visibility). The oscillating power above is the geometrical fringe before that correction.

<a id="1/image-projected-interferometer-baseline-geometric-delay-and-illustrative-fringes-before-electronic-fringe-stopping"></a>
![](../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1-interferometer-fringes.png)

**[Figure 1](#1/image-projected-interferometer-baseline-geometric-delay-and-illustrative-fringes-before-electronic-fringe-stopping). Projected interferometer baseline, geometric delay and illustrative fringes before electronic fringe stopping**.

For a small angular displacement $d\theta$ along the projected baseline, $d\phi=2\pi b_p\,d\theta/\lambda$. One full fringe therefore spans **$\Delta\theta\sim\lambda/b_p$**. Here $b_p=|\mathbf b-(\mathbf b\cdot\mathbf s)\mathbf s|$. This is the angular period of the measured Fourier component and the characteristic resolution scale when such long baselines are synthesized; precise beam width and image ambiguity also depend on baseline coverage and weighting. A single pair by itself does not give an unambiguous complete image.

Writing $x=h\nu/(k_BT)$, the expansion $e^x-1=x+O(x^2)$ immediately gives the [Rayleigh-Jeans law](../../astrophysics.md#rayleigh-jeans-law),

$$
\boxed{B_\nu\simeq\frac{2k_BT\nu^2}{c^2}\quad(h\nu\ll k_BT).}
$$

The factor two counts the two independent modes of [polarization of waves](../../wave.md#polarization-waves). A small brightness-temperature perturbation thus has $\Delta I_\nu=2k_B\nu^2\Delta T_{\rm RJ}/c^2$ in this limit.

Hot intracluster [electrons](../../physics.md#electron) inverse-Compton scatter the microwave-background [photons](../../quantum-mechanics.md#photon). The scattering [optical depth](../../astrophysics.md#optical-depth) is $d\tau=n_e\sigma_T\,dl$ and the characteristic thermal fractional energy transfer is of order $k_BT_e/(m_ec^2)$. The integrated distortion is therefore controlled by

$$
y=\int\frac{k_BT_e}{m_ec^2}n_e\sigma_T\,dl.
$$

Scattering conserves [photon number](../../quantum-harmonic-oscillator.md#photon-number) while shifting [photons](../../quantum-mechanics.md#photon) toward higher [frequencies](../../wave.md#frequency), giving a low-frequency decrement and a high-frequency increment. Thus the printed estimate correctly gives a negative change of order $yT_{\rm CMB}$. Its numerical coefficient, however, is not the standard Rayleigh-Jeans coefficient. For nonrelativistic [electrons](../../physics.md#electron) and small $y$, the [Kompaneets equation](../../mathematical-physics.md#kompaneets-equation) gives $\Delta n=y x^{-2}\partial_x(x^4\partial_x n_0)$. At small $x$, $n_0\simeq1/x$, so $\Delta n\simeq-2y/x$ and

$$
\boxed{\frac{\Delta T_{\rm RJ}}{T_{\rm CMB}}\simeq-2y.}
$$

Equivalently the thermodynamic-temperature spectral factor is $x\coth(x/2)-4\to-2$. The original PDF really prints the estimate with $-y$, not $-2y$; both numerical conventions are retained below. Relativistic corrections at the supplied $T_e$ are small compared with this factor-of-two difference.[abstract and Rayleigh-Jeans limit: the leading coefficient is minus twice the conventional Compton y parameter](../../physics-bibliography.md#relativistic-corrections-to-the-sunyaev-zel-dovich-effect-by-a-d-challinor-and-a-n-lasenby)

The uniform cube has a constant line-of-sight depth $L=6\times10^{22}\,\mathrm m$. Using the supplied cross-section rather than replacing it with a more precise value gives

$$
\tau=n_e\sigma_TL=8.04\times10^{-4},\qquad \frac{k_BT_e}{m_ec^2}=1.01\times10^{-2},\qquad y=8.14\times10^{-6}.
$$

Adopt $T_{\rm CMB}=2.72548\,\mathrm K$, explicitly an external measured constant, not a [temperature](../../temperature.md) supplied in the question. The values $k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}$, $c=299792458\,\mathrm{m\,s^{-1}}$ and $m_e\simeq9.10938\times10^{-31}\,\mathrm{kg}$ set the physical units. Hence **the printed relation gives $\Delta T\simeq-22\,\mathrm{\mu K}$; the standard Rayleigh-Jeans result gives $\Delta T\simeq-44\,\mathrm{\mu K}$**. Keeping the answer as $-8.14\times10^{-6}T_{\rm CMB}$, or twice that, avoids needing a numerical background [temperature](../../temperature.md).[abstract, literature-combined temperature $2.72548\pm0.00057$ K; adopted value rounded only at the end](../../physics-bibliography.md#the-temperature-of-the-cosmic-microwave-background-by-dale-j-fixsen)

The face is a square, so its [solid angle](../../euclidean-geometry.md#solid-angle) is $\Omega=(6\pi/10800)^2=3.046\times10^{-6}\,\mathrm{sr}$, not the area of a circular six-arcminute aperture. At $15\,\mathrm{GHz}$,

$$
\Delta S_\nu=\int\Delta I_\nu\,d\Omega\simeq\frac{2k_B\nu^2}{c^2}\Delta T\,\Omega.
$$

Thus **$\Delta S_\nu\simeq-4.67\times10^{-4}\,\mathrm{Jy}=-0.47\,\mathrm{mJy}$ using the printed estimate**, or **$-0.93\,\mathrm{mJy}$ using the standard factor two**. The sign denotes missing brightness relative to the surrounding microwave background. At this [frequency](../../wave.md#frequency) $h\nu/(k_BT_{\rm CMB})\simeq0.264$; the exact nonrelativistic spectral intensity differs from the strict Rayleigh-Jeans approximation by about one percent. This precision does not affect the estimates.

For the array noise, the [system temperature](../../astrophysics.md#system-temperature) sets the receiver noise scale; let $A_e=\eta_A\pi d^2/4$ be the effective area of each dish, and let $\eta_c$ describe correlation losses. No efficiencies or [polarization of waves](../../wave.md#polarization-waves) count are supplied, so first take $\eta_A=\eta_c=1$ and a single independent [polarization of waves](../../wave.md#polarization-waves). An unpolarized [point source](../../fluid-mechanics.md#point-source) produces [antenna](../../electrical-engineering.md#antenna-radio) [temperature](../../temperature.md) $T_a=S_\nu A_e/(2k_B)$, and the [system-equivalent flux density](../../astrophysics.md#system-equivalent-flux-density) is $\mathrm{SEFD}=2k_BT_{\rm sys}/A_e$. The [interferometric radiometer equation](../../astrophysics.md#interferometric-radiometer-equation) gives one baseline an rms flux error $\mathrm{SEFD}/\sqrt{2\Delta\nu t}$. There are $N(N-1)/2=45$ cross-correlation baselines; averaging their independent [thermal noise](../../electrical-engineering.md#thermal-noise) for a [point source](../../fluid-mechanics.md#point-source) gives

$$
\sigma_S=\frac{2k_BT_{\rm sys}}{A_e\eta_c\sqrt{n_{\rm pol}N(N-1)\Delta\nu t}}.
$$

The ideal single-dish effective area is $4\pi\,\mathrm{m^2}$, giving $\mathrm{SEFD}=6.59\times10^3\,\mathrm{Jy}$ and

$$
\boxed{\sigma_S\simeq9.0\times10^{-6}\,\mathrm{Jy}=9.0\,\mathrm{\mu Jy}\quad(n_{\rm pol}=1).}
$$

Combining two independent parallel-hand [polarization of waves](../../wave.md#polarization-waves) measurements gives $6.3\,\mathrm{\mu Jy}$. Nonunit efficiencies increase these estimates by $1/(\eta_A\eta_c)$. Here signal equal to noise means a weak-source [signal-to-noise ratio](../../electrical-engineering.md#signal-to-noise-ratio) of one after integration; it does not mean equating the source to the entire unaveraged receiver-noise power.[2004 Synthesis Imaging Summer School, slides 6–12 and 20: SEFD, independent baseline noise and single-polarization synthesis-image sensitivity](../../physics-bibliography.md#sensitivity-by-joan-wrobel)

At the band centre, $\lambda=0.01999\,\mathrm m$. Taking a representative maximum projected baseline of $20\,\mathrm m$ gives **$\theta_{\rm res}\sim3.4$ arcminutes**. A corner-to-corner baseline of $20\sqrt2\,\mathrm m$ would give about $2.4$ arcminutes before projection and weighting. The exact [antenna](../../electrical-engineering.md#antenna-radio) locations and source declination are not supplied, so neither a unique [synthesized beam](../../astrophysics.md#synthesized-beam) shape nor an exact FWHM is determined. The individual-dish primary-beam scale, roughly $\lambda/4\,\mathrm m\sim17$ arcminutes, is the field of view, not the synthesized resolution.

To extract the cluster signal, retain frequency-resolved [complex visibilities](../../astrophysics.md#complex-visibility) and fit an extended SZ template together with contaminating compact sources. For the ideal uniform square centred at the [phase centre](../../astrophysics.md#phase-centre) and with a nearly constant [primary beam](../../astrophysics.md#primary-beam) across it, the [Fourier transform](../../fourier-transform.md) is

$$
V(u,v)=\Delta S_\nu\,\operatorname{sinc}(\pi\Theta u)\operatorname{sinc}(\pi\Theta v),\qquad \operatorname{sinc}x=\frac{\sin x}{x},\qquad\Theta=6\ \text{arcminutes in radians}.
$$

This is why the integrated decrement must not be treated as a point-source flux on every baseline. The first axial visibility null occurs at $b=\lambda/\Theta\simeq11.5\,\mathrm m$. Short baselines carry most of the large-scale decrement; the longest baselines are useful for separating unresolved positive radio sources. [natural visibility weighting](../../astrophysics.md#natural-visibility-weighting) or a suitable taper gives a clearer extended-source image than emphasizing the longest baselines, while a [visibility-domain matched filter](../../electrical-engineering.md#visibility-domain-matched-filter) uses all samples with weights proportional to template amplitude divided by noise [variance](../../variance.md). Its amplitude estimate is $\widehat a=\operatorname{Re}(T^\dagger C^{-1}d)/(T^\dagger C^{-1}T)$ for a real template amplitude. A joint fit propagates radio-source uncertainty instead of subtracting exact, noise-free source models.

<a id="1/image-normalized-visibilities-of-the-six-arcminute-square-cluster-and-their-suppression-on-long-baselines"></a>
![](../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1-square-cluster-visibility.png)

**[Figure 2](#1/image-normalized-visibilities-of-the-six-arcminute-square-cluster-and-their-suppression-on-long-baselines). Normalized visibilities of the six-arcminute square cluster and their suppression on long baselines**.

Earth-rotation and multifrequency synthesis improve Fourier coverage, but each channel must use its own baseline in [wavelengths](../../wave-equation.md#wavelength), [primary beam](../../astrophysics.md#primary-beam) and SZ spectrum. Use the longer baselines and spectra to identify variable [point sources](../../fluid-mechanics.md#point-source), flag bad data, and test the decrement with time, [antenna](../../electrical-engineering.md#antenna-radio) and [frequency](../../wave.md#frequency) splits. Primary-beam and absolute-flux [calibration](../../differential-geometry.md#calibration-differential-geometry) must be included. Large-scale microwave-background fluctuations and residual ground or atmospheric signals can remain even below the thermal-noise estimate. The narrow low-frequency band alone gives limited separation of SZ and primary microwave-background [temperature](../../temperature.md) structure. There is no zero-spacing interferometric datum: integrated flux is model dependent unless sufficiently short baselines or additional total-power information are available. Exact cluster detection significance cannot be obtained from the point-source noise alone without the actual projected baseline distribution and weighting.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For data $D$, parameters $\theta$ and model $M$, [conditional probability](../../probability-theory.md#conditional-probability) gives

$$
\boxed{p(\theta\mid D,M)=\frac{p(D\mid\theta,M)\,p(\theta\mid M)}{p(D\mid M)},\qquad p(D\mid M)=\int p(D\mid\theta,M)p(\theta\mid M)\,d\theta.}
$$

The [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) describes the measurement process, the [prior](../../bayesian-statistics.md#prior-probability) encodes parameter information before these data, and the [Bayesian evidence](../../bayesian-statistics.md#bayesian-model-evidence) normalizes the [posterior](../../bayesian-statistics.md#bayesian-posterior). A [prior](../../bayesian-statistics.md#prior-probability) is a [probability density](../../wave-function.md#probability-density) with respect to a specified measure; a uniform [prior](../../bayesian-statistics.md#prior-probability) in distance is not uniform in parallax. [Bayes' theorem](../../probability-theory.md#bayes-theorem) combines [conditional probabilities](../../probability-theory.md#conditional-probability) and does not itself select an appropriate [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) or [prior](../../bayesian-statistics.md#prior-probability).

An astronomical application starts with a forward model. For measured fluxes $d_i$ with predictions $f_i(\theta)$ and known Gaussian covariance $C$, $L\propto|C|^{-1/2}\exp[-(d-f)^{\mathsf T}C^{-1}(d-f)/2]$. Correlated [calibration](../../differential-geometry.md#calibration-differential-geometry) errors belong in $C$ or in explicit [calibration](../../differential-geometry.md#calibration-differential-geometry) [nuisance parameters](../../statistical-model.md#nuisance-parameter); assuming every filter or epoch is independent can give falsely narrow uncertainties. For a faint photon-counting source, the more appropriate [likelihood](../../maximum-likelihood-estimation.md#likelihood-function) can instead be $p(N\mid s,b)=e^{-(s+b)}(s+b)^N/N!$, with nonnegative expected source and background counts. Background measurements constrain $b$, which is then marginalized rather than set to an exact subtracted number. The observed background-subtracted count can be negative even though the physical expected source count is nonnegative.

For a simple flux example with $d\mid F\sim\mathcal N(F,\sigma^2)$ and a Gaussian [calibration](../../differential-geometry.md#calibration-differential-geometry) [prior](../../bayesian-statistics.md#prior-probability) $F\sim\mathcal N(F_0,\sigma_0^2)$, completing the square gives

$$
\sigma_p^{-2}=\sigma^{-2}+\sigma_0^{-2},\qquad F_p=\sigma_p^2\left(\frac d{\sigma^2}+\frac{F_0}{\sigma_0^2}\right).
$$

This explicitly shows how independent information combines. A physical nonnegative-flux [prior](../../bayesian-statistics.md#prior-probability) would truncate or replace that illustrative Gaussian [prior](../../bayesian-statistics.md#prior-probability). Photometric-redshift fitting similarly compares predicted [galaxy](../../galaxy.md) colours with measured fluxes, then integrates over [luminosity](../../astrophysics.md#luminosity), dust and other [nuisance parameters](../../statistical-model.md#nuisance-parameter) to obtain $p(z\mid D)$. Multimodal [posteriors](../../bayesian-statistics.md#bayesian-posterior) should be retained when different spectral features produce similar colours; a best fit alone hides that ambiguity. The same framework applies to orbit parameters, stellar [temperatures](../../temperature.md), cosmological parameters and cluster SZ amplitudes.

[credible intervals](../../bayesian-statistics.md#credible-interval) state [posterior](../../bayesian-statistics.md#bayesian-posterior) [probability](../../probability-theory.md#probability) conditional on the model and [prior](../../bayesian-statistics.md#prior-probability). [posterior predictive checks](../../bayesian-statistics.md#posterior-predictive-check) compare replicated observations with the data and can reveal a deficient noise or source model. Sensitivity to plausible [priors](../../bayesian-statistics.md#prior-probability) is especially important for weak signals and inverse problems. For competing models, [posterior](../../bayesian-statistics.md#bayesian-posterior) odds equal [prior](../../bayesian-statistics.md#prior-probability) odds times the [Bayes factor](../../bayesian-statistics.md#bayes-factor) $Z_1/Z_2$; the evidence averages fit quality over the [prior](../../bayesian-statistics.md#prior-probability) volume and therefore depends on proper, physically justified [prior](../../bayesian-statistics.md#prior-probability) ranges. Detection thresholds and catalogue selection must enter the sampling model when inferring a population, otherwise a carefully calculated [posterior](../../bayesian-statistics.md#bayesian-posterior) can still describe a biased sample. **The practical gain is a joint uncertainty distribution with [nuisance parameters](../../statistical-model.md#nuisance-parameter) propagated, not merely a single fitted number.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Atmospheric refractive-index fluctuations impose a changing phase screen on the pupil. For a [telescope](../../physics.md#telescope) much larger than the [Fried parameter](../../optics.md#fried-parameter) $r_0$, long-exposure resolution is approximately $0.98\lambda/r_0$, rather than the [diffraction](../../quantum-scattering.md#diffraction) scale $\lambda/D$. The scaling $r_0\propto\lambda^{6/5}$ makes the [seeing](../../optics.md#astronomical-seeing) width proportional to $\lambda^{-1/5}$ for fixed turbulence. An [atmospheric coherence time](../../optics.md#atmospheric-coherence-time) sets the exposure or correction cadence needed to freeze the phase, while the [isoplanatic angle](../../optics.md#isoplanatic-angle) sets the useful angular separation from a reference source. These are atmospheric quantities, not improvements automatically supplied by a larger [mirror](../../optical-instrument.md#mirror).

First reduce avoidable turbulence: choose a good high site, control [mirror](../../optical-instrument.md#mirror) and enclosure [temperatures](../../temperature.md), ventilate the dome, and observe when the [line of sight](../../astrophysics.md#line-of-sight) crosses less turbulent air. Guiding removes [telescope](../../physics.md#telescope) drift, and a fast tip-tilt correction removes image motion. Slow [active optics](../../optical-instrument.md#active-optics) corrects [mirror](../../optical-instrument.md#mirror) figure and alignment; it cannot by itself follow all atmospheric phase fluctuations. These measures improve the input wavefront but do not guarantee diffraction-limited performance.

In [adaptive optics](../../optical-instrument.md#adaptive-optics), a [wavefront sensor](../../optical-instrument.md#wavefront-sensor) measures the reference-star wavefront, a reconstructor estimates its aberration, and a fast control loop commands a [deformable mirror](../../optical-instrument.md#deformable-mirror) and tip-tilt element. A Shack-Hartmann sensor obtains local slopes from the displacement of focused lenslet spots. The science beam receives the corresponding optical-path correction. Residual phase [variance](../../variance.md) limits the [Strehl ratio](../../point-spread-function.md#strehl-ratio) approximately as $S\simeq e^{-\sigma_\phi^2}$ when the residual is small. Enough corrected spatial modes, adequate reference [photons](../../quantum-mechanics.md#photon) and a response faster than atmospheric changes are all needed. [infrared](../../optics.md#infrared) correction is easier because a given path error has smaller phase in radians and the atmospheric coherence length is larger. A faint or distant [guide star](../../optical-instrument.md#guide-star-adaptive-optics) leaves larger errors and a core-plus-halo [point spread function](../../point-spread-function.md). The NACO manual documents these reference-star and anisoplanatic limitations.[§§3.1–3.2, printed p.13; §4.3, printed p.19: atmospheric coherence, real-time correction and anisoplanatism](../../physics-bibliography.md#naco-user-manual-by-european-southern-observatory)

A [laser guide star](../../optical-instrument.md#laser-guide-star) supplies a wavefront reference in fields lacking a bright suitable star, but a finite-altitude beacon samples a cone rather than the full stellar cylinder. It also does not by itself supply the absolute celestial tip-tilt reference; a natural source is still required for that measurement. Multiple [guide stars](../../optical-instrument.md#guide-star-adaptive-optics) and conjugate correction planes can improve wider-field compensation, with greater hardware and reconstruction demands. The [point spread function](../../point-spread-function.md) can vary across the field and with time, so reference stars and telemetry are needed to calibrate [astrometry](../../astronomy.md#astrometry) and [photometry](../../optics.md#photometry-optics); a sharper image alone is not a guarantee of accurate science.[Laser guide stars: artificial reference sources, limited sky coverage and retained natural-star requirements](../../physics-bibliography.md#adaptive-optics-by-european-southern-observatory)

Short-exposure methods provide another route. Exposures shorter than the [atmospheric coherence time](../../optics.md#atmospheric-coherence-time) freeze [speckle patterns](../../physical-optics.md#speckle-pattern). [speckle interferometry](../../optics.md#speckle-interferometry) uses calibrated Fourier statistics of many frames to recover diffraction-scale information; phase information requires methods such as [bispectrum](../../time-series.md#bispectrum) reconstruction, not just averaging the blurred frames. [lucky imaging](../../optics.md#lucky-imaging) selects the best short frames, registers them and combines them. It sacrifices [photons](../../quantum-mechanics.md#photon) through selection and can be read-noise limited for faint targets, so it is most effective with enough reference [photons](../../quantum-mechanics.md#photon). Ordinary shift-and-add mainly corrects motion; it does not remove every high-order phase error. Deconvolution using a measured [point spread function](../../point-spread-function.md) can recover supported structure but amplifies noise and cannot reliably invent [spatial frequencies](../../fourier-analysis.md#spatial-frequency) absent from the observations. **Good-site engineering, fast wavefront correction and short-exposure reconstruction address different limitations and can be combined.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

An [electron](../../physics.md#electron) accelerated in an [ion](../../chemistry.md#ion)'s Coulomb field emits [bremsstrahlung](../../electromagnetic-radiation.md#bremsstrahlung). Both [electron](../../physics.md#electron) states are unbound, giving free-free radiation rather than a discrete bound-state line. Averaging over a Maxwellian [electron](../../physics.md#electron) distribution gives an optically thin spectral emissivity with dependence

$$
j_\nu=C_{\rm ff}Z^2n_en_iT^{-1/2}e^{-h\nu/(k_BT)}\bar g_{\rm ff}(\nu,T).
$$

Here $C_{\rm ff}$ depends on the emissivity convention, and the [Gaunt factor](../../astrophysics.md#gaunt-factor) supplies the quantum correction. No numerical emissivity normalization is needed for these diagnostics. For a mixture, sum $Z_i^2n_i$ over [ion](../../chemistry.md#ion) species. The bolometric emissivity is proportional to $n_e\sum Z_i^2n_i\,T^{1/2}$ with a frequency-averaged [Gaunt factor](../../astrophysics.md#gaunt-factor). Thermal [electron](../../physics.md#electron) speeds control the spectrum while the encounter rate supplies its density-squared dependence.

[temperature](../../temperature.md) can be measured from the high-energy exponential cutoff at [photon](../../quantum-mechanics.md#photon) energy of order $k_BT$, provided the spectrum spans that turnover and foreground absorption and nonthermal contamination are modelled. At radio [frequencies](../../wave.md#frequency) $h\nu\ll k_BT$, the exponential is nearly one, so the optically thin continuum is a poor thermometer by slope alone. Kirchhoff's law, $\alpha_\nu=j_\nu/B_\nu$, and the [Rayleigh-Jeans law](../../astrophysics.md#rayleigh-jeans-law) give $\alpha_\nu\propto n_en_iT^{-3/2}\nu^{-2}\bar g_{\rm ff}$ for an isothermal thermal [plasma](../../physics.md#plasma-physics). The transfer solution is

$$
I_\nu=B_\nu(T)(1-e^{-\tau_\nu}),\qquad T_b\simeq T(1-e^{-\tau_\nu})
$$

in the radio limit. A resolved optically thick region therefore measures its [electron](../../physics.md#electron) [temperature](../../temperature.md) through [brightness temperature](../../exoplanet.md#brightness-temperature), if it fills the beam. The turnover between thick and thin emission constrains the line-of-sight [emission measure](../../astrophysics.md#emission-measure) $\mathrm{EM}=\int n_e^2dl$ for a hydrogen-dominated fully ionized [plasma](../../physics.md#plasma-physics). In the thin regime $T_b\simeq T\tau_\nu$, rather than $T_b=T$. The slowly varying [Gaunt factor](../../astrophysics.md#gaunt-factor) gives a nearly flat optically thin radio flux-density spectrum, in contrast to the $\nu^2$ thick limit at fixed projected area.[chapter 4, §4.3, especially equations (4.57)–(4.58): emission measure, absorption and optically thick/thin diagnostics](../../physics-bibliography.md#essential-radio-astronomy-by-james-j-condon-and-scott-m-ransom)

To obtain [density](../../fluid-mechanics.md#density), one also needs geometry. An angular extent and independent distance give a transverse size; an assumed shape provides a depth or volume. For approximately uniform emitting gas with [astrophysical volume filling factor](../../astrophysics.md#astrophysical-volume-filling-factor) $f_V$, $L_{\rm ff}\propto n_e^2 f_VVT^{1/2}$, so $n_e\propto[L_{\rm ff}/(f_VVT^{1/2})]^{1/2}$. Alternatively a measured column [emission measure](../../astrophysics.md#emission-measure) and assumed path length give an rms [density](../../fluid-mechanics.md#density). Clumping raises the mean squared [density](../../fluid-mechanics.md#density) relative to the square of the mean: the inferred value is not automatically the mean gas [density](../../fluid-mechanics.md#density). **Free-free brightness alone does not uniquely determine [temperature](../../temperature.md), [density](../../fluid-mechanics.md#density) and physical size.** Resolved imaging, a distance, optical-depth information or an independent column-density diagnostic is needed to remove those degeneracies. Cluster SZ data are complementary because their leading signal depends on $\int n_eT_e\,dl$, whereas free-free emission depends on [density](../../fluid-mechanics.md#density) squared. Metal lines, unresolved [temperature](../../temperature.md) structure, foreground absorption, synchrotron emission and [background subtraction](../../optical-instrument.md#background-subtraction) must be controlled before attributing the continuum to a single thermal component.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Type Ia supernovae are [standardizable candles](../../astrophysics.md#standardizable-candle). Repeated multiband [photometry](../../optics.md#photometry-optics) measures peak [apparent magnitude](../../astrophysics.md#apparent-magnitude), light-curve width and colour; spectra identify the supernova class and determine [redshift](../../optics.md#redshift), often from the host [galaxy](../../galaxy.md). Nearby objects calibrate the relation between light-curve shape, colour and absolute [luminosity](../../astrophysics.md#luminosity). Applying those relations produces a corrected [apparent magnitude](../../astrophysics.md#apparent-magnitude) $m_{\rm corr}$, not an assumption that every event has identical [luminosity](../../astrophysics.md#luminosity). The [distance modulus](../../astrophysics.md#distance-modulus) then gives

$$
\mu=m_{\rm corr}-M=5\log_{10}\left(\frac{d_L}{\mathrm{Mpc}}\right)+25.
$$

A common uncertainty in $M$ is degenerate with the absolute distance scale, but does not erase the redshift-dependent shape of the [Hubble diagram](../../cosmology.md#hubble-diagram).

[luminosity distance](../../cosmology.md#luminosity-distance) probes the expansion history. In a spatially flat model,

$$
d_L(z)=(1+z)c\int_0^z\frac{dz'}{H(z')},\qquad d_L(z)=\frac c{H_0}\left[z+\frac{1-q_0}{2}z^2+O(z^3)\right],\qquad q_0=-\frac{a\ddot a}{\dot a^2}\bigg|_0.
$$

For fixed low-redshift [calibration](../../differential-geometry.md#calibration-differential-geometry), a negative $q_0$ increases the second-order distance relative to a decelerating model. Objects at a given [redshift](../../optics.md#redshift) are therefore fainter. A [Hubble diagram](../../cosmology.md#hubble-diagram) spanning enough [redshift](../../optics.md#redshift) can distinguish this curvature from the common magnitude intercept. In matter-plus-cosmological-constant models, $q_0=\Omega_m/2-\Omega_\Lambda$; fitting the distances can test whether $q_0<0$. The two original supernova teams found distances supporting an accelerating expansion in that framework.[abstract and cosmological interpretation of standardized supernova luminosity distances](../../physics-bibliography.md#observational-evidence-from-supernovae-for-an-accelerating-universe-and-a-cosmological-constant-by-adam-riess-and-others)[abstract; cosmological likelihood constraints and tests of systematic uncertainty](../../physics-bibliography.md#measurements-of-omega-and-lambda-from-42-high-redshift-supernovae-by-saul-perlmutter-and-others)

The comparison requires matched rest-frame passbands and [K corrections](../../astrophysics.md#k-correction), correction for [redshift](../../optics.md#redshift) time dilation in the [light curves](../../astrophysics.md#light-curve), a common [photometric calibration](../../optics.md#photometric-calibration), and explicit uncertainty propagation. Dust [extinction](../../ecology.md#extinction) can imitate dimming; multicolour and [infrared](../../optics.md#infrared) observations test reddening and the adopted [extinction](../../ecology.md#extinction) law. Evolution in the progenitor population or host-galaxy dependence can alter standardization, so one compares matched populations and fits host-dependent terms where warranted. Flux-limited discovery introduces [Malmquist bias](../../astrophysics.md#malmquist-bias) and other selection effects, which must be modelled through the survey detection efficiency. [peculiar velocities](../../cosmology.md#peculiar-velocity) matter at low [redshift](../../optics.md#redshift), while [gravitational lensing](../../gravitational-lensing.md) and intrinsic scatter broaden the distant sample. Classification and outlier tests reduce contamination by other transient types.

Independent data reductions, nearby anchors, spectroscopic checks and a fit over the full [redshift](../../optics.md#redshift) range distinguish an expansion-history signal from one instrumental offset. Complementary cosmological observations help separate matter [density](../../fluid-mechanics.md#density), curvature and dark-energy parameters. **The acceleration inference comes from the relative distance-redshift relation, conditional on standardization and an expansion model.** Distant supernovae integrate the past expansion history; they do not directly measure the instantaneous second time derivative of today's [scale factor](../../cosmology.md#scale-factor-cosmology) without such modelling.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In a [CCD](../../optical-instrument.md#charge-coupled-device), absorbed optical [photons](../../quantum-mechanics.md#photon) create photoelectrons collected in electrostatic wells beneath gate electrodes. During readout, clock voltages move the charge packets row by row into a serial register; serial clocks move them one [pixel](../../computer-graphics.md#pixel) at a time to an output node. The node converts charge to a voltage, approximately $\Delta V=Q/C$, which is amplified and digitized. [pixel](../../computer-graphics.md#pixel) addresses are recovered from the row and serial-clock sequence. Resetting and sampling the output between packets establishes the baseline. Efficient transfer preserves charge; trapping or incomplete transfer produces loss and trailing. This is [CCD clocked charge transfer](../../optical-instrument.md#ccd-clocked-charge-transfer), not independent wiring of an [amplifier](../../electrical-circuit.md#amplifier) to every imaging [pixel](../../computer-graphics.md#pixel).[§7, SIS: charge generation, electrode-clock transfer and preamplifier readout](../../physics-bibliography.md#asca-technical-description-sis-by-nasa-heasarc)

[dark current](../../optical-instrument.md#dark-current-physics) is thermally generated charge accumulated even without illumination. If its mean rate is $d$ [electrons](../../physics.md#electron) per [pixel](../../computer-graphics.md#pixel) per second, a single exposure adds mean $dt$ and Poisson [variance](../../variance.md) $dt$. Cooling the detector and using low-defect material suppresses this generation. A dark [calibration](../../differential-geometry.md#calibration-differential-geometry) removes the reproducible mean pattern, but cannot remove the dark [electrons](../../physics.md#electron)' random [shot noise](../../electrical-engineering.md#shot-noise) in the science exposure. [read noise](../../optical-instrument.md#read-noise) comes from measuring the output packet and resetting the sense node, [amplifiers](../../electrical-circuit.md#amplifier) and electronics; write its rms as $r$ [electrons](../../physics.md#electron) per read. [correlated double sampling](../../optical-instrument.md#correlated-double-sampling) reduces reset and correlated offsets by subtracting the baseline measurement from the signal measurement. Low-noise electronics and an appropriate slower readout reduce the remaining contribution. The [CCD noise budget](../../optical-instrument.md#ccd-noise-budget) for $M$ separate exposures combined over total time $t$ contains independent dark and read contributions $dt+Mr^2$, not $(dt)^2+M^2r^2$. Long exposures reduce repeated [read noise](../../optical-instrument.md#read-noise), but saturation, cosmic rays and tracking requirements constrain the exposure length. On-chip binning can reduce read-noise penalties for a fixed binned area at the cost of angular sampling.

For the source and sky calculation, define the count conversion factor $K=At\Delta\nu/(h\nu)$ and the source flux per [pixel](../../computer-graphics.md#pixel) $s_\nu=F_\nu/N_{\rm pix}$. The ideal source and background [electron](../../physics.md#electron) counts are $S=Ks_\nu$ and $B=Kb_\nu\Omega_{\rm pix}$. These assume unit throughput and [quantum efficiency](../../optical-instrument.md#quantum-efficiency), approximately constant quantities across the band and a well-determined mean sky level from many background [pixels](../../computer-graphics.md#pixel). Source and sky [photons](../../quantum-mechanics.md#photon) have independent Poisson fluctuations, so the [variance](../../variance.md) after subtracting that mean sky is $S+B$. Subtracting a background removes its mean, not its [photon](../../quantum-mechanics.md#photon) noise. Therefore

$$
R=\frac S{\sqrt{S+B}}=\frac{F_\nu}{N_{\rm pix}}\left[\frac{At\Delta\nu}{h\nu(F_\nu/N_{\rm pix}+b_\nu\Omega_{\rm pix})}\right]^{1/2}.
$$

Thus **the required expression follows directly from adding photon-count [variances](../../variance.md)**. Finite sky-estimation noise, [dark current](../../optical-instrument.md#dark-current-physics) and [read noise](../../optical-instrument.md#read-noise) would add further [variance](../../variance.md). A nonunit common efficiency replaces $A$ by the effective collecting area; a nonflat spectrum requires the corresponding [frequency](../../wave.md#frequency) integral. For example, estimating the sky from one equally exposed background [pixel](../../computer-graphics.md#pixel) would add an extra $B$, whereas a large sky region makes that extra term small.

With $A=\pi(1\,\mathrm m)^2$ and the supplied [photon](../../quantum-mechanics.md#photon) [frequency](../../wave.md#frequency), the sky flux per [pixel](../../computer-graphics.md#pixel) is $b_\nu\Omega_{\rm pix}=1.75\times10^{-32}\,\mathrm{W\,m^{-2}\,Hz^{-1}}$. Multiplying arcsecond-squared [pixel](../../computer-graphics.md#pixel) area by brightness per arcsecond squared already gives a flux: no additional steradian conversion belongs in this product. Rearranging gives

$$
\frac t{R^2}=\frac{h\nu}{A\Delta\nu}\frac{F_\nu/N_{\rm pix}+b_\nu\Omega_{\rm pix}}{(F_\nu/N_{\rm pix})^2}.
$$

Using $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$ yields

<a id="3/table-ideal-per-pixel-source-and-sky-rates-and-exposure-divided-by-squared-signal-to-noise-ratio"></a>
| $F_\nu\ (\mathrm{W\,m^{-2}\,Hz^{-1}})$ | Source rate per [pixel](../../computer-graphics.md#pixel) $\mathrm{s^{-1}}$ | Sky rate per [pixel](../../computer-graphics.md#pixel) $\mathrm{s^{-1}}$ | $t/R^2\ (\mathrm s)$ |
| --- | --- | --- | --- |
| $10^{-29}$ | $98.8$ | $13.8$ | **$0.0115$** |
| $10^{-30}$ | $9.88$ | $13.8$ | **$0.243$** |
| $10^{-31}$ | $0.988$ | $13.8$ | **$15.2$** |

The first case is mainly source-shot-noise limited, while the last is strongly sky limited. At high source brightness $t/R^2\propto F_\nu^{-1}$; at low source brightness it approaches $F_\nu^{-2}$. Reducing source flux by ten can therefore require nearly a hundred times the exposure once sky noise dominates. These are per-pixel values for the ideal model, not guaranteed integration times including [calibration](../../differential-geometry.md#calibration-differential-geometry), cosmic rays or [read noise](../../optical-instrument.md#read-noise).

Increasing the diameter increases both source and sky [photon](../../quantum-mechanics.md#photon) rates as $D^2$ for fixed angular [pixels](../../computer-graphics.md#pixel). In this ideal limit the required exposure decreases as $D^{-2}$, whereas the stated [telescope](../../physics.md#telescope) cost increases as $D^{2.5}$: collecting area grows only as cost to the power $0.8$. A larger ground [telescope](../../physics.md#telescope) does not remove atmospheric [photons](../../quantum-mechanics.md#photon) or recover arbitrary wavefront information lost in a long seeing-limited exposure. Space observations avoid atmospheric airglow, weather and [atmospheric turbulence](../../optics.md#atmospheric-turbulence), and offer stable high-resolution imaging and access to very faint structure. They still have zodiacal light, instrumental backgrounds and their own [calibration](../../differential-geometry.md#calibration-differential-geometry) limits. [adaptive optics](../../optical-instrument.md#adaptive-optics) can provide excellent ground-based resolution in suitable fields, but its guide-star, [wavelength](../../wave-equation.md#wavelength) and field-dependent limitations do not remove the need for space-based continuum imaging. **The need is for complementary low-background, stable and high-resolution measurements; the cost exponent alone is not a proof that every imaging programme is cheaper in space.**

For X rays, one fully absorbed [photon](../../quantum-mechanics.md#photon) produces many [electron-hole pairs](../../quantum-mechanics.md#electron-hole-pair) in [silicon](../../chemical-substance.md#silicon), rather than one optical photoelectron count. At moderate [surface brightness](../../astrophysics.md#surface-brightness), the [probability](../../probability-theory.md#probability) of two [photons](../../quantum-mechanics.md#photon) landing in the same event island during one [CCD](../../optical-instrument.md#charge-coupled-device) frame is small. The charge packet or sum over neighbouring split-event [pixels](../../computer-graphics.md#pixel) then supplies a pulse height for each [photon](../../quantum-mechanics.md#photon), while its [pixel](../../computer-graphics.md#pixel) position supplies the image coordinate. Calibrating pulse height against energy produces an event list from which a spectrum can be accumulated for any spatial region. [photon pile-up](../../optical-instrument.md#photon-pile-up) at larger occupancies merges [photon](../../quantum-mechanics.md#photon) energies and corrupts both spectra and event grades, so fast enough frames and event-pattern screening are essential.[§7, SIS: silicon electron-hole yield, charge collection and imaging spectroscopy](../../physics-bibliography.md#asca-technical-description-sis-by-nasa-heasarc)

A measured [silicon](../../chemical-substance.md#silicon) pair-creation energy $w\simeq3.65\,\mathrm{eV}$ gives $N_e=E/w\simeq2.74\times10^3$ [electrons](../../physics.md#electron) for a $10\,\mathrm{keV}$ [photon](../../quantum-mechanics.md#photon). Let $F$ be the [Fano factor](../../variance.md#fano-factor) of pair production, $n_r$ the number of independently read [pixels](../../computer-graphics.md#pixel) in the event sum, and $r$ the rms [read noise](../../optical-instrument.md#read-noise) per [pixel](../../computer-graphics.md#pixel). Then

$$
\sigma_E=w\sqrt{F\frac Ew+n_rr^2+\sigma_d^2+\cdots},\qquad \Delta E_{\rm FWHM}=2\sqrt{2\ln2}\,\sigma_E.
$$

The [Fano-limited X-ray CCD energy resolution](../../optical-instrument.md#fano-limited-x-ray-ccd-energy-resolution) using the representative [silicon](../../chemical-substance.md#silicon) value $F\simeq0.12$ gives an ideal Fano-limited **$\Delta E_{\rm FWHM}\simeq0.16\,\mathrm{keV}$ at $10\,\mathrm{keV}$**, or resolving power $E/\Delta E\simeq64$. Finite [read noise](../../optical-instrument.md#read-noise), charge loss and event summing broaden this; an order-of-magnitude practical estimate is a few tenths of a keV, but the particular detector's value is not determined by the given optical-pixel parameters. These $w$ and $F$ values are external detector properties, not supplied question data. Treating every pair as independent Poisson production instead would give $0.19\,\mathrm{keV}$ rms, or $0.45\,\mathrm{keV}$ FWHM; stating which width is meant avoids conflating those estimates. Radiation-induced charge-transfer inefficiency requires additional gain and spectral-response [calibration](../../differential-geometry.md#calibration-differential-geometry).[§4.7, non-uniform CTI: silicon yield, Fano factor near 0.12 and FWHM resolution formula](../../physics-bibliography.md#the-asca-data-reduction-guide-by-nasa-heasarc)

## ↑ Ancestors (11)

1. [2016](../2016.md)
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
