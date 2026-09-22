# Fourier transform

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier_transform)

For $f\in L^1(\mathbb R^n)$, the angular-frequency Fourier transform is

$$
\widehat f(\xi)
=\int_{\mathbb R^n}f(x)e^{-ix\cdot\xi}\,dx.
$$

**Table of contents**

- [Inverse Fourier transform](#inverse-fourier-transform)
- [Fourier transform of a polynomial multiple](#fourier-transform-of-a-polynomial-multiple)
- [Duality property of the Fourier transform](#duality-property-of-the-fourier-transform)
- [Fourier transform of a truncated cosine](#fourier-transform-of-a-truncated-cosine)
- [Fourier transform of the hyperbolic secant](#fourier-transform-of-the-hyperbolic-secant)
- [Hermitian symmetry](#hermitian-symmetry)
- [Window function](#window-function)
  - [Spectral leakage](#spectral-leakage)
- [Uncentred Fourier uncertainty principle](#uncentred-fourier-uncertainty-principle)
- [Fourier transform on a locally compact abelian group](#fourier-transform-on-a-locally-compact-abelian-group)
  - [Fourier inversion on a locally compact abelian group](#fourier-inversion-on-a-locally-compact-abelian-group)
- [Fourier decay from a derivative jump](#fourier-decay-from-a-derivative-jump)
  - [Fourier transform of an algebraic cusp](#fourier-transform-of-an-algebraic-cusp)
- [Modulation property of the Fourier transform](#modulation-property-of-the-fourier-transform)
- [Fourier transform of a finite measure](#fourier-transform-of-a-finite-measure)
- [Complex spectral Fourier transform](#complex-spectral-fourier-transform)
- [Bandlimited function](#bandlimited-function)
- [Half-range Fourier transform](#half-range-fourier-transform)
  - [Rotated null contours for half-range Fourier inversion](#rotated-null-contours-for-half-range-fourier-inversion)
  - [Half-line drift null contour identity](#half-line-drift-null-contour-identity)
- [Fourier transform isomorphism of the Schwartz space](#fourier-transform-isomorphism-of-the-schwartz-space)
- [Fourier cosine transform](#fourier-cosine-transform)
- [Fourier sine transform](#fourier-sine-transform)
  - [Fourier sine inversion](#fourier-sine-inversion)
- [Sinc function](#sinc-function)
  - [Sinc fourth-power integral](#sinc-fourth-power-integral)
- [Fourier space](#fourier-space)
- [Moment differentiation of the Fourier transform](#moment-differentiation-of-the-fourier-transform)
- [Fourier transform has proper dense image from L1 to C0](#fourier-transform-has-proper-dense-image-from-l1-to-c0)
- [Hankel transform](#hankel-transform)
  - [Isotropic transverse covariance spectrum](#isotropic-transverse-covariance-spectrum)
  - [Fourier-Hankel normalization for an isotropic spectrum](#fourier-hankel-normalization-for-an-isotropic-spectrum)
- [Wigner distribution](#wigner-distribution)
  - [Optical Wigner function](#optical-wigner-function)
  - [Free Schrodinger Wigner transport](#free-schrodinger-wigner-transport)
  - [Receiver-averaged Wigner distribution](#receiver-averaged-wigner-distribution)
- [Japanese bracket](#japanese-bracket)
  - [Peetre weight inequality](#peetre-weight-inequality)
- [Fourier shift theorem](#fourier-shift-theorem)
- [Fresnel integral](#fresnel-integral)
  - [Optical normalization of Fresnel integrals](#optical-normalization-of-fresnel-integrals)
  - [Finite Fresnel integrals](#finite-fresnel-integrals)
    - [Fresnel tail expansion](#fresnel-tail-expansion)
  - [Regulated complex Fresnel integral](#regulated-complex-fresnel-integral)
  - [Oscillatory Gaussian integral with negative phase](#oscillatory-gaussian-integral-with-negative-phase)
- [Additive character](#additive-character)
  - [Character annihilator](#character-annihilator)
- [Fourier transform over a local field](#fourier-transform-over-a-local-field)
  - [Fourier transform of a ball indicator over a local field](#fourier-transform-of-a-ball-indicator-over-a-local-field)
  - [Self-dual Haar measure](#self-dual-haar-measure)
  - [Annihilator of the valuation ring](#annihilator-of-the-valuation-ring)
- [Fourier multiplier](#fourier-multiplier)
  - [Half-plane Fourier projection](#half-plane-fourier-projection)
  - [Nonintegrability of a radial triangular Fourier cutoff in three dimensions](#nonintegrability-of-a-radial-triangular-fourier-cutoff-in-three-dimensions)
  - [Fourier multiplier operator](#fourier-multiplier-operator)
- [Fourier transform of a function with reciprocal tails](#fourier-transform-of-a-function-with-reciprocal-tails)
- [Scaling property of the Fourier transform](#scaling-property-of-the-fourier-transform)
  - [Scaling necessity for an Lp to Lq Fourier bound](#scaling-necessity-for-an-lp-to-lq-fourier-bound)
- [Fourier transform of inverse distance in three dimensions](#fourier-transform-of-inverse-distance-in-three-dimensions)
- [Hilbert transform](#hilbert-transform)
  - [Hilbert transform of the sinc function](#hilbert-transform-of-the-sinc-function)
  - [Directional Hilbert transform](#directional-hilbert-transform)
  - [Large-distance tail of the Hilbert transform](#large-distance-tail-of-the-hilbert-transform)
  - [Hilbert-transform Fourier multiplier](#hilbert-transform-fourier-multiplier)
- [Fourier transform of an interval indicator](#fourier-transform-of-an-interval-indicator)
- [Sinc-squared integral](#sinc-squared-integral)

## Inverse Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

With the [Fourier transform](fourier-transform.md) convention $\widehat f(k)=\int_{\mathbb R}f(x)e^{-ikx}\,dx$, the inverse Fourier transform is the displayed [linear operator](vector-space.md#linear-operator). The integral is defined directly for an [integrable function](measure-theory.md#lebesgue-integrable-function) $g$. The [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem) ensures $\mathcal F^{-1}\widehat f=f$ under its hypotheses, in particular for [Schwartz functions](fourier-analysis.md#schwartz-function), and for integrable $f$ and $\widehat f$ at continuity points of $f$. The operation also extends to [tempered distributions](fourier-analysis.md#tempered-distribution); the normalization and sign depend on the chosen [Fourier transform](fourier-transform.md) convention.

## Fourier transform of a polynomial multiple

↑ **Parent:** [Fourier transform](fourier-transform.md)

With [Fourier transform](fourier-transform.md) convention $\widehat f(k)=\int f(x)e^{-ikx}dx$, differentiation under the [integral](integral.md) gives $\partial_k^n\widehat f=\int(-ix)^nf(x)e^{-ikx}dx$, proving the displayed identity. For example it applies when all $x^jf(x)$ for $0\leq j\leq n$ are absolutely integrable, or in the [tempered distribution](fourier-analysis.md#tempered-distribution) sense. It is the dual counterpart of the [Fourier transform of a derivative](fourier-analysis.md#fourier-transform-of-a-derivative).

## Duality property of the Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

For the [Fourier transform](fourier-transform.md) convention $\mathcal Ff(\omega)=\int_{\mathbb R}f(t)e^{-i\omega t}\,dt$, [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) at $-\omega$ gives $f(-\omega)=(2\pi)^{-1}\int_{\mathbb R}(\mathcal Ff)(t)e^{-i\omega t}\,dt$. Thus transforming twice reflects the argument and multiplies by $2\pi$. The identity holds directly on the [Schwartz space](fourier-analysis.md#schwartz-space), and extends to the [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) and to [tempered distributions](fourier-analysis.md#tempered-distribution). It lets an already known transform pair be used in reverse without another integration.

## Fourier transform of a truncated cosine

↑ **Parent:** [Fourier transform](fourier-transform.md)

For $f(x)=\cos x$ on $[-a,a]$ and zero outside, the angular-frequency [Fourier transform](fourier-transform.md) follows by writing the cosine as two [complex exponentials](calculus.md#complex-exponential-function). Combining fractions gives $[2k\cos a\sin(ak)-2\sin a\cos(ak)]/(k^2-1)$. The apparent singularities at $k=\pm1$ are removable, with value $a+\sin(2a)/2$. If $\cos a\ne0$, jumps at the endpoints give an oscillatory $O(|k|^{-1})$ envelope. If $\cos a=0$, the function is continuous at the endpoints but its first [derivative](calculus.md#derivative) jumps, giving an $O(|k|^{-2})$ envelope. This is an explicit instance of [Fourier decay from a derivative jump](#fourier-decay-from-a-derivative-jump).

## Fourier transform of the hyperbolic secant

↑ **Parent:** [Fourier transform](fourier-transform.md)

For real $k$, integrate $e^{-ikz}/\cosh z$ around a rectangle of height $\pi$. Its top-edge value is $-e^{\pi k}$ times the bottom-edge value, and the only enclosed [simple pole](isolated-singularity.md#simple-pole) is $i\pi/2$, with [residue](analysis.md#residue) $e^{\pi k/2}/i$. The vertical-edge integrals vanish as their real parts tend to positive and negative infinity. The [residue theorem](analysis.md#residue-theorem) gives $(1+e^{\pi k})\widetilde f(k)=2\pi e^{\pi k/2}$, proving the stated [Fourier transform](fourier-transform.md) identity. This is an example of a function reproducing its shape under a [Fourier transform](fourier-transform.md), up to rescaling.

## Hermitian symmetry

↑ **Parent:** [Fourier transform](fourier-transform.md)

If $f$ is a [real-valued function](function.md#real-valued-function) and an [integrable function](measure-theory.md#lebesgue-integrable-function), its [Fourier transform](fourier-transform.md) has [Hermitian symmetry](#hermitian-symmetry): $F(-u)=\overline{F(u)}$. The value at negative [frequency](wave.md#frequency) is the [complex conjugate](complex-analysis.md#complex-conjugate) of the value at positive [frequency](wave.md#frequency).

## Window function

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Window_function)

A window function is a [function](function.md) that vanishes outside a chosen finite [interval](real-analysis.md#interval-mathematics); multiplying an input by it selects and weights that part of the history before a [Fourier transform](fourier-transform.md). The rectangular window $w_T$ is the [indicator function](measure-theory.md#indicator-function) of $[0,T]$. Applied to the weighted [causal extension by zero](integral-transform.md#causal-extension-by-zero) of an input, it produces the finite-history [integral](integral.md) $\int_0^T e^{-st}f(t)\,dt$ used to approximate a [Laplace transform](integral-transform.md#laplace-transform).

### Spectral leakage

↑ **Parent:** [Window function](#window-function)

Multiplying a measured [signal](electrical-engineering.md#signal) by a finite-duration [window function](#window-function) convolves its [Fourier transform](fourier-transform.md) with the transform of the window. A spectrally sharp component therefore contributes to nearby frequencies rather than remaining a single ideal line. Smooth tapering can reduce distant sidelobes at the cost of widening the main spectral feature. This finite-record effect is distinct from [aliasing](fourier-analysis.md#aliasing), which superposes copies of the spectrum because of time sampling.

## Uncentred Fourier uncertainty principle

↑ **Parent:** [Fourier transform](fourier-transform.md)

For nonzero $f$ with $f,xf,f'\in L^2(\mathbb R)$, integration by parts gives $\|f\|_2^2=-2\operatorname{Re}\langle f',xf\rangle$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and [Plancherel theorem](fourier-analysis.md#plancherel-theorem) yield the moment product bound $1/4$ with the angular-frequency Fourier convention. Equality occurs exactly for $f(x)=C e^{-ax^2/2}$ with $a>0$ real and $C\ne0$. Translation, modulation or a quadratic phase increase one of these uncentred moments; the equality family is narrower than that for centred variances.

## Fourier transform on a locally compact abelian group

↑ **Parent:** [Fourier transform](fourier-transform.md)

For $f\in L^1(G)$ the displayed integral defines a bounded continuous function on the [Pontryagin dual group](group.md#pontryagin-dual-group). It takes [convolution](fourier-analysis.md#convolution) to pointwise multiplication and left translation $T_x$ to multiplication by $\overline{\chi(x)}$. The transform depends on the scale of [Haar measure](measure.md#haar-measure) on $G$; the compatible [dual Haar measure](group.md#dual-haar-measure) scales reciprocally.

### Fourier inversion on a locally compact abelian group

↑ **Parent:** [Fourier transform on a locally compact abelian group](#fourier-transform-on-a-locally-compact-abelian-group)

For the [dual Haar measure](group.md#dual-haar-measure), the formula first follows for continuous compactly supported convolution squares from the [Bochner theorem](harmonic-analysis.md#bochner-s-theorem). More generally, if $f\in L^1(G)$ and $\widehat f\in L^1(\widehat G)$, the right-hand side is a continuous representative of $f$; equality holds everywhere if $f$ is continuous, and otherwise at every point where the chosen representative is continuous. Convolution with normalized small-support positive convolution squares proves the extension: the spatial convolutions approach $f$ in $L^1$, while their transforms approach $\widehat f$ in $L^1$ by [equicontinuity of compact families of characters](group.md#equicontinuity-of-compact-families-of-characters) and an integrable-tail split.

## Fourier decay from a derivative jump

↑ **Parent:** [Fourier transform](fourier-transform.md)

For a piecewise smooth decaying function, a jump in its $j$th derivative at $a$ contributes the displayed algebraic term to its high-frequency [Fourier transform](fourier-transform.md). Distributionally, $D^{j+1}f$ contains $[f^{(j)}]_a\delta(x-a)$, and [integration by parts](calculus.md#integration-by-parts) or the derivative-transform identity supplies the factor $(ik)^{-j-1}$. Adequate integrability of the subsequent derivatives controls the remainder. Smooth localized polynomial terms give no algebraic cusp contribution.

### Fourier transform of an algebraic cusp

↑ **Parent:** [Fourier decay from a derivative jump](#fourier-decay-from-a-derivative-jump)

For $p>-1$ this formula is interpreted away from $k=0$ as a [tempered distribution](fourier-analysis.md#tempered-distribution) or by exponential regularization. It also supplies local high-frequency cusp terms after multiplying by a smooth cutoff. Even nonnegative integer $p$ give smooth polynomials and only contact terms at $k=0$, so their localized forms have no algebraic tail. For example, the cusp expansion of $(1+|x|^3)^{-1}$ gives $-12|k|^{-4}+2\,9!|k|^{-10}+O(|k|^{-16})$.

## Modulation property of the Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

Multiplication by a unit-modulus linear phase shifts the [Fourier transform](fourier-transform.md). Substituting $e^{ia\cdot x}$ into the defining integral gives the displayed identity. For a surface measure this permits independent translations of cap transforms without changing their input [norms](normed-vector-space.md#norm) or angular supports.

## Fourier transform of a finite measure

↑ **Parent:** [Fourier transform](fourier-transform.md)

The angular-frequency [Fourier transform](fourier-transform.md) of a [finite measure](measure.md#finite-measure), or a complex measure of finite total variation, is defined by the displayed integral. It is bounded by total variation and continuous by [dominated convergence](measure-theory.md#dominated-convergence-theorem). An integrable density recovers the ordinary [Fourier transform](fourier-transform.md) of a function. A measure supported on a curved surface instead leads to a [Fourier extension operator](fourier-analysis.md#fourier-extension-operator).

## Complex spectral Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

A complex-coordinate parametrization of the two-dimensional [Fourier transform](fourier-transform.md). With $z=x+iy$, $k=k_1+ik_2$, and $(\xi_1,\xi_2)=(2k_2,-2k_1)$, its exponent is $-i\xi\cdot(x,y)$. Since $d\xi=4dA(k)$, its inverse is $q(z)=\pi^{-2}\int e^{k\bar z-\bar kz}Q(k)dA(k)$. The spectral equation $(\partial_{\bar z}-k)F=q$ gives $\partial_{\bar k}F=-e^{k\bar z-\bar kz}Q(k)/\pi$, linking [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) to a [spectral dbar equation](analysis.md#spectral-dbar-equation).

## Bandlimited function

↑ **Parent:** [Fourier transform](fourier-transform.md)

A [bandlimited function](#bandlimited-function) has [Fourier transform](fourier-transform.md) supported in a bounded frequency interval. An integrable bandlimited function has a bounded continuous representative when its [Fourier transform](fourier-transform.md) is integrable, and that representative extends analytically using the compact-frequency integral. Scaling arguments scales its frequency support inversely, while multiplying two such functions adds their support intervals through convolution.

## Half-range Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

With the $e^{ikx}$ convention, a right-supported decaying function has a transform analytic in the upper half-plane and a left-supported one in the lower half-plane. Incident modes continued with small imaginary frequency can have poles outside the initial convergence strip; these poles must be tracked separately from outgoing scattered waves.

### Rotated null contours for half-range Fourier inversion

↑ **Parent:** [Half-range Fourier transform](#half-range-fourier-transform)

For $Q(k)=\int_0^\infty e^{-ikx}q(x)\,dx$, the [Half-range Fourier transform](#half-range-fourier-transform) is [holomorphic](holomorphic-function.md) in the lower half-plane. Let $\alpha=e^{2\pi i/3}$, $E=\{0<\arg k<\pi/3\}$ and $D=\{2\pi/3<\arg k<\pi\}$, with their boundaries oriented counterclockwise. The rotated arguments $\alpha^2k$ on $E$ and $\alpha k$ on $D$ remain in the lower half-plane. For $x>0$ and transform-admissible smooth decay, the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and [Jordan lemma](complex-analysis.md#jordan-s-lemma) give the displayed null integrals. Arbitrary multiples can therefore be added to [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) without changing the recovered function on the positive half-line.

// Target: integrable-systems.bigb

### Half-line drift null contour identity

↑ **Parent:** [Half-range Fourier transform](#half-range-fourier-transform)

For $\alpha>0$, let $L$ be the upper branch $\operatorname{Im}k=(\alpha+\sqrt{\alpha^2+4(\operatorname{Re}k)^2})/2$, oriented left to right. Above $L$, $i\alpha-k$ lies in the lower half-plane, where a decaying half-line [Fourier transform](fourier-transform.md) is analytic. For $x>0$, closing upward proves that the displayed integral vanishes. An additional multiplier analytic above $L$ with at most polynomial growth is allowed, using exponential decay and, if needed, regularized contours. This supplies a null term in a [Fokas method](boundary-value-problem.md#fokas-method) inversion formula without changing the function in the interior.

## Fourier transform isomorphism of the Schwartz space

↑ **Parent:** [Fourier transform](fourier-transform.md)

The [Fourier transform](fourier-transform.md) with negative exponential and inverse factor $(2\pi)^{-n}$ is a continuous isomorphism of the [Schwartz space](fourier-analysis.md#schwartz-space). Weighted frequency derivatives are transforms of derivatives of weighted input functions, so their suprema are controlled by finitely many Schwartz [seminorms](topological-vector-space.md#seminorm). [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) gives $\mathcal F^2=(2\pi)^n\mathcal R$, where $\mathcal Rf(x)=f(-x)$. Transposition gives a continuous isomorphism on [tempered distributions](fourier-analysis.md#tempered-distribution) as well.

## Fourier cosine transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

For sufficiently regular decaying data, this half-line transform has inverse $f(x)=(2/\pi)\int_0^\infty C(k)\cos(kx)dk$. To derive it, extend $f$ evenly to the real line. Its [Fourier transform](fourier-transform.md) with negative exponential is $2C(k)$, and its odd sine contribution vanishes. The [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem) then gives the stated factor $2/\pi$. If the forward transform is instead defined as $\widehat f_c=2C$, the inverse factor is $1/\pi$.

With boundary terms at infinity vanishing, two [integrations by parts](calculus.md#integration-by-parts) give the cosine transform of $f''$ as $-k^2C(k)-f'(0)$. Thus a homogeneous [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) makes it a multiplier $-k^2C(k)$, paralleling the [Fourier sine transform](#fourier-sine-transform) with a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition).

## Fourier sine transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

The Fourier sine transform is a half-line transform adapted to a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition). With the displayed normalization, inversion is $f(x)=(2/\pi)\int_0^\infty\sin(kx)S(k)dk$. It is equivalent to the [Fourier transform](fourier-transform.md) of an odd extension. If $f(0)=0$ and boundary terms vanish, two [integrations by parts](calculus.md#integration-by-parts) give the transform of $f''$ as $-k^2S(k)$.

### Fourier sine inversion

↑ **Parent:** [Fourier sine transform](#fourier-sine-transform)

For sufficiently regular integrable functions on a half-line, [Fourier sine transform](#fourier-sine-transform) inversion recovers the odd extension at continuity points. A zero endpoint value is required when demanding continuity at the endpoint.

## Sinc function

↑ **Parent:** [Fourier transform](fourier-transform.md)

The unnormalized sinc is $\operatorname{sinc}(x)=\sin x/x$, extended by value one at zero. The normalized form is $\sin(\pi x)/(\pi x)$. It is the inverse [Fourier transform](fourier-transform.md) of a frequency interval indicator, so it describes ideal low-pass filtering and the [Shannon scaling function](fourier-analysis.md#shannon-scaling-function).

### Sinc fourth-power integral

↑ **Parent:** [Sinc function](#sinc-function)

The [triangular function](fourier-analysis.md#triangular-function) $f(x)=(1-|x|)$ on $|x|<1$, zero elsewhere, has [Fourier transform](fourier-transform.md) $\widehat f(k)=[\sin(k/2)/(k/2)]^2$ in the angular-frequency convention. Its squared [L2 norm](real-analysis.md#l2-norm) is $2/3$. [Parseval's identity](fourier-analysis.md#parseval-identity) therefore gives

$$
\frac23=\frac1{2\pi}\int_{-\infty}^{\infty}\left(\frac{\sin(k/2)}{k/2}\right)^4dk=\frac2\pi\int_0^\infty\left(\frac{\sin u}u\right)^4du.
$$

This proves the displayed value. The removable value at zero is one, and the fourth-power decay bounds the tail. The [sinc-squared integral](#sinc-squared-integral) follows similarly from a rectangular function rather than a triangle.

## Fourier space

↑ **Parent:** [Fourier transform](fourier-transform.md)

Fourier space labels a field by the frequency or wavevector variables of its [Fourier transform](fourier-transform.md), rather than by its original coordinates. Spatial gradients act by multiplication by $i\mathbf k$, and the negative [Laplacian](multivariable-calculus.md#laplacian) acts by $k^2$.

## Moment differentiation of the Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

If $f\in L^1(\mathbb R)$ and $x^kf\in L^1(\mathbb R)$ for $0\le k\le r$, then its [Fourier transform](fourier-transform.md) is $r$ times [continuously differentiable](multivariable-calculus.md#continuously-differentiable-function) and the displayed formula holds. The [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) permits each [derivative](calculus.md#derivative) under the [integral](integral.md). Thus $r+1$ [vanishing moments](fourier-analysis.md#vanishing-moment) give a zero [Taylor polynomial](calculus.md#taylor-polynomial) through degree $r$ at the origin. Unweighted $L^1$ membership only guarantees a [continuous function](calculus.md#continuous-function) as the [Fourier transform](fourier-transform.md).

## Fourier transform has proper dense image from L1 to C0

↑ **Parent:** [Fourier transform](fourier-transform.md)

The [Riemann-Lebesgue lemma](fourier-analysis.md#riemann-lebesgue-lemma) and [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) give a bounded injective map $L^1(\mathbb R)\to C_0(\mathbb R)$ with dense image. It is not onto: inverse transforms of $\chi_{[-n,n]}*\chi_{[-1,1]}$ have unbounded $L^1$ norms while the targets have [uniform norm](normed-vector-space.md#supremum-norm) $2$, contradicting the bounded inverse that the [open mapping theorem](functional-analysis.md#open-mapping-theorem-functional-analysis) would give.

## Hankel transform

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hankel_transform)

### Isotropic transverse covariance spectrum

↑ **Parent:** [Hankel transform](#hankel-transform)

For the [Fourier transform](fourier-transform.md) convention $C(\mathbf s)=\int\Phi(\boldsymbol\kappa)e^{i\boldsymbol\kappa\cdot\mathbf s}d^2\kappa/(2\pi)^2$, angular integration of an isotropic [power spectrum](probability-and-statistics.md#power-spectrum) gives the displayed [Hankel transform](#hankel-transform). A purely radial Hankel transform without the prefactor corresponds to defining its spectrum as $\Phi/(2\pi)$.

### Fourier-Hankel normalization for an isotropic spectrum

↑ **Parent:** [Hankel transform](#hankel-transform)

For the Cartesian convention $\widehat f(\mathbf q)=\int_{\mathbb R^2}f(\mathbf r)e^{-i\mathbf q\cdot\mathbf r}d\mathbf r$, an isotropic function has $\widehat f(\nu)=2\pi\int_0^\infty f(r)J_0(\nu r)r\,dr$. Its inverse is $f(r)=(2\pi)^{-1}\int_0^\infty\widehat f(\nu)J_0(\nu r)\nu\,d\nu$. The self-reciprocal [Hankel transform](#hankel-transform) instead uses $F_H=\widehat f/(2\pi)$. In particular $f(0)=\int F_H(\nu)\nu\,d\nu$. Mixing these spectral conventions changes attenuation coefficients by $2\pi$.

## Wigner distribution

↑ **Parent:** [Fourier transform](fourier-transform.md)

The [Wigner distribution](#wigner-distribution) of two fields is the [Fourier transform](fourier-transform.md) of a field's two-point product in its separation variable:

$$
W[u,v](\mathbf z,\mathbf p)=(2\pi)^{-d}\int e^{-i\mathbf p\cdot\mathbf s}u(\mathbf z+\mathbf s/2)\overline{v(\mathbf z-\mathbf s/2)}\,d\mathbf s.
$$

Its inverse reconstructs $u(\mathbf z)\overline{v(\mathbf z')}$. For vector fields, specify whether the product is an outer product or a scalar contraction; the latter can encode an average over receiver channels.

### Optical Wigner function

↑ **Parent:** [Wigner distribution](#wigner-distribution)

For $X_1=x$, $X_2=y$ with $[X_1,X_2]=i/2$, normalize the phase-space function by $\int W(x,y)\,dx\,dy=1$. A [coherent state](quantum-theory.md#coherent-state) of amplitude $\alpha$ has $W=2e^{-2|x+iy-\alpha|^2}/\pi$. Quadrature marginals are physical probability distributions, but the full function can be negative. Cross terms of an [optical cat state](quantum-optics.md#schrodinger-cat-state) give interference fringes, even when low-order moments approach those of a mixture.

### Free Schrodinger Wigner transport

↑ **Parent:** [Wigner distribution](#wigner-distribution)

For $i\Psi_t=-\Delta\Psi/2$, differentiate the two-point product $\Psi(x+y/2)\overline\Psi(x-y/2)$. The difference of its two Laplacians is $2\nabla_x\cdot\nabla_y$, so Fourier transformation in $y$ gives the displayed free-transport equation for the [Wigner transform](#wigner-distribution). Its solution is $w(x,\xi,t)=w(x-t\xi,\xi,0)$.

### Receiver-averaged Wigner distribution

↑ **Parent:** [Wigner distribution](#wigner-distribution)

For receiver-dependent [Green functions](green-s-function.md) $g_{\boldsymbol\zeta}(\mathbf z)$ and [aperture](optics.md#aperture) weight $a(\boldsymbol\zeta)$, define $\mathcal W_A(\mathbf Z,\mathbf p)=\int a(\boldsymbol\zeta)W[g_{\boldsymbol\zeta},g_{\boldsymbol\zeta}](\mathbf Z,\mathbf p)\,d\boldsymbol\zeta$. Its inverse separation [Fourier transform](fourier-transform.md) is the kernel of the [time reversal operator](physics.md#time-reversal-operator) on the source plane.

## Japanese bracket

↑ **Parent:** [Fourier transform](fourier-transform.md)

The Japanese bracket is a smooth positive frequency weight, comparable to $1+|\xi|$. It defines [Sobolev space](sobolev-space.md) norms and the growth estimates of a [symbol class](distribution-theory.md#symbol-class) without singularities at zero frequency.

### Peetre weight inequality

↑ **Parent:** [Japanese bracket](#japanese-bracket)

For real $s$ and vectors $\xi,\eta$, the displayed bound follows from $\langle a+b\rangle\le\sqrt2\langle a\rangle\langle b\rangle$, applied in the opposite direction when $s<0$. One can take $C_s=2^{|s|/2}$. Combined with [Young's convolution inequality](fourier-analysis.md#young-s-convolution-inequality), it proves [Sobolev multiplication by a smooth cutoff](sobolev-space.md#sobolev-multiplication-by-a-smooth-cutoff) for all real orders: the rapidly decreasing transform of the cutoff absorbs the extra weight. The negative-order case is particularly useful when a [distribution](distribution-theory.md#distribution-mathematical-analysis) is not initially a function.

## Fourier shift theorem

↑ **Parent:** [Fourier transform](fourier-transform.md)

For the angular-frequency convention,

$$
\mathcal F[e^{iax}f(x)](k)=\widehat f(k-a),
\qquad
\mathcal F[f(x-a)](k)=e^{-iak}\widehat f(k).
$$

## Fresnel integral

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fresnel_integral)

The Fresnel integral is an oscillatory Gaussian integral. In the angular-frequency convention, its distributional form is

$$
\int_{\mathbb R}e^{i\omega x^2/2-i\lambda x}\,dx
=\sqrt{\frac{2\pi}{|\omega|}}
e^{i\pi\operatorname{sgn}(\omega)/4}
e^{-i\lambda^2/(2\omega)}
$$

for nonzero real $\omega$.

### Optical normalization of Fresnel integrals

↑ **Parent:** [Fresnel integral](#fresnel-integral)

For the optical convention of [Fresnel integrals](#fresnel-integral), $C(w)=\int_0^w\cos(\pi u^2/2)du$ and $S(w)=\int_0^w\sin(\pi u^2/2)du$. Both functions are odd and tend to $1/2$ as $w\to+\infty$. If the unscaled convention uses phase $t^2$, multiply its argument by $\sqrt{\pi/2}$ and its value by $\sqrt{2/\pi}$ to obtain this convention. An aperture factor with phase $\pi x^2/(\lambda R)$ uses $u=x\sqrt{2/(\lambda R)}$. Stating the convention prevents missing factors of $\pi$ or $\sqrt2$ in [diffraction](quantum-scattering.md#diffraction) calculations.

### Finite Fresnel integrals

↑ **Parent:** [Fresnel integral](#fresnel-integral)

In the unscaled convention, the finite [Fresnel integrals](#fresnel-integral) are $C(\lambda)=\int_0^\lambda\cos(t^2)dt$ and $S(\lambda)=\int_0^\lambda\sin(t^2)dt$. Their [Taylor series](calculus.md#taylor-series) follow by termwise integration. At infinity both tend to $\sqrt{\pi/8}$, and their oscillatory tails have [asymptotic expansions](asymptotic-expansion.md) obtained by [integration by parts](calculus.md#integration-by-parts). This convention differs from the convention with phase $\pi t^2/2$.

#### Fresnel tail expansion

↑ **Parent:** [Finite Fresnel integrals](#finite-fresnel-integrals)

For $A=\sqrt{\pi/8}$, define real tail functions by $Q+iP=e^{-i\lambda^2}\int_\lambda^\infty e^{it^2}dt$. Then $C=A+P\sin\lambda^2-Q\cos\lambda^2$ and $S=A-P\cos\lambda^2-Q\sin\lambda^2$. Repeated [integration by parts](calculus.md#integration-by-parts) gives

$$
P\sim\sum_{m\ge0}\frac{(-1)^m(4m-1)!!}{2^{2m+1}\lambda^{4m+1}},\qquad Q\sim\sum_{m\ge0}\frac{(-1)^m(4m+1)!!}{2^{2m+2}\lambda^{4m+3}},
$$

where $(-1)!!=1$. These are [asymptotic expansions](asymptotic-expansion.md), rather than convergent infinite sums at a fixed argument.

### Regulated complex Fresnel integral

↑ **Parent:** [Fresnel integral](#fresnel-integral)

For $\alpha>0$, polar coordinates reduce the integral to $2\pi\int_0^\infty r e^{-(\alpha-i\lambda)r^2}dr$. The result is $\pi/(\alpha-i\lambda)$. Its damped limit for real $\lambda>0$ is $i\pi/\lambda$, which fixes the sign of the oscillatory complex [Gaussian integral](integral.md#gaussian-integral). The [Fresnel integral](#fresnel-integral) convention can be compared with [NIST definitions](https://dlmf.nist.gov/7.2).

### Oscillatory Gaussian integral with negative phase

↑ **Parent:** [Fresnel integral](#fresnel-integral)

For $t>0$, contour rotation of the [Gaussian integral](integral.md#gaussian-integral) gives

$$
\int_{-\infty}^{\infty}e^{-itu^2}du
=e^{-i\pi/4}\sqrt{\frac\pi t}.
$$

## Additive character

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_character)

An additive character of a locally compact field $F$ is a continuous [group homomorphism](group-theory.md#group-homomorphism) from $(F,+)$ to the complex unit circle.

### Character annihilator

↑ **Parent:** [Additive character](#additive-character)

For a nontrivial [additive character](#additive-character) $\psi$ on a [local field](non-archimedean-analysis.md#local-field), the character annihilator of an additive subgroup $H$ is $H^\perp=\{y:\psi(xy)=1\text{ for all }x\in H\}$. If $\mathcal O_F^\perp=\pi^c\mathcal O_F$, then $(\pi^n\mathcal O_F)^\perp=\pi^{c-n}\mathcal O_F$. This is a character pairing construction, distinct from the [annihilator](module-theory.md#annihilator-ring-theory) of a module.

## Fourier transform over a local field

↑ **Parent:** [Fourier transform](fourier-transform.md)

For a [local field](non-archimedean-analysis.md#local-field) $F$, an [additive character](#additive-character) $\psi$, and a [Haar measure](measure.md#haar-measure) $dx$, the Fourier transform is

$$
\widehat f(y)=\int_Ff(x)\psi(xy)\,dx.
$$

It maps the [Schwartz-Bruhat space](fourier-analysis.md#schwartz-bruhat-space) to itself.

### Fourier transform of a ball indicator over a local field

↑ **Parent:** [Fourier transform over a local field](#fourier-transform-over-a-local-field)

For a compact open additive subgroup $H$ of a [local field](non-archimedean-analysis.md#local-field), translation and [additive character](#additive-character) orthogonality give the displayed transform of a coset indicator. With the [self-dual Haar measure](#self-dual-haar-measure), transforming again gives $\mathbf1_{a+H}(-x)$. Every [Schwartz-Bruhat function](fourier-analysis.md#schwartz-bruhat-function) is a finite linear combination of these indicators.

### Self-dual Haar measure

↑ **Parent:** [Fourier transform over a local field](#fourier-transform-over-a-local-field)

Relative to a nontrivial [additive character](#additive-character), the self-dual additive [Haar measure](measure.md#haar-measure) makes the twice-applied [Fourier transform over a local field](#fourier-transform-over-a-local-field) equal to reflection. If the [annihilator of the valuation ring](#annihilator-of-the-valuation-ring) is $\pi^c\mathcal O_F$ and its [residue field](commutative-algebra.md#residue-field) has $q$ elements, the normalization is $\operatorname{vol}(\mathcal O_F)=q^{c/2}$. Volumes of a compact open subgroup and its [character annihilator](#character-annihilator) then multiply to one.

### Annihilator of the valuation ring

↑ **Parent:** [Fourier transform over a local field](#fourier-transform-over-a-local-field)

For an [additive character](#additive-character) $\psi$ of a non-Archimedean [local field](non-archimedean-analysis.md#local-field) $F$,

$$
\mathcal O_F^\perp
=\{y\in F:\psi(xy)=1\text{ for every }x\in\mathcal O_F\}.
$$

For the character induced from the standard character of $\mathbb Q_p$, this annihilator is the [inverse different](non-archimedean-analysis.md#inverse-different).

## Fourier multiplier

↑ **Parent:** [Fourier transform](fourier-transform.md)

A Fourier multiplier is a function $m$ on frequency space used to define an operator by multiplication after taking a [Fourier transform](fourier-transform.md).

### Half-plane Fourier projection

↑ **Parent:** [Fourier multiplier](#fourier-multiplier)

The half-plane Fourier projection is $(I-iH_v)/2$, where $H_v$ is the [directional Hilbert transform](#directional-hilbert-transform). A disk of radius $R$, modulated to put a boundary point at the origin, has symbol $\mathbf1_{\{|\xi+Rv|\le R\}}$, which converges almost everywhere to this half-plane symbol. The [Plancherel theorem](fourier-analysis.md#plancherel-theorem) makes this an $L^2$ multiplier limit.

### Nonintegrability of a radial triangular Fourier cutoff in three dimensions

↑ **Parent:** [Fourier multiplier](#fourier-multiplier)

The inverse [Fourier transform](fourier-transform.md) of $(1-|\xi|)_+$ in three dimensions, with $a=2\pi|x|$, is $-4\pi\sin a/a^3+8\pi(1-\cos a)/a^4$. Its leading oscillatory $|x|^{-3}$ tail is not absolutely integrable against the radial [volume](geometry-and-topology.md#volume) element $4\pi|x|^2d|x|$. Multiplying by a Gaussian [Fourier transform](fourier-transform.md) retains a nonzero boundary-[derivative](calculus.md#derivative) tail, so the radial cutoff need not map even [Schwartz functions](fourier-analysis.md#schwartz-function) into $L^1$. A [tensor product](multilinear-algebra.md#tensor-product) of one-dimensional triangular cutoffs is a valid [approximate identity](fourier-analysis.md#approximate-identity), and must not be confused with this Euclidean radial cutoff.

### Fourier multiplier operator

↑ **Parent:** [Fourier multiplier](#fourier-multiplier)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier_multiplier_operator)

A Fourier multiplier operator $T_m$ is defined by $\widehat{T_mf}(\xi)=m(\xi)\widehat f(\xi)$. On $L^2$, a bounded symbol gives a bounded operator by the [Plancherel theorem](fourier-analysis.md#plancherel-theorem), while an unbounded symbol defines a [closed linear operator](functional-analysis.md#closed-linear-operator) on the functions for which $m\widehat f$ remains square-integrable.

## Fourier transform of a function with reciprocal tails

↑ **Parent:** [Fourier transform](fourier-transform.md)

Suppose $w$ is locally integrable and

$$
w(x)=\frac{c_+}{x}+O(x^{-2})\quad(x\to+\infty),
\qquad
w(x)=\frac{c_-}{x}+O(x^{-2})\quad(x\to-\infty).
$$

Then $\widehat w(\lambda)+(c_+-c_-)\log|\lambda|$ has finite limits at zero from both sides. With the convention $\widehat w(\lambda)=\int e^{-i\lambda x}w(x)dx$, the positive-frequency limit minus the negative-frequency limit is

$$
-i\pi(c_++c_-).
$$

Subtracting suitable reflected copies of $x^{-1}\mathbf1_{(1,\infty)}(x)$ leaves an $L^1$ function, whose Fourier transform is continuous; the jump then follows from the [Dirichlet integral](fourier-analysis.md#dirichlet-integral).

## Scaling property of the Fourier transform

↑ **Parent:** [Fourier transform](fourier-transform.md)

If $f_\lambda(x)=f(\lambda x)$ on $\mathbb R^n$ with $\lambda>0$, then

$$
\widehat {f_\lambda}(\xi)
=\lambda^{-n}\widehat f(\xi/\lambda),
$$

and consequently

$$
\|f_\lambda\|_p=\lambda^{-n/p}\|f\|_p,
\qquad
\|\widehat {f_\lambda}\|_q
=\lambda^{-n(1-1/q)}\|\widehat f\|_q.
$$

### Scaling necessity for an Lp to Lq Fourier bound

↑ **Parent:** [Scaling property of the Fourier transform](#scaling-property-of-the-fourier-transform)

If a nontrivial uniform estimate

$$
\|\widehat f\|_q\leq C\|f\|_p
$$

holds for all integrable $L^p$ functions on $\mathbb R^n$, dilation by every $\lambda>0$ forces

$$
1-\frac1q=\frac1p.
$$

Thus $q$ must be the [conjugate exponent](functional-analysis.md#conjugate-exponents) of $p$.

## Fourier transform of inverse distance in three dimensions

↑ **Parent:** [Fourier transform](fourier-transform.md)

As a [tempered distribution](fourier-analysis.md#tempered-distribution) on $\mathbb R^3$,

$$
\mathcal F(|x|^{-1})(\xi)=C|\xi|^{-2}
$$

for a nonzero convention-dependent constant $C$. One proof writes

$$
|x|^{-1}=C_1\int_0^\infty t^{-1/2}e^{-t|x|^2}\,dt
$$

and applies the [Fourier transform of a Gaussian](fourier-analysis.md#fourier-transform-of-a-gaussian) before substituting $u=|\xi|^2/(4t)$.

## Hilbert transform

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_transform)

With one common sign convention,

$$
Hf(y)=\frac1\pi\operatorname{PV}
\int_{-\infty}^{\infty}\frac{f(x)}{y-x}\,dx.
$$

Reversing the denominator reverses the sign.

### Hilbert transform of the sinc function

↑ **Parent:** [Hilbert transform](#hilbert-transform)

With convention $\mathcal Hf(t)=\pi^{-1}\operatorname{PV}\int f(\tau)/(t-\tau)\,d\tau$, the analytic function $F(z)=(e^{iz}-1)/(iz)$ has removable singularity at zero and decays on large upper semicircles. Its boundary real part is $\sin t/t$ and imaginary part is $(1-\cos t)/t$. The upper-half-plane contour indented above $t$ gives $\operatorname{PV}\int F(\tau)/(\tau-t)\,d\tau=i\pi F(t)$. Taking imaginary parts after reversing the denominator proves the displayed transform, with value zero at $t=0$ by continuous extension.

### Directional Hilbert transform

↑ **Parent:** [Hilbert transform](#hilbert-transform)

For a unit vector $v$, the directional [Hilbert transform](#hilbert-transform) integrates along lines parallel to $v$. Its [Fourier multiplier](#fourier-multiplier) is $-i\operatorname{sgn}(\xi\cdot v)$ under the usual transform convention. Applied to a rectangle whose long axis is $v$, it reduces to the one-dimensional logarithmic tail of an interval [indicator function](measure-theory.md#indicator-function), separately on each transverse coordinate.

### Large-distance tail of the Hilbert transform

↑ **Parent:** [Hilbert transform](#hilbert-transform)

For a [Schwartz function](fourier-analysis.md#schwartz-function) $f$, the [Hilbert transform](#hilbert-transform) satisfies $\mathcal Hf(x)=(\int f)/(\pi x)+o(|x|^{-1})$ at both infinities. Splitting the inverse [Fourier transform](fourier-transform.md) at the sign multiplier's jump and integrating each half-line by parts extracts the zero-frequency value $\widehat f(0)$; the remainder vanishes by the [Riemann-Lebesgue lemma](fourier-analysis.md#riemann-lebesgue-lemma). A nonzero zeroth moment therefore obstructs Schwartz decay.

### Hilbert-transform Fourier multiplier

↑ **Parent:** [Hilbert transform](#hilbert-transform)

For $\mathcal Hf(x)=\pi^{-1}\operatorname{pv}\int f(y)/(x-y)\,dy$ and $\widehat f(\xi)=\int e^{-ix\xi}f(x)dx$, the [Fourier transform](fourier-transform.md) multiplier is $-i\operatorname{sgn}\xi$. The [Heaviside function](integral-transform.md#heaviside-step-function) transform and the double-transform reflection identity give the sign. [Plancherel theorem](fourier-analysis.md#plancherel-theorem) proves the $L^2$ isometry, and multiplication by $i\xi$ proves commutation with differentiation. The map need not preserve the [Schwartz space](fourier-analysis.md#schwartz-space).

## Fourier transform of an interval indicator

↑ **Parent:** [Fourier transform](fourier-transform.md)

For $f=\mathbf1_{[-a,a]}$ and the convention $\widehat f(\xi)=\int f(x)e^{-ix\xi}\,dx$,

$$
\widehat f(\xi)=\frac{2\sin(a\xi)}{\xi},
$$

with its continuous value $2a$ at zero.

## Sinc-squared integral

↑ **Parent:** [Fourier transform](fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sinc-squared_integral)

With the standard Fourier convention, [Plancherel theorem](fourier-analysis.md#plancherel-theorem) applied to $\mathbf1_{[-1,1]}$ gives

$$
\int_{-\infty}^{\infty}\left(\frac{\sin x}{x}\right)^2dx=\pi,
\qquad
\int_0^\infty\left(\frac{\sin x}{x}\right)^2dx=\frac\pi2.
$$

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (694)

- [Advanced Green function](green-s-function.md#advanced-green-function)
- [Airy disk](point-spread-function.md#airy-disk)
- [Airy disk derivation](point-spread-function.md#airy-disk-derivation)
- [Airy equation](integrable-systems.md#airy-equation)
- [Angular spectrum](wave.md#angular-spectrum)
- [Anisotropic theta functional equation](modular-function.md#anisotropic-theta-functional-equation)
- [Aperture synthesis](astrophysics.md#aperture-synthesis)
- [Autocorrelation function of a random field](gaussian-process.md#autocorrelation-function-of-a-random-field)
- [Autocorrelation of a square-integrable function](fourier-analysis.md#autocorrelation-of-a-square-integrable-function)
- [Band-limited linear density correlation](linear-cosmological-density-perturbation.md#band-limited-linear-density-correlation)
- [Bandlimited function](#bandlimited-function)
- [Bilateral exponential forcing of an overdamped oscillator](analysis.md#bilateral-exponential-forcing-of-an-overdamped-oscillator)
- [Bispectrum](time-series.md#bispectrum)
- [Bobylev identity](boltzmann-equation.md#bobylev-identity)
- [Born approximation for scalar wave scattering](inverse-problem.md#born-approximation-for-scalar-wave-scattering)
- [Born non-scattering contrasts at one incident direction](inverse-problem.md#born-non-scattering-contrasts-at-one-incident-direction)
- [Box smoothing of a two-sided exponential](fourier-analysis.md#box-smoothing-of-a-two-sided-exponential)
- [Cauchy convolution semigroup](probability-distribution.md#cauchy-convolution-semigroup)
- [Cauchy principal value](complex-analysis.md#cauchy-principal-value)
- [Causal extension by zero](integral-transform.md#causal-extension-by-zero)
- [Causal Fourier resolvent of a point-driven fixed string](wave-equation.md#causal-fourier-resolvent-of-a-point-driven-fixed-string)
- [Causal Green function of a damped oscillator](analysis.md#causal-green-function-of-a-damped-oscillator)
- [Causal Green function of an overdamped oscillator](analysis.md#causal-green-function-of-an-overdamped-oscillator)
- [Causality versus stability of a Green function](green-s-function.md#causality-versus-stability-of-a-green-function)
- [Character theta transformation](algebraic-number-theory.md#character-theta-transformation)
- [Characteristic function](characteristic-function.md)
- [Chirped Gaussian wave packet](quantum-theory.md#chirped-gaussian-wave-packet)
- [Circle cap Fourier lower bound](fourier-analysis.md#circle-cap-fourier-lower-bound)
- [Complementary transition bands for a scaling function](fourier-analysis.md#complementary-transition-bands-for-a-scaling-function)
- [Complex Gaussian Fourier transform](fourier-analysis.md#complex-gaussian-fourier-transform)
- [Complex spectral Fourier transform](#complex-spectral-fourier-transform)
- [Complex visibility](astrophysics.md#complex-visibility)
- [Contact term in a correlation function](quantum-field-theory.md#contact-term-in-a-correlation-function)
- [Convolution](fourier-analysis.md#convolution)
- [Convolution theorem](fourier-analysis.md#convolution-theorem)
- [Correlation-volume derivation of the scalar Ginzburg ratio](critical-phenomenon.md#correlation-volume-derivation-of-the-scalar-ginzburg-ratio)
- [Coulomb exchange splitting of two orbitals](electromagnetism.md#coulomb-exchange-splitting-of-two-orbitals)
- [Cross-correlation](fourier-analysis.md#cross-correlation)
- [Cutoff bootstrap for local elliptic regularity](distribution-theory.md#cutoff-bootstrap-for-local-elliptic-regularity)
- [Decaying two-sided Green function of a constant-coefficient ordinary differential equation](green-s-function.md#decaying-two-sided-green-function-of-a-constant-coefficient-ordinary-differential-equation)
- [Deconvolution](fourier-analysis.md#deconvolution)
- [Delay-range resolution in Fourier transform spectroscopy](optical-instrument.md#delay-range-resolution-in-fourier-transform-spectroscopy)
- [Delayed cursor feedback experiment](control-theory.md#delayed-cursor-feedback-experiment)
- [Delta derivatives from polynomial oscillatory amplitudes](distribution-theory.md#delta-derivatives-from-polynomial-oscillatory-amplitudes)
- [Delta-shell Born amplitude](quantum-theory.md#delta-shell-born-amplitude)
- [Derivative energy constant for a smooth sieve cutoff](analytic-number-theory.md#derivative-energy-constant-for-a-smooth-sieve-cutoff)
- [Derivative jump of a free scalar time-ordered two-point function](quantum-field-theory.md#derivative-jump-of-a-free-scalar-time-ordered-two-point-function)
- [Diffraction-limited resolution](point-spread-function.md#diffraction-limited-resolution)
- [Diffraction-limited system](point-spread-function.md#diffraction-limited-system)
- [Dirac comb](distribution-theory.md#dirac-comb)
- [Dirty image](astrophysics.md#dirty-image)
- [Discrete Fourier transform](discrete-fourier-transform.md)
- [Dual lattice](fourier-analysis.md#dual-lattice)
- [Duality property of the Fourier transform](#duality-property-of-the-fourier-transform)
- [Dynamic structure factor](critical-phenomenon.md#dynamic-structure-factor)
- [Earth-rotation aperture synthesis](astrophysics.md#earth-rotation-aperture-synthesis)
- [Electric-dipole excitation by a passing ion](atomic-nucleus.md#electric-dipole-excitation-by-a-passing-ion)
- [Entire wave cosine multiplier](wave-equation.md#entire-wave-cosine-multiplier)
- [Exponential forcing of an underdamped oscillator](analysis.md#exponential-forcing-of-an-underdamped-oscillator)
- [Fast-inhibitor elimination in a reaction-diffusion system](diffusion-equation.md#fast-inhibitor-elimination-in-a-reaction-diffusion-system)
- [Finite-seed local extinction in the voter model](stochastic-process.md#finite-seed-local-extinction-in-the-voter-model)
- [Fixed-frequency nonradiating source](physics.md#fixed-frequency-nonradiating-source)
- [Flat-top kernel for density estimation](nonparametric-statistics.md#flat-top-kernel-for-density-estimation)
- [Focal ratio](optical-instrument.md#focal-ratio)
- [Force-extension of an intrinsically curved filament](elasticity-physics.md#force-extension-of-an-intrinsically-curved-filament)
- [Four-slit Fraunhofer diffraction](physical-optics.md#four-slit-fraunhofer-diffraction)
- [Fourier analysis](fourier-analysis.md)
- [Fourier cosine transform](#fourier-cosine-transform)
- [Fourier decay from a derivative jump](#fourier-decay-from-a-derivative-jump)
- [Fourier decay of repeated interval convolutions](fourier-analysis.md#fourier-decay-of-repeated-interval-convolutions)
- [Fourier diffraction theorem](inverse-problem.md#fourier-diffraction-theorem)
- [Fourier distance of order two](boltzmann-equation.md#fourier-distance-of-order-two)
- [Fourier extension operator](fourier-analysis.md#fourier-extension-operator)
- [Fourier Green function in a spatially varying background](green-s-function.md#fourier-green-function-in-a-spatially-varying-background)
- [Fourier independence from disjoint distribution supports](distribution-theory.md#fourier-independence-from-disjoint-distribution-supports)
- [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem)
- [Fourier mode](fourier-analysis.md#fourier-mode)
- [Fourier model of a Lyot coronagraph](optics.md#fourier-model-of-a-lyot-coronagraph)
- [Fourier multiplier](#fourier-multiplier)
- [Fourier shell correlation](fourier-analysis.md#fourier-shell-correlation)
- [Fourier sine transform](#fourier-sine-transform)
- [Fourier solution of the strip Dirichlet problem](partial-differential-equation.md#fourier-solution-of-the-strip-dirichlet-problem)
- [Fourier space](#fourier-space)
- [Fourier transform isomorphism of the Schwartz space](#fourier-transform-isomorphism-of-the-schwartz-space)
- [Fourier transform microwave spectroscopy](molecule.md#fourier-transform-microwave-spectroscopy)
- [Fourier transform of a compactly supported distribution](distribution-theory.md#fourier-transform-of-a-compactly-supported-distribution)
- [Fourier transform of a finite measure](#fourier-transform-of-a-finite-measure)
- [Fourier transform of a polynomial multiple](#fourier-transform-of-a-polynomial-multiple)
- [Fourier transform of a tempered distribution](fourier-analysis.md#fourier-transform-of-a-tempered-distribution)
- [Fourier transform of a truncated cosine](#fourier-transform-of-a-truncated-cosine)
- [Fourier transform of the Bessel function J0](bessel-function.md#fourier-transform-of-the-bessel-function-j0)
- [Fourier transform of the hyperbolic secant](#fourier-transform-of-the-hyperbolic-secant)
- [Fourier transform of the modified Bessel function K0](bessel-function.md#fourier-transform-of-the-modified-bessel-function-k0)
- [Fourier transform spectroscopy](optical-instrument.md#fourier-transform-spectroscopy)
- [Fourth-order Green kernel with two decay scales](green-s-function.md#fourth-order-green-kernel-with-two-decay-scales)
- [Fraunhofer diffraction](physical-optics.md#fraunhofer-diffraction)
- [Free-transport phase mixing](kinetic-theory.md#free-transport-phase-mixing)
- [Frequency spectrum](fourier-analysis.md#frequency-spectrum)
- [Fresnel diffraction phase curvature](physical-optics.md#fresnel-diffraction-phase-curvature)
- [Fresnel slit propagation](physical-optics.md#fresnel-slit-propagation)
- [Front velocity](dispersion-relation.md#front-velocity)
- [Gaussian chirped pulse compression](laser.md#gaussian-chirped-pulse-compression)
- [Gaussian limit of the end-to-end distribution of a freely jointed chain](mathematical-biology.md#gaussian-limit-of-the-end-to-end-distribution-of-a-freely-jointed-chain)
- [Gaussian Poisson summation identity](fourier-analysis.md#gaussian-poisson-summation-identity)
- [Gaussian semivariogram](statistical-modelling.md#gaussian-semivariogram)
- [Gaussian shell covariance](critical-phenomenon.md#gaussian-shell-covariance)
- [Geostrophic adjustment of a Gaussian height ridge](geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-gaussian-height-ridge)
- [Goldstone theorem](quantum-field-theory.md#goldstone-theorem)
- [Gravitational potential evolution of a barotropic fluid](linear-cosmological-perturbation-theory.md#gravitational-potential-evolution-of-a-barotropic-fluid)
- [Green function of the linear complex Ginzburg-Landau equation](partial-differential-equation.md#green-function-of-the-linear-complex-ginzburg-landau-equation)
- [Ground-state energy](quantum-mechanics.md#ground-state-energy)
- [Half-line advection-diffusion global relation](diffusion-equation.md#half-line-advection-diffusion-global-relation)
- [Half-line drift null contour identity](#half-line-drift-null-contour-identity)
- [Hankel inversion of a rotation-measure correlation](electromagnetic-wave.md#hankel-inversion-of-a-rotation-measure-correlation)
- [Harmonic analysis](harmonic-analysis.md)
- [Harmonic chain](classical-mechanics.md#harmonic-chain)
- [Hasselmann stochastic climate model](geophysics.md#hasselmann-stochastic-climate-model)
- [Heisenberg uncertainty relation](quantum-theory.md#heisenberg-uncertainty-relation)
- [Helioseismology](astrophysical-fluid-dynamics.md#helioseismology)
- [Hermite function](orthogonal-polynomial.md#hermite-function)
- [Hermite functions are Fourier eigenfunctions](orthogonal-polynomial.md#hermite-functions-are-fourier-eigenfunctions)
- [Hermitian symmetry](#hermitian-symmetry)
- [Hilbert-transform Fourier multiplier](#hilbert-transform-fourier-multiplier)
- [Homogeneous distribution](distribution-theory.md#homogeneous-distribution)
- [Homogeneous Sobolev space](sobolev-space.md#homogeneous-sobolev-space)
- [Inferring a binary from a detector network](gravitational-wave.md#inferring-a-binary-from-a-detector-network)
- [Infinite-aperture spectral normalization](time-series.md#infinite-aperture-spectral-normalization)
- [Inflationary scalar Fourier mode](cosmic-inflation.md#inflationary-scalar-fourier-mode)
- [Integer-frequency zeros of a scaling function](fourier-analysis.md#integer-frequency-zeros-of-a-scaling-function)
- [Interferogram](physical-optics.md#interferogram)
- [Interferogram apodization](optical-instrument.md#interferogram-apodization)
- [Inverse Fourier transform](#inverse-fourier-transform)
- [Inverse scattering problem](inverse-problem.md#inverse-scattering-problem)
- [Isotropic cosmological correlation-power-spectrum relation](large-scale-structure-of-the-universe.md#isotropic-cosmological-correlation-power-spectrum-relation)
- [Isotropic transverse covariance spectrum](#isotropic-transverse-covariance-spectrum)
- [Kelvin-Voigt rod Green function](rheology.md#kelvin-voigt-rod-green-function)
- [Klein-Gordon plane-wave normalization](quantum-field-theory.md#klein-gordon-plane-wave-normalization)
- [L2 density from a square-integrable Fourier transform](fourier-analysis.md#l2-density-from-a-square-integrable-fourier-transform)
- [Laplace transform](integral-transform.md#laplace-transform)
- [Large-distance tail of the Hilbert transform](#large-distance-tail-of-the-hilbert-transform)
- [LIGO displacement readout and control](gravitational-wave.md#ligo-displacement-readout-and-control)
- [Line-forced fluid-loaded bending plate](elasticity-physics.md#line-forced-fluid-loaded-bending-plate)
- [Linear configuration count](additive-combinatorics.md#linear-configuration-count)
- [Linear dispersive Stokes equation](integrable-systems.md#linear-dispersive-stokes-equation)
- [Lippmann fringe spacing](optics.md#lippmann-fringe-spacing)
- [Locally compact group](topological-group.md#locally-compact-group)
- [Logarithmically smoothed Perron formula](analytic-number-theory.md#logarithmically-smoothed-perron-formula)
- [Long-path projection of a magnetic correlation](electromagnetic-wave.md#long-path-projection-of-a-magnetic-correlation)
- [Lorentzian quasiparticle spectral peak](quantum-field-theory.md#lorentzian-quasiparticle-spectral-peak)
- [Low-frequency decomposition of the wave propagator](wave-equation.md#low-frequency-decomposition-of-the-wave-propagator)
- [Magnetic energy spectrum](electromagnetic-wave.md#magnetic-energy-spectrum)
- [Mellin transform](integral-transform.md#mellin-transform)
- [Mellin transform in logarithmic coordinates](integral-transform.md#mellin-transform-in-logarithmic-coordinates)
- [Modulation property of the Fourier transform](#modulation-property-of-the-fourier-transform)
- [Mollifier regularization for contour recovery of support](distribution-theory.md#mollifier-regularization-for-contour-recovery-of-support)
- [Moment differentiation of the Fourier transform](#moment-differentiation-of-the-fourier-transform)
- [Momentum representation in quantum mechanics](wave-function.md#momentum-representation-in-quantum-mechanics)
- [Momentum-shell decomposition of a scalar field](perturbative-quantum-field-theory.md#momentum-shell-decomposition-of-a-scalar-field)
- [Momentum-space propagator in a uniform force](quantum-system.md#momentum-space-propagator-in-a-uniform-force)
- [Mössbauer velocity scan](mossbauer-effect.md#mossbauer-velocity-scan)
- [MRA projection Fourier identity](fourier-analysis.md#mra-projection-fourier-identity)
- [Mukhanov-Sasaki variable](cosmic-inflation.md#mukhanov-sasaki-variable)
- [Narrow resonance and instrumental resolution](particle-detection.md#narrow-resonance-and-instrumental-resolution)
- [Negative Sobolev regularity of a compactly supported distribution](distribution-theory.md#negative-sobolev-regularity-of-a-compactly-supported-distribution)
- [NIST trace-gas FTMW validation experiment](molecule.md#nist-trace-gas-ftmw-validation-experiment)
- [Nonintegrability of a radial triangular Fourier cutoff in three dimensions](#nonintegrability-of-a-radial-triangular-fourier-cutoff-in-three-dimensions)
- [Nuclear charge form factor](atomic-nucleus.md#nuclear-charge-form-factor)
- [Nuclear elastic electron scattering cross-section](atomic-nucleus.md#nuclear-elastic-electron-scattering-cross-section)
- [Nuclear resonance linewidth](nuclear-magnetic-resonance.md#nuclear-resonance-linewidth)
- [Nyquist–Shannon sampling theorem](fourier-analysis.md#nyquist-shannon-sampling-theorem)
- [Off-axis holography](physical-optics.md#off-axis-holography)
- [Off-plane razor-thin Poisson kernel](astrophysical-disk.md#off-plane-razor-thin-poisson-kernel)
- [One-dimensional retarded wave Green function](wave-equation.md#one-dimensional-retarded-wave-green-function)
- [One-dimensional transverse Fresnel propagation](partial-differential-equation.md#one-dimensional-transverse-fresnel-propagation)
- [Optical transfer function](point-spread-function.md#optical-transfer-function)
- [Optical trap Langevin calibration](optics.md#optical-trap-langevin-calibration)
- [Paley–Wiener–Schwartz theorem](distribution-theory.md#paley-wiener-schwartz-theorem)
- [Paley–Wiener theorem](distribution-theory.md#paley-wiener-theorem)
- [Parametric-rate kernel estimation of a bandlimited density](nonparametric-statistics.md#parametric-rate-kernel-estimation-of-a-bandlimited-density)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2013/paper-1.md#1/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2013/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019.md#section-b/6/solution)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#16e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-50.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-72.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-72.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-72.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1.md#7b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4.md#8b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-64.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-8.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2.md#16b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-44.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-58.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-58.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-66.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-66.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4.md#15a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4.md#15a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4.md#5a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-59.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-59.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-61.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-7.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76.md#1/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76.md#5/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#33b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#29c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#30a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-52.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-79.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#15d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2.md#37c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#33a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-13.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-88.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#14d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#14d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#32d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#30a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#30a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#29a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-51.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-86.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#16a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#37b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#25j/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#25j/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#30c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#30c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-48.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-50.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-81.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-88.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-88.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3.md#6a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4.md#15d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#38a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#30b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#30b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-43.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#14e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#14e/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#30e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-46.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-46.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-64.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-67.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-68.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-49.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-50.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-68.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/b/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/b/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4.md#17c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-6.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-6.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-6.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-60.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67.md#4/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-9.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-9.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#16d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40.md#1/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-44.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-44.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-53.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-67.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-67.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-69.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-75.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-75.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#36b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#30e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#31a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-28.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-45.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-46.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-70.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#15b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#15b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#4a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-303.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-304.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-304.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-312.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-327.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-327.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331.md#3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#14b/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#14b/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#14b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#14a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#24j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#24j/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#20f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#20f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#20f/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#22f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#22f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#22f/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-312.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338.md#3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-310.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-312.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-327.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-327.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#2/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3.md#15d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#26k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-147.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-312.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-327.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-327.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-335.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#4b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#13b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#39b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#23i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#23i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2.md#14a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#15b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#22h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#22h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-312.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-312.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-346.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3.md#3a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#23g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-117.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-312.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-319.md#1/g/solution)
- [B](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327.md#1/b)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-344.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#1a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#11f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#14a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#14a/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4.md#14a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#23f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#23f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#13c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#22f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#39c/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-303.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-310.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-312.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-321.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-321.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-335.md#2/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-344.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-303.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-304.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327.md#1/b/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-335.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-335.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337.md#2/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-342.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-129.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-205.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-311.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-326.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-327.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-335.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-217.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-321.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-327.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2.md#5/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#4/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1.md#4/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#8/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#8/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#8/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2.md#5/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#4/d/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/8/iv/a/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2012/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2014/paper-1.md#4/solution)
- [Spectrometer and resolution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2018.md#section-b/b2/spectrometer-and-resolution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021.md#section-b/b5/c/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-1.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1.md#section-d/d12/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1.md#section-d/d12/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-2.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-d/d13/b/solution)
- [Wavepacket derivation of group velocity](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b7/wavepacket-derivation-of-group-velocity)
- [Convolution and a finite slit array](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b8/convolution-and-a-finite-slit-array)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2.md#section-b/b7/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2.md#section-b/b8/e/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2.md#section-d/d13/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-b/b8/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2.md#section-b/b6/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2.md#section-b/b7/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-b/b2/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#b7/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017.md#4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1.md#1/d/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2014/paper-1.md#5/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2014/paper-1.md#5/c/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1.md#3/b/solution)
- [Causal support and contour conditions](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2017.md#4/a/causal-support-and-contour-conditions)
- [Frequency-space inverse](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2017.md#4/a/frequency-space-inverse)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#4/c/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2013/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2019.md#2/d/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/solution)
- [Patterson map](physical-chemistry.md#patterson-map)
- [Periodization of a Schwartz function](fourier-analysis.md#periodization-of-a-schwartz-function)
- [Point-force radiation from a fluid-loaded sheet](linear-acoustics.md#point-force-radiation-from-a-fluid-loaded-sheet)
- [Poisson summation formula](fourier-analysis.md#poisson-summation-formula)
- [Poisson summation formula for a Euclidean lattice](fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice)
- [Pole subtraction in a Wiener-Hopf equation](boundary-value-problem.md#pole-subtraction-in-a-wiener-hopf-equation)
- [Power spectrum of surface height](physics.md#power-spectrum-of-surface-height)
- [Proca time-ordering contact term](electromagnetism.md#proca-time-ordering-contact-term)
- [Purcell nuclear resonance absorption experiment](nuclear-magnetic-resonance.md#purcell-nuclear-resonance-absorption-experiment)
- [Radial Fourier representation of the Helmholtz Green function](partial-differential-equation.md#radial-fourier-representation-of-the-helmholtz-green-function)
- [Radial induced-charge screening kernel](quantum-mechanics.md#radial-induced-charge-screening-kernel)
- [Rayleigh integral for baffled acoustic radiation](linear-acoustics.md#rayleigh-integral-for-baffled-acoustic-radiation)
- [Receiver-averaged Wigner distribution](#receiver-averaged-wigner-distribution)
- [Rectangular function](electrical-engineering.md#rectangular-function)
- [Residual amplitude of an oscillator after an integrable force](analysis.md#residual-amplitude-of-an-oscillator-after-an-integrable-force)
- [Retarded Fourier pole prescription](distribution-theory.md#retarded-fourier-pole-prescription)
- [Retarded fundamental solution of a constant-coefficient ordinary differential operator](distribution-theory.md#retarded-fundamental-solution-of-a-constant-coefficient-ordinary-differential-operator)
- [Retarded unit-frequency oscillator response](quantum-field-theory.md#retarded-unit-frequency-oscillator-response)
- [Rotation equivariance of the Fourier transform](fourier-analysis.md#rotation-equivariance-of-the-fourier-transform)
- [Roth density-increment step](additive-combinatorics.md#roth-density-increment-step)
- [Sampling expansion by periodic Fourier projection](fourier-analysis.md#sampling-expansion-by-periodic-fourier-projection)
- [Scale-free density correlation transform](linear-cosmological-density-perturbation.md#scale-free-density-correlation-transform)
- [Schrödinger equation](mathematical-physics.md#schrodinger-equation)
- [Schwartz seminorm](fourier-analysis.md#schwartz-seminorm)
- [Self-convolution of a bilateral exponential](fourier-analysis.md#self-convolution-of-a-bilateral-exponential)
- [Shannon scaling mask](fourier-analysis.md#shannon-scaling-mask)
- [Shot noise spectral convention](electrical-engineering.md#shot-noise-spectral-convention)
- [Sinc fourth-power integral](#sinc-fourth-power-integral)
- [Sinc function](#sinc-function)
- [Sixth Fourier moment as a three-sum collision count](additive-combinatorics.md#sixth-fourier-moment-as-a-three-sum-collision-count)
- [Smooth-mask vanishing-moment criterion](fourier-analysis.md#smooth-mask-vanishing-moment-criterion)
- [Smooth-window Fourier coefficients of a periodic distribution](fourier-series.md#smooth-window-fourier-coefficients-of-a-periodic-distribution)
- [Sobolev duality](sobolev-space.md#sobolev-duality)
- [Sobolev multiplication by a smooth cutoff](sobolev-space.md#sobolev-multiplication-by-a-smooth-cutoff)
- [Source-position-dependent Fourier Green function](green-s-function.md#source-position-dependent-fourier-green-function)
- [Source-to-far-field operator at fixed frequency](physics.md#source-to-far-field-operator-at-fixed-frequency)
- [Spectral leakage](#spectral-leakage)
- [Spectral measure of a stationary random field](time-series.md#spectral-measure-of-a-stationary-random-field)
- [Spectral phase](physical-optics.md#spectral-phase)
- [Spectral phase in pulse compression](laser.md#spectral-phase-in-pulse-compression)
- [Spectral pulse shaping](optics.md#spectral-pulse-shaping)
- [Spectral tensor](probability-and-statistics.md#spectral-tensor)
- [Spectrogram](fourier-analysis.md#spectrogram)
- [Spherical surface measure convolution](distribution-theory.md#spherical-surface-measure-convolution)
- [Spherical top-hat window function](linear-cosmological-density-perturbation.md#spherical-top-hat-window-function)
- [Split-step Fourier method](partial-differential-equation.md#split-step-fourier-method)
- [Square-pulse resonance profile](quantum-mechanics.md#square-pulse-resonance-profile)
- [Squared derivative correlations force frequency-graph energy](additive-combinatorics.md#squared-derivative-correlations-force-frequency-graph-energy)
- [Static structure factor](critical-phenomenon.md#static-structure-factor)
- [Stationary no-runaway response and preacceleration](electromagnetic-radiation.md#stationary-no-runaway-response-and-preacceleration)
- [Tempered distribution](fourier-analysis.md#tempered-distribution)
- [Temporal optical coherence](physical-optics.md#temporal-optical-coherence)
- [Thermal damping of a sinusoidal density of states](quantum-ideal-gas-statistics.md#thermal-damping-of-a-sinusoidal-density-of-states)
- [Thin-disk potential-density inversion](astrophysical-disk.md#thin-disk-potential-density-inversion)
- [Translation of a function](function.md#translation-of-a-function)
- [Translation property of the Fourier transform](fourier-analysis.md#translation-property-of-the-fourier-transform)
- [Transverse tangent correlation of a stretched worm-like chain](mathematical-biology.md#transverse-tangent-correlation-of-a-stretched-worm-like-chain)
- [Triangular pulse splitting under the wave equation](wave-equation.md#triangular-pulse-splitting-under-the-wave-equation)
- [Trigonometric integral](integral.md#trigonometric-integral)
- [Trispectrum](time-series.md#trispectrum)
- [Two-path attosecond phase reconstruction](laser.md#two-path-attosecond-phase-reconstruction)
- [Two-point-source aperture synthesis](astrophysics.md#two-point-source-aperture-synthesis)
- [Uniform-disk stellar visibility](quantum-optics.md#uniform-disk-stellar-visibility)
- [Uniqueness of Fourier coefficients in L1](fourier-series.md#uniqueness-of-fourier-coefficients-in-l1)
- [Van Cittert-Zernike theorem](physical-optics.md#van-cittert-zernike-theorem)
- [Vanishing moments and Fourier zeros](fourier-analysis.md#vanishing-moments-and-fourier-zeros)
- [Velocity correlation tensor](turbulence.md#velocity-correlation-tensor)
- [Visibility of a uniform rectangular source](astrophysics.md#visibility-of-a-uniform-rectangular-source)
- [Wiener-Hopf solution of rigid half-plane diffraction](partial-differential-equation.md#wiener-hopf-solution-of-rigid-half-plane-diffraction)
- [Wiener-Khinchin theorem](fourier-analysis.md#wiener-khinchin-theorem)
- [Wigner distribution](#wigner-distribution)
- [Window function](#window-function)
