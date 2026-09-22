# Paper 338

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_338.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_338.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
    - [iv](#2/a/iv)
      - [Solution](#2/a/iv/solution)
    - [v](#2/a/v)
      - [Solution](#2/a/v/solution)
    - [vi](#2/a/vi)
      - [Solution](#2/a/vi/solution)
    - [vii](#2/a/vii)
      - [Solution](#2/a/vii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
    - [iii](#3/d/iii)
      - [Solution](#3/d/iii/solution)

## 1

↑ **Parent:** [Paper 338](paper-338.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The bright peaks occur when contributions from adjacent grooves have equal phase modulo $2\pi$, so all illuminated grooves contribute by [constructive interference](../../../fourier-analysis.md#constructive-interference). Use the reflection-grating convention shown below: $\alpha$ and $\beta$ are positive angles of the incident and outgoing ray lines on the same side of the normal. The incoming and outgoing path differences between neighboring grooves are $d\sin\alpha$ and $d\sin\beta$, respectively. Hence the [grating equation](../../../optics.md#grating-equation) is

$$
\boxed{g(\alpha,\beta,\lambda,d,m)=d(\sin\alpha+\sin\beta)-m\lambda=0.}
$$

The integer $m$ labels the [diffraction order](../../../optics.md#diffraction-order). With a different signed-angle convention, the same physical condition contains a difference of sines.

<a id="1/a/i/image-reflection-grating-angle-convention"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338-grating-rays.png)

**[Figure 1](#1/a/i/image-reflection-grating-angle-convention). Reflection-grating angle convention**. The incident ray and selected outgoing ray are both drawn on the positive side of the surface normal. Adjacent groove spacing contributes the sum of their two projected path differences.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

At fixed incidence angle, [differentiation](../../../calculus.md#differentiation) of the [grating equation](../../../optics.md#grating-equation) gives $d\cos\beta\,d\beta=m\,d\lambda$. Near the camera axis, the focal-plane displacement is $dX\simeq f_{\rm cam}d\beta$, so the local [grating dispersion](../../../optics.md#grating-dispersion) is

$$
\boxed{q=\frac{dX}{d\lambda}=\frac{mf_{\rm cam}}{d\cos\beta}.}
$$

It has units of distance per unit [wavelength](../../../wave-equation.md#wavelength). If the camera axis is at $\beta_0$ and the flat focal-plane coordinate is retained exactly as $X=f_{\rm cam}\tan(\beta-\beta_0)$, then

$$
q=\frac{mf_{\rm cam}\sec^2(\beta-\beta_0)}{d\cos\beta}.
$$

The boxed expression is the local value at the optical axis.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

In the simple slit-image approximation, the projected slit width is $w=x f_{\rm cam}/f_{\rm coll}$. Equating this width to the separation $q\Delta\lambda$ of barely resolved features, using the [grating dispersion](../../../optics.md#grating-dispersion), gives

$$
\Delta\lambda\simeq\frac{xd\cos\beta}{mf_{\rm coll}},\qquad
\boxed{R\simeq\frac{mf_{\rm coll}\lambda}{xd\cos\beta}.}
$$

This recovers the stated [spectral resolving power](../../../optics.md#spectral-resolving-power) under the assumption that the grating has unit anamorphic magnification.

For arbitrary distinct $\alpha$ and $\beta$, the [anamorphic magnification of a grating](../../../optics.md#anamorphic-magnification-of-a-grating) must be included. At fixed [wavelength](../../../wave-equation.md#wavelength), the [grating equation](../../../optics.md#grating-equation) gives $|d\beta/d\alpha|=\cos\alpha/\cos\beta$, so the slit image instead has width $w=x f_{\rm cam}\cos\alpha/(f_{\rm coll}\cos\beta)$. Thus the general [slit-limited resolving power of a grating](../../../optics.md#slit-limited-resolving-power-of-a-grating) is

$$
\boxed{R=\frac{mf_{\rm coll}\lambda}{xd\cos\alpha}.}
$$

The two expressions agree in the [Littrow configuration](../../../optics.md#littrow-configuration), $\alpha=\beta$. Without that condition or the unit-magnification approximation, the quoted $\cos\beta$ expression is not the general slit-limited result. Finite grating size, detector sampling, and [optical aberrations](../../../optics.md#optical-aberration) can lower the actual resolution further.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [echellogram](../../../optics.md#echellogram) contains nearly parallel traces, one for each [diffraction order](../../../optics.md#diffraction-order). Choose the main [echelle grating](../../../optics.md#echelle-grating) dispersion to increase [wavelength](../../../wave-equation.md#wavelength) toward the right and the [cross-disperser](../../../optics.md#cross-disperser) to increase wavelength upward. At a fixed horizontal coordinate, order $m+1$ has a shorter wavelength than order $m$, so it lies below order $m$ in this convention.

<a id="1/b/i/image-adjacent-orders-in-a-cross-dispersed-echellogram"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338-echellogram.png)

**[Figure 2](#1/b/i/image-adjacent-orders-in-a-cross-dispersed-echellogram). Adjacent orders in a cross-dispersed echellogram**. Order m+1 is bluer than order m at the same main-dispersion coordinate. Within either order, wavelength increases along the trace to the right; the chosen cross-dispersion orientation puts longer wavelengths higher on the detector.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let $\beta_0$ be the central camera direction. The [grating equation](../../../optics.md#grating-equation) fixes

$$
K=d(\sin\alpha+\sin\beta_0),\qquad \lambda_m=\frac Km,\qquad\lambda_{m+1}=\frac K{m+1}.
$$

The usual adjacent-order [free spectral range of an echelle grating](../../../optics.md#free-spectral-range-of-an-echelle-grating) is therefore

$$
\boxed{S=\lambda_m-\lambda_{m+1}=\frac K{m(m+1)}.}
$$

The constant $K$ has dimensions of length and is the path difference between adjacent grooves for light directed along the camera axis; it is also the fixed product $m\lambda_m$. Near the [Littrow configuration](../../../optics.md#littrow-configuration), $K=2d\sin\alpha$. The detector width corresponding to this interval is approximately $qS$, with [grating dispersion](../../../optics.md#grating-dispersion) $q$.

There is a convention issue in reading the question literally. Adjacent order-center separation is exactly the expression above. A partition assigning each wavelength to whichever order lands closest to the vertical axis has boundaries halfway in detector displacement, not at adjacent order centers. In the small-angle detector approximation its boundaries for order $m$ are $2K/(2m+1)$ and $2K/(2m-1)$, giving width $4K/(4m^2-1)$. Both conventions give $S\sim K/m^2$ for high orders, but their exact finite-$m$ widths differ. The quoted expression is the conventional adjacent-order spacing.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The [magnitude zero point](../../../astrophysics.md#magnitude-zero-point) is defined by the reference response $I_0$. With zero magnitude assigned to that reference, the [apparent magnitude](../../../astrophysics.md#apparent-magnitude) is

$$
\boxed{m=-2.5\log_{10}\left(\frac I{I_0}\right).}
$$

The two responses must use the same [photometric passband](../../../astrophysics.md#photometric-passband) and instrumental weighting. If the reference has assigned magnitude $m_0$ instead, add $m_0$ to the right-hand side.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

The traditional [infrared photometric bands](../../../astrophysics.md#infrared-photometric-band) extending the optical [photometric system](../../../astrophysics.md#photometric-system) into this range are approximately

$$
\boxed{J:1.25\,\mu{\rm m},\quad H:1.65\,\mu{\rm m},\quad K:2.2\,\mu{\rm m},\quad L:3.5\,\mu{\rm m},\quad M:4.8\,\mu{\rm m}.}
$$

Their [photometric passbands](../../../astrophysics.md#photometric-passband) lie mainly in [atmospheric windows](../../../optics.md#atmospheric-window) between strong molecular absorption bands. This makes ground-based observations practical. The exact centers depend on the system: $L'$ is near $3.8\,\mu{\rm m}$, and shortened $K_s$ and $M'$ bands reduce unwanted background or absorption. At the longest wavelengths, atmospheric and instrumental [thermal radiation](../../../electromagnetism.md#thermal-radiation) make [sky brightness](../../../astrophysics.md#sky-brightness) especially important. A modern $Y$ band near $1.0\,\mu{\rm m}$ is an additional choice, rather than one of the traditional $JHKLM$ extensions.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

For identical [luminosities](../../../astrophysics.md#luminosity) in a uniform Euclidean distribution, the [inverse-square law](../../../physics.md#inverse-square-law) gives flux $F\propto r^{-2}$, while the number of sources within distance $r$ is proportional to $r^3$. Therefore ten times as many objects require $r_{10}/r_1=10^{1/3}$ and $F_{10}/F_1=10^{-2/3}$. Applying the definition of [apparent magnitude](../../../astrophysics.md#apparent-magnitude) gives

$$
\boxed{m_{10}-m_1=-2.5\log_{10}(10^{-2/3})=\frac53,\qquad m_{10}=m_1+\frac53.}
$$

This is the [Euclidean magnitude-limited source count](../../../astrophysics.md#euclidean-magnitude-limited-source-count) relation. It assumes no extinction, spatial variation of density, or cosmological change in the flux-distance relation.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

[Atmospheric extinction](../../../optics.md#atmospheric-extinction) changes the amplitude of the incoming light through absorption and scattering. Its [wavelength](../../../wave-equation.md#wavelength) dependence alters the measured [optical spectrum](../../../optics.md#optical-spectrum) and colors; clouds and aerosols introduce additional time dependence. Scattered moonlight and atmospheric emission increase [sky brightness](../../../astrophysics.md#sky-brightness).

[Atmospheric refraction](../../../optics.md#atmospheric-refraction) changes the apparent position of the source. Its wavelength dependence, [atmospheric dispersion](../../../optics.md#atmospheric-dispersion), spreads a broadband image toward the zenith. The mean [refractive index](../../../electromagnetism.md#refractive-index) gradient therefore affects direction even in the absence of small-scale turbulence.

[Atmospheric turbulence](../../../optics.md#atmospheric-turbulence) produces rapidly varying [optical path lengths](../../../optics.md#optical-path-length), distorting the phase and curvature of a nominally plane [wavefront](../../../optics.md#wavefront). Different pupil regions acquire different phase delays, producing [astronomical seeing](../../../optics.md#astronomical-seeing), image motion, and short-exposure [speckle patterns](../../../optics.md#speckle-pattern). Different lines of sight sample different fluctuations, giving [anisoplanatism](../../../optics.md#anisoplanatism).

Propagation through the fluctuating medium also changes the intensity through [atmospheric scintillation](../../../optics.md#scintillation-astronomy), the familiar twinkling of stars. A phase-only [adaptive optics](../../../optics.md#adaptive-optics) correction can reduce atmospheric phase errors but does not remove absorption, all scintillation, or the atmospheric emission background.

## 2

↑ **Parent:** [Paper 338](paper-338.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

**[Adaptive optics](../../../optics.md#adaptive-optics) corrects rapidly changing atmospheric [wavefront errors](../../../optics.md#wavefront-error) to improve angular resolution and image concentration.** A [wavefront sensor](../../../optics.md#wavefront-sensor) estimates those errors and a feedback controller commands a [deformable mirror](../../../optics.md#deformable-mirror) to oppose them, aiming toward the [diffraction limit of a telescope](../../../optics.md#diffraction-limit-of-a-telescope) rather than the uncorrected [astronomical seeing](../../../optics.md#astronomical-seeing) limit.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The main optical path is telescope to [deformable mirror](../../../optics.md#deformable-mirror) to [beam splitter](../../../optics.md#beam-splitter) to science camera. The splitter also directs reference light to a [wavefront sensor](../../../optics.md#wavefront-sensor); a controller reconstructs the [wavefront error](../../../optics.md#wavefront-error) and feeds mirror commands back to the deformable mirror. The mirror is normally conjugate to a pupil so its actuators address the corresponding pupil phase. A separate steering mirror can handle overall image motion.

<a id="2/a/ii/image-an-adaptive-optics-feedback-loop"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338-adaptive-optics-loop.png)

**[Figure 3](#2/a/ii/image-an-adaptive-optics-feedback-loop). An adaptive-optics feedback loop**. Solid arrows show optical paths. The wavefront sensor observes the corrected reference beam; dashed arrows return measured errors and actuator commands through the controller. The science beam shares the deformable mirror.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The [Strehl ratio](../../../optics.md#strehl-ratio) is

$$
\boxed{S=\frac{\text{observed point-spread-function peak}}{\text{ideal diffraction-limited peak}},}
$$

using the same total flux, pupil, and [wavelength](../../../wave-equation.md#wavelength) for both images. A value near one means that little light has been redistributed from the ideal central peak by [wavefront errors](../../../optics.md#wavefront-error). For small residual phase variance $\sigma_\phi^2$, the [Maréchal approximation](../../../optics.md#marechal-approximation) is $S\simeq e^{-\sigma_\phi^2}$, with $\sigma_\phi=2\pi h_{\rm rms}/\lambda$ for the residual optical-path [root mean square](../../../analysis.md#root-mean-square) error.

<h4 id="2/a/iv">iv</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/a/iv)

[Adaptive-optics sky coverage](../../../optics.md#adaptive-optics-sky-coverage) is limited by the need for a [guide star](../../../optics.md#guide-star-adaptive-optics) bright enough to measure the [wavefront error](../../../optics.md#wavefront-error) on the atmospheric evolution time. A faint guide gives noisy measurements; a guide too far from the target samples a different turbulent column. That angular mismatch is [anisoplanatism](../../../optics.md#anisoplanatism), with useful separation characterized by the [isoplanatic angle](../../../optics.md#isoplanatic-angle). Thus a conventional single-guide system cannot provide equally good correction at every target position.

A [laser guide star](../../../optics.md#laser-guide-star) supplies an artificial bright reference and improves coverage. However, its finite-distance beam does not sample the full stellar turbulence column, and conventional laser systems need a natural reference for absolute image motion. The required reference brightness, angular separation, and desired correction quality therefore still constrain observations.

<h4 id="2/a/v">v</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/v/solution">Solution</h5>

↑ **Parent:** [V](#2/a/v)

**[Astronomical seeing](../../../optics.md#astronomical-seeing) is the atmospheric angular blurring of a point-source image, usually reported in [arcseconds](../../../geometry-and-topology.md#arcsecond).** Operationally it is commonly characterized by the [full width at half maximum](../../../analysis.md#full-width-at-half-maximum) of a long-exposure stellar [point spread function](../../../optics.md#point-spread-function). The full observed width can also contain telescope and instrumental contributions; the atmospheric seeing is the turbulence contribution.

<h4 id="2/a/vi">vi</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#2/a/vi)

For a large aperture in the standard turbulence model, [astronomical seeing](../../../optics.md#astronomical-seeing) is approximately $s=0.98\lambda/r_0$ radians, with [Fried parameter](../../../optics.md#fried-parameter) $r_0$. Maintaining comparable correction requires a [deformable mirror](../../../optics.md#deformable-mirror) actuator pitch of order $r_0$, so the number of actuators across a diameter is proportional to $D/r_0$ and the total illuminated actuator count is proportional to $(D/r_0)^2$. Therefore

$$
\boxed{N_{\rm across}\propto\lambda^{-6/5},\qquad N_{\rm total}\propto\lambda^{-12/5},\qquad s\propto\lambda^{-1/5}.}
$$

Longer wavelengths require fewer actuators and have slightly smaller uncorrected atmospheric angular blur, even though the telescope's [diffraction-limited resolution](../../../optics.md#diffraction-limited-resolution) scale $\lambda/D$ increases with wavelength.

<h4 id="2/a/vii">vii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/vii/solution">Solution</h5>

↑ **Parent:** [Vii](#2/a/vii)

For the unnormalized [Zernike polynomial](../../../numerical-analysis.md#zernike-polynomials) with $n=4,m=0$, the three radial terms are

$$
\frac{4!}{2!2!}\rho^4-\frac{3!}{1!1!1!}\rho^2+\frac{2!}{2!0!0!}=6\rho^4-6\rho^2+1.
$$

Since $\cos0\phi=1$,

$$
\boxed{Z_4^0(\rho,\phi)=6\rho^4-6\rho^2+1.}
$$

Along a central chord with signed coordinate $s\in[-1,1]$, replace $\rho$ by $|s|$. The profile is even, equals one at the center and both edges, and has minima $-1/2$ at $s=\pm1/\sqrt2$. This [Zernike spherical mode](../../../numerical-analysis.md#zernike-spherical-mode) corresponds to **primary [spherical aberration](../../../optics.md#spherical-aberration)**, balanced by defocus and piston terms rather than simply the raw quartic Seidel term.

<a id="2/a/vii/image-the-unnormalized-zernike-spherical-mode-on-a-central-chord"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338-zernike-spherical-mode.png)

**[Figure 4](#2/a/vii/image-the-unnormalized-zernike-spherical-mode-on-a-central-chord). The unnormalized Zernike spherical mode on a central chord**. The even quartic has central and edge values one and two minima of minus one half. Its lower-order terms remove its projections onto piston and defocus.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The projected actuator pitch is $p=D/N$ in the question's sampling convention. A sinusoidal [wavefront error](../../../optics.md#wavefront-error) needs at least two samples per spatial period, by the [Nyquist–Shannon sampling theorem](../../../fourier-analysis.md#nyquist-shannon-sampling-theorem). Thus the shortest limiting correctable scale at the primary is

$$
\boxed{\Lambda_{\min}=2p=\frac{2D}N.}
$$

The [Nyquist spatial frequency](../../../fourier-analysis.md#nyquist-spatial-frequency) is $N/(2D)$ cycles per unit length. Exactly at that limiting frequency some phases are poorly sampled; actual [deformable mirror](../../../optics.md#deformable-mirror) performance also depends on actuator influence functions, so this is an ideal bandwidth limit.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Count independent sinusoidal ripples by their spatial [Fourier series](../../../fourier-series.md) indices. A mode with $n$ cycles across $D$ has $\Lambda=D/n$, so the given half-wave index is $j=2n$. The [Nyquist spatial frequency](../../../fourier-analysis.md#nyquist-spatial-frequency) permits $n\leq N/2$. In two dimensions, a circular cutoff therefore contains approximately $\pi(N/2)^2$ integer wavevectors.

For a real [wavefront error](../../../optics.md#wavefront-error), the wavevectors $\mathbf n$ and $-\mathbf n$ describe the same ripple with conjugate coefficients, so count each pair once. The continuum mode-counting approximation gives

$$
\boxed{M\simeq\frac12\pi\left(\frac N2\right)^2=\frac{\pi N^2}8=\frac\pi4\left(\frac{N^2}2\right).}
$$

This counts one ripple with amplitude and phase per conjugate pair, not one real coefficient. Exact finite-grid counts are integers and have boundary corrections; the formula is the circular area estimate implicit in the question, with piston excluded.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The supplied [speckle contrast of a sinusoidal wavefront error](../../../optics.md#speckle-contrast-of-a-sinusoidal-wavefront-error) gives $h_0=\lambda\sqrt C/\pi$. Each sinusoid has [root mean square](../../../analysis.md#root-mean-square) error $h_0/\sqrt2$. For orthogonal modes, or for uncorrelated phases so that cross terms average to zero, the total mean square adds:

$$
h_{\rm rms}^2=M\frac{h_0^2}2=\frac{\pi N^2}8\frac{\lambda^2C}{2\pi^2}.
$$

Therefore the assumed equal-contrast modal model gives

$$
\boxed{h_{\rm rms}=\frac{N\lambda\sqrt C}{4\sqrt\pi}.}
$$

If the individual contrasts are not equal, the corresponding formula is $h_{\rm rms}^2=\lambda^2\sum_iC_i/(2\pi^2)$. The error here is optical-path [wavefront error](../../../optics.md#wavefront-error); for a near-normal reflecting mirror, physical surface error is half the optical-path error.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

A [wavefront error](../../../optics.md#wavefront-error) ripple of period $\Lambda$ generates a pair of speckles at angular displacement $\lambda/\Lambda$. Combining this with $\Lambda_{\min}=2D/N$ gives the [deformable-mirror control radius](../../../optics.md#deformable-mirror-control-radius) along an actuator row or column:

$$
\boxed{\theta_{\max}=\frac{N\lambda}{2D}.}
$$

A square actuator lattice has a square ideal frequency region: $|\theta_x|,|\theta_y|\leq N\lambda/(2D)$. Its full width is $N\lambda/D$, approximately $N$ [diffraction-limited resolution](../../../optics.md#diffraction-limited-resolution) elements per side, or $N^2$ in area. The circular subset within the row-direction radius contains approximately $\pi N^2/4$ such elements. The primary aperture shapes each speckle's [point spread function](../../../optics.md#point-spread-function); it does not turn the square sampling limit into a circular one.

This full square describes phase-error control. Simultaneous amplitude and phase correction with a single pupil-plane [deformable mirror](../../../optics.md#deformable-mirror) generally requires restricting the dark region to a half-plane; it is a different constraint from the sampling bandwidth.

## 3

↑ **Parent:** [Paper 338](paper-338.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $u$ and $v$ be the real object and image distances from the [thin lens](../../../optics.md#thin-lens). The object-screen separation gives $u+v=L$, and the [thin lens](../../../optics.md#thin-lens) equation gives $uv=fL$. Thus the two lens positions solve

$$
u(L-u)=fL,\qquad u_\pm=\frac{L\pm\sqrt{L^2-4fL}}2.
$$

Their separation is $d=u_+-u_-=\sqrt{L^2-4fL}$, so

$$
\boxed{f=\frac{L^2-d^2}{4L}.}
$$

This is the [Bessel lens displacement method](../../../optics.md#bessel-lens-displacement-method) for measuring [focal length](../../../optics.md#focal-length). It uses the screen-object separation and the displacement between two sharp-image settings, reducing the need to locate the lens's effective optical center. It assumes the thin-lens or corresponding principal-plane approximation; $L>4f$ is what provides two distinct real-image settings.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

For thin lenses in contact, [optical powers](../../../optics.md#optical-power) add. At the two reference wavelengths, the [lensmaker's equation](../../../optics.md#lensmaker-s-equation) gives total power

$$
\Phi_F=\rho_1(n_{1F}-1)+\rho_2(n_{2F}-1),\qquad\Phi_C=\rho_1(n_{1C}-1)+\rho_2(n_{2C}-1).
$$

An [achromatic lens](../../../optics.md#achromatic-lens) has $\Phi_F=\Phi_C$. Subtracting and solving for the curvature-factor ratio yields

$$
\boxed{\frac{\rho_1}{\rho_2}=-\frac{n_{2F}-n_{2C}}{n_{1F}-n_{1C}}.}
$$

Opposite curvature-weighted powers compensate the two materials' [optical dispersion](../../../optics.md#dispersion-optics).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

At the intermediate $d$ reference wavelength, the [lensmaker's equation](../../../optics.md#lensmaker-s-equation) gives $1/f_{id}=\rho_i(n_{id}-1)$. Therefore the curvature-factor ratio from the previous part implies

$$
\frac{f_{2d}}{f_{1d}}=\frac{\rho_1(n_{1d}-1)}{\rho_2(n_{2d}-1)},
$$

and hence

$$
\boxed{\frac{f_{2d}}{f_{1d}}=-\frac{(n_{2F}-n_{2C})/(n_{2d}-1)}{(n_{1F}-n_{1C})/(n_{1d}-1)}=-\frac{V_{1d}}{V_{2d}}.}
$$

The last equality uses the [Abbe number](../../../optics.md#abbe-number) definition and expresses the [achromatic doublet power balance](../../../optics.md#achromatic-doublet-power-balance) in terms of component [focal lengths](../../../optics.md#focal-length).

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Write $\Phi_i=1/f_{id}$ and $\Phi=1/f_d$. The [achromatic doublet power balance](../../../optics.md#achromatic-doublet-power-balance) is

$$
\Phi_1+\Phi_2=\Phi,\qquad \frac{\Phi_1}{V_{1d}}+\frac{\Phi_2}{V_{2d}}=0.
$$

Solving these two linear equations gives $\Phi_1=\Phi V_{1d}/(V_{1d}-V_{2d})$ and $\Phi_2=-\Phi V_{2d}/(V_{1d}-V_{2d})$. Taking reciprocals gives the required [focal lengths](../../../optics.md#focal-length):

$$
\boxed{f_{1d}=\frac{f_d(V_{1d}-V_{2d})}{V_{1d}},\qquad f_{2d}=\frac{f_d(V_{2d}-V_{1d})}{V_{2d}}.}
$$

The design requires distinct [Abbe numbers](../../../optics.md#abbe-number); identical relative dispersion cannot yield a nonzero total achromatic power from this two-element thin model.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

**$V_d$ is the [Abbe number](../../../optics.md#abbe-number)**, a measure of inverse relative [optical dispersion](../../../optics.md#dispersion-optics). Ordinary [crown glasses](../../../optics.md#crown-glass-optics) have comparatively large $V_d$ and lower [refractive index](../../../electromagnetism.md#refractive-index), while ordinary [flint glasses](../../../optics.md#flint-glass) have smaller $V_d$ and often higher index. The [Abbe diagram](../../../optics.md#abbe-diagram) below spans typical optical-glass values; the shaded family ranges are schematic, and the marked examples are catalogue data. Modern glass compositions broaden and overlap the simple crown/flint picture.

<a id="3/b/iv/image-refractive-index-and-abbe-number-for-representative-optical-glasses"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338-abbe-diagram.png)

**[Figure 5](#3/b/iv/image-refractive-index-and-abbe-number-for-representative-optical-glasses). Refractive index and Abbe number for representative optical glasses**. Markers use refractive indices and Abbe numbers from the SCHOTT Optical Glass pocket catalogue. Shaded regions are schematic family ranges rather than a catalogue boundary. The horizontal axis follows the traditional convention of decreasing Abbe number toward the right.

For a positive doublet with $V_{1d}>V_{2d}$, the preceding formulas require $f_{1d}>0$ and $f_{2d}<0$: a converging [crown glass](../../../optics.md#crown-glass-optics) element and a diverging [flint glass](../../../optics.md#flint-glass) element. Their dispersion corrections cancel, while their net [optical power](../../../optics.md#optical-power) is positive. A small difference in Abbe numbers requires large opposing component powers, which makes the design harder to correct for other [optical aberrations](../../../optics.md#optical-aberration).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Let the two internal angles be $r=\theta_2$ and $\phi-r=\theta_3$, since the [optical prism](../../../optics.md#prism-optics) geometry gives $\theta_2+\theta_3=\phi$. By [Snell's law](../../../partial-differential-equation.md#snell-s-law), the corresponding external angles are $F(r)$ and $F(\phi-r)$, where $F(r)=\arcsin(n\sin r)$. The deviation is

$$
\gamma(r)=F(r)+F(\phi-r)-\phi.
$$

On the transmitted branch with $n>1$ and $0<r<\arcsin(1/n)$,

$$
F''(r)=\frac{n(n^2-1)\sin r}{(1-n^2\sin^2r)^{3/2}}>0.
$$

Thus $F'$ is strictly increasing. The stationary condition $\gamma'(r)=F'(r)-F'(\phi-r)=0$ forces $r=\phi-r$, and the positive second [derivative](../../../calculus.md#derivative) makes this the unique [minimum deviation](../../../optics.md#minimum-deviation). Consequently

$$
\boxed{\theta_2=\theta_3=\frac\phi2,\qquad\theta_1=\theta_4.}
$$

The argument assumes a transmitted ray is possible; the symmetric internal angles must lie below the critical angle.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The [reversibility of an optical ray](../../../optics.md#reversibility-of-an-optical-ray) interchanges entry and exit while preserving the total deviation. Away from the turning point, a ray and its reversed configuration give the same deviation with the entry and exit angles exchanged. At [minimum deviation](../../../optics.md#minimum-deviation) the two configurations merge: the path is symmetric and the entry and exit angles are equal.

Physically, distributing the refraction symmetrically between the two faces avoids making one face contribute disproportionately large bending. The strict convexity established in the preceding part proves that this stationary symmetric configuration is the minimum, rather than merely following from reversibility alone.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

At [minimum deviation](../../../optics.md#minimum-deviation), $\theta_2=\theta_3=\phi/2$ and $\theta_1=\theta_4=(\gamma_{\min}+\phi)/2$. Substituting in [Snell's law](../../../partial-differential-equation.md#snell-s-law) gives

$$
\boxed{n=\frac{\sin[(\gamma_{\min}+\phi)/2]}{\sin(\phi/2)}.}
$$

For a known prism apex angle, measuring the minimum deviation with monochromatic light determines its [refractive index](../../../electromagnetism.md#refractive-index). Repeating the measurement at several [wavelengths](../../../wave-equation.md#wavelength) measures [optical dispersion](../../../optics.md#dispersion-optics). If the surrounding medium is not air, the measured ratio is relative to that medium's refractive index.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

The two standard designs are **[multi-slit spectrographs](../../../optics.md#multi-slit-spectrograph)** and **[fiber-fed spectrographs](../../../optics.md#fiber-fed-spectrograph)**. Both select many astronomical targets simultaneously and arrange their light so the resulting [optical spectra](../../../optics.md#optical-spectrum) remain distinguishable on the detector.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

A [multi-slit spectrograph](../../../optics.md#multi-slit-spectrograph) uses a focal-plane mask containing slitlets at the target positions, or movable slitlets placed there. Each transmits its target and nearby sky into the [collimator](../../../optics.md#collimator); a [diffraction grating](../../../optics.md#diffraction-grating) or other disperser produces a separate [optical spectrum](../../../optics.md#optical-spectrum) on the detector. The layout must avoid overlap between spectra, and the length of a slit allows local sampling of [sky brightness](../../../astrophysics.md#sky-brightness) and sometimes spatial information within the target.

A [fiber-fed spectrograph](../../../optics.md#fiber-fed-spectrograph) places [optical fibers](../../../optics.md#optical-fiber) at target positions in the telescope focal plane. The fibers carry the selected light to a spectrograph and their outputs are lined up as a pseudo-slit. The spectrograph can be mechanically stable and separate from the telescope's focal plane. Additional fibers aimed at blank sky provide a simultaneous estimate of [sky brightness](../../../astrophysics.md#sky-brightness); fiber positioning, coupling losses, transmission, and [focal-ratio degradation](../../../optics.md#focal-ratio-degradation) must be accounted for.

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

For **field of view**, [fiber-fed spectrographs](../../../optics.md#fiber-fed-spectrograph) commonly cover wider sky areas: fibers can pick targets across a broad focal plane while feeding a compact spectrograph with a fixed output slit. A [multi-slit spectrograph](../../../optics.md#multi-slit-spectrograph) must image its field through the spectrograph optics, and spectra must fit on the detector without overlap, which restricts both field and target layout.

For **spectral resolution**, fibers can feed an optimized, stable high-dispersion instrument, including an [echelle grating](../../../optics.md#echelle-grating). The fiber image acts as its entrance width. In a [multi-slit spectrograph](../../../optics.md#multi-slit-spectrograph), slit width and dispersion similarly determine the [spectral resolving power](../../../optics.md#spectral-resolving-power). Neither feed type alone imposes a universal resolution ranking: narrower fibers or slits improve resolution at the cost of losing source light, and both can be designed for high or low resolution.

For **faintness limit**, slit masks often have an advantage for individual faint objects because they avoid fiber coupling and transmission losses, permit a slit width matched to [astronomical seeing](../../../optics.md#astronomical-seeing), and sample local sky along the slit. Fibers can admit more sky through a fixed circular aperture and require sky subtraction from separate locations; [focal-ratio degradation](../../../optics.md#focal-ratio-degradation) can also reduce throughput. The actual limit depends on throughput, aperture size, background stability, and detector noise through the [signal-to-noise ratio in photon counting](../../../optics.md#signal-to-noise-ratio-in-photon-counting). Well-designed fiber instruments can nevertheless be very efficient for wide-field surveys, so the comparison is conditional on the optical design and observing conditions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
