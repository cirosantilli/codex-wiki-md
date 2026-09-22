# Integral transform

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_transform)

An integral transform maps a function to a new function by integration against a kernel.

**Table of contents**

- [Weierstrass transform](#weierstrass-transform)
- [Spherical mean](#spherical-mean)
- [Radon transform](#radon-transform)
  - [Filtered backprojection](#filtered-backprojection)
  - [Attenuated Radon transform](#attenuated-radon-transform)
    - [Spectral reconstruction of an attenuated Radon transform](#spectral-reconstruction-of-an-attenuated-radon-transform)
      - [Projection formula for inverse attenuated Radon transform](#projection-formula-for-inverse-attenuated-radon-transform)
      - [Complexified transport Cauchy kernel](#complexified-transport-cauchy-kernel)
- [Mellin transform](#mellin-transform)
  - [Restricted Mellin transform on the unit interval](#restricted-mellin-transform-on-the-unit-interval)
  - [Mellin integral of a reciprocal binomial](#mellin-integral-of-a-reciprocal-binomial)
  - [Mellin transform of an interval indicator](#mellin-transform-of-an-interval-indicator)
  - [Fundamental strip of a Mellin transform](#fundamental-strip-of-a-mellin-transform)
  - [Scaling property of the Mellin transform](#scaling-property-of-the-mellin-transform)
  - [Mellin transform in logarithmic coordinates](#mellin-transform-in-logarithmic-coordinates)
  - [Imaginary-part regularization at a zero Mellin exponent](#imaginary-part-regularization-at-a-zero-mellin-exponent)
  - [Mellin transform of call prices](#mellin-transform-of-call-prices)
  - [Meromorphic continuation of a Mellin transform from an asymptotic expansion](#meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion)
    - [Accumulating asymptotic exponents obstruct Mellin continuation](#accumulating-asymptotic-exponents-obstruct-mellin-continuation)
  - [Mellin inversion theorem](#mellin-inversion-theorem)
- [Laplace transform](#laplace-transform)
  - [Exponential order](#exponential-order)
  - [Region of absolute convergence of a Laplace transform](#region-of-absolute-convergence-of-a-laplace-transform)
  - [Causal extension by zero](#causal-extension-by-zero)
  - [Ramanujan's function](#ramanujan-s-function)
    - [Logarithmic expansion of Ramanujan's function](#logarithmic-expansion-of-ramanujan-s-function)
  - [Newman Tauberian theorem](#newman-tauberian-theorem)
    - [Contour damping for bounded Laplace transforms](#contour-damping-for-bounded-laplace-transforms)
  - [Convolution theorem for Laplace transforms](#convolution-theorem-for-laplace-transforms)
  - [Bromwich inversion formula](#bromwich-inversion-formula)
    - [Causality in finite-time Laplace contour inversion](#causality-in-finite-time-laplace-contour-inversion)
  - [Long-time asymptotics from a Laplace transform](#long-time-asymptotics-from-a-laplace-transform)
  - [Laplace transform of a derivative](#laplace-transform-of-a-derivative)
  - [Laplace transform shift theorem](#laplace-transform-shift-theorem)
    - [Laplace transform time-shift rule](#laplace-transform-time-shift-rule)
    - [Heaviside step function](#heaviside-step-function)
  - [Laplace transform of a periodic function](#laplace-transform-of-a-periodic-function)
  - [Matrix-valued Laplace transform](#matrix-valued-laplace-transform)
    - [Laplace-transform solution of a constant-coefficient vector ODE](#laplace-transform-solution-of-a-constant-coefficient-vector-ode)

## Weierstrass transform

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_transform)

The [Weierstrass transform](#weierstrass-transform) is [Gaussian](probability-distribution.md#normal-distribution) [convolution](fourier-analysis.md#convolution), $Wf(x)=(4\pi)^{-1/2}\int_{\mathbb R}e^{-(x-y)^2/4}f(y)\,dy$. It smooths appropriate functions and is the [heat semigroup](diffusion-equation.md#heat-semigroup) at unit time. The [Brownian transition semigroup](brownian-motion.md#brownian-transition-semigroup) uses variance-$t$ Gaussian kernels and therefore supplies the scaled time family.

## Spherical mean

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spherical_mean)

The spherical mean of a function on $\mathbb R^n$ is its average over a sphere:

$$
M_rf(x)=\frac1{|S^{n-1}|}\int_{S^{n-1}}f(x+r\omega)\,d\omega.
$$

## Radon transform

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radon_transform)

The Radon transform integrates a function over affine hyperplanes:

$$
\mathcal Rf(s,\omega)=\int_{x\cdot\omega=s}f(x)\,dA_x.
$$

### Filtered backprojection

↑ **Parent:** [Radon transform](#radon-transform)

The [Radon transform](#radon-transform) records line integrals of a planar density. Apply the transverse [Hilbert transform](fourier-transform.md#hilbert-transform) and a derivative to each projection, then average the filtered values over all lines through the reconstruction point. With $Hh(\rho)=\pi^{-1}\operatorname{PV}\int h(r)/(\rho-r)dr$, the filter has [Fourier multiplier](fourier-transform.md#fourier-multiplier) $|\kappa|$. The [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem), or the jump of the [complexified transport Cauchy kernel](#complexified-transport-cauchy-kernel), proves the displayed formula. The factor is $1/(2\pi)$ when directions are integrated over a half-circle. The growing [Fourier multiplier](fourier-transform.md#fourier-multiplier) explains amplification of measurement noise and the need for [regularization of an inverse problem](inverse-problem.md#regularization-of-an-inverse-problem).

### Attenuated Radon transform

↑ **Parent:** [Radon transform](#radon-transform)

The integral of a source over a directed line, weighted by exponential absorption between each source point and a detector. For line coordinates $x=p\boldsymbol n+s\boldsymbol d$ and a detector at the negative end, it is $\int f(p,s)\exp[-\int_{-\infty}^s\mu(p,r)dr]ds$. The [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) of a [transport equation](transport-equation.md) derives the weight. Reversing the detector direction changes the weight for spatially varying attenuation, so the two directed measurements need not coincide. Setting $\mu=0$ recovers the [Radon transform](#radon-transform).

#### Spectral reconstruction of an attenuated Radon transform

↑ **Parent:** [Attenuated Radon transform](#attenuated-radon-transform)

Complexifying the directional [transport equation](transport-equation.md) yields spectral solutions analytic inside and outside the unit circle. An [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) built from known attenuation removes its multiplication term. The limiting Green kernels encode weighted line measurements and transverse [Hilbert transforms](fourier-transform.md#hilbert-transform). Their jump gives a [Riemann-Hilbert problem](boundary-value-problem.md#riemann-hilbert-problem); its solution recovers the source from an asymptotic coefficient. A general primary treatment of this spectral construction is [https://www.stat.uchicago.edu/~guillaumebal/PAPERS/AttRadTh.pdf](https://www.stat.uchicago.edu/~guillaumebal/PAPERS/AttRadTh.pdf) .

##### Projection formula for inverse attenuated Radon transform

↑ **Parent:** [Spectral reconstruction of an attenuated Radon transform](#spectral-reconstruction-of-an-attenuated-radon-transform)

Let $F(\rho,\tau,\theta)=\int_\tau^\infty f(s\boldsymbol d+\rho\boldsymbol n)ds$, $S=\mathcal Rf$, and $A=\int_{\mathbb R}e^{-F}g\,d\tau$ be the directed [attenuated Radon transform](#attenuated-radon-transform). With the [signed Cauchy boundary operators](holomorphic-function.md#signed-cauchy-boundary-operators), set $J=e^F[e^{P^-S}P^-(e^{-P^-S}A)+e^{-P^+S}P^+(e^{P^+S}A)]$. An [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) turns the attenuated equation into unattenuated directional transport; its spectral solution has jump $-J$ on the unit circle. A normalized [Cauchy integral formula](analysis.md#cauchy-integral-formula) and the coefficient at spectral infinity then prove the reconstruction formula. Known attenuation and full directed angular data determine the source; attenuation itself is not reconstructed by this pair.

##### Complexified transport Cauchy kernel

↑ **Parent:** [Spectral reconstruction of an attenuated Radon transform](#spectral-reconstruction-of-an-attenuated-radon-transform)

For $w=x_1+ix_2$ and $0<|k|\ne1$, the operator $D_k=(k+k^{-1})\partial_{x_1}/2+(k-k^{-1})\partial_{x_2}/(2i)$ has the displayed decaying [fundamental solution](distribution-theory.md#fundamental-solution-of-a-linear-differential-operator). A rotated real-linear coordinate turns it into a multiple of a [Wirtinger derivative](analysis.md#wirtinger-derivatives), reducing the kernel identity to $\partial_{\bar z}(1/(\pi z))=\delta$. The kernel is analytic in $k$ separately inside and outside the unit circle, is $O(k)$ at zero and $O(k^{-1})$ at infinity, and develops a jump at the real directional-transport limit.

## Mellin transform

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mellin_transform)

The [Mellin transform](#mellin-transform) is an [integral transform](integral-transform.md) suited to changes of scale: replacing $f(x)$ by $f(ax)$ multiplies its transform by $a^{-s}$ for $a>0$. For a [locally integrable function](distribution-theory.md#locally-integrable-function) $f:(0,\infty)\to\mathbb C$, define

$$
\mathcal Mf(s)=\int_0^\infty x^{s-1}f(x)\,dx,\qquad s=\sigma+i\tau,
$$

where the [improper integral](real-analysis.md#improper-integral) converges. The [complex number](complex-analysis.md#complex-number) $x^{s-1}=\exp((s-1)\log x)$ uses the real [natural logarithm](calculus.md#natural-logarithm) because $x>0$. Its [absolute value](real-analysis.md#absolute-value) is $x^{\sigma-1}$, so [absolute convergence](sequence-and-series.md#absolute-convergence) depends on the [real part](complex-analysis.md#real-part) $\sigma$ rather than the [imaginary part](complex-analysis.md#imaginary-part) $\tau$. The [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) records the open range of such [real parts](complex-analysis.md#real-part).[Chapter 2, §2.5(i), equation 2.5.1 and the following strip-of-analyticity paragraph](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

A familiar example is the [exponential function](calculus.md#exponential-function) $f(x)=e^{-x}$:

$$
\mathcal M\{e^{-x}\}(s)=\Gamma(s),\qquad \operatorname{Re}s>0.
$$

This is exactly the [Gamma integral](complex-analysis.md#gamma-integral). Near zero $e^{-x}$ tends to one, so [absolute convergence](sequence-and-series.md#absolute-convergence) requires $\sigma>0$; at infinity $x^r e^{-x}\to0$ for every real $r$, so there is no upper boundary. The [Gamma function](complex-analysis.md#gamma-function) has a [meromorphic continuation](holomorphic-function.md#meromorphic-continuation) with [simple poles](isolated-singularity.md#simple-pole) at $0,-1,-2,\ldots$, but a finite continued value elsewhere in $\sigma\leq0$ does not make the defining [improper integral](real-analysis.md#improper-integral) converge.[Chapter 5, §5.2(i), equation 5.2.1, its Re z \> 0 condition, and the following analytic-continuation paragraph](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

The [Mellin transform of an interval indicator](#mellin-transform-of-an-interval-indicator) gives an elementary example with [absolute convergence](sequence-and-series.md#absolute-convergence) for every [complex number](complex-analysis.md#complex-number) $s$. The [Mellin transform in logarithmic coordinates](#mellin-transform-in-logarithmic-coordinates) explains why changes of scale become [translations](geometry-and-topology.md#translation-geometry), connecting the [scaling property of the Mellin transform](#scaling-property-of-the-mellin-transform) to the [Fourier transform](fourier-transform.md).

### Restricted Mellin transform on the unit interval

↑ **Parent:** [Mellin transform](#mellin-transform)

This is the [Mellin transform](#mellin-transform) of the function extended by zero beyond the unit interval. The [change of variables](multivariable-calculus.md#change-of-variables-formula) $\lambda=e^{-t}$ identifies it with the unilateral [Laplace transform](#laplace-transform) of $h(e^{-t})$. The [Bromwich inversion formula](#bromwich-inversion-formula) therefore gives $h(\lambda)=(2\pi i)^{-1}\int_{\gamma-i\infty}^{\gamma+i\infty}\lambda^{-s}H(s)\,ds$ for $0<\lambda<1$, with $\gamma$ in the convergence half-plane and suitable inversion hypotheses. At a jump, symmetric inversion returns the mean of the two limiting values. In particular, for $0<c<1$, the cutoff $h(\lambda)=\lambda^q\mathbf1_{(0,c)}(\lambda)$ has transform $c^{s+q}/(s+q)$ when $\operatorname{Re}(s+q)>0$. Multiplication by $c^s$ shifts the support threshold in logarithmic coordinates, the [Laplace transform time-shift rule](#laplace-transform-time-shift-rule) expressed multiplicatively.

### Mellin integral of a reciprocal binomial

↑ **Parent:** [Mellin transform](#mellin-transform)

For real $p>0$ and $0<s<p$, the displayed [improper integral](real-analysis.md#improper-integral) converges: its endpoint powers are $x^{s-1}$ near zero and $x^{s-p-1}$ near infinity. The [change of variables](multivariable-calculus.md#change-of-variables-formula) $t=x^p$ gives

$$
\frac1p\int_0^\infty\frac{t^{s/p-1}}{1+t}dt=\frac1pB(s/p,1-s/p)=\frac{\Gamma(s/p)\Gamma(1-s/p)}p=\frac\pi{p\sin(\pi s/p)}.
$$

Here the [beta function](complex-analysis.md#beta-function), the [beta-gamma identity](complex-analysis.md#beta-gamma-identity), and the [Gamma reflection formula](complex-analysis.md#gamma-reflection-formula) evaluate the integral. The same formula holds for complex $s$ in the [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) $0<\operatorname{Re}s<p$, by absolute convergence and analytic continuation within the strip. For integer $p$, a sector contour of angle $2\pi/p$ gives a direct [residue theorem](analysis.md#residue-theorem) proof, with a consistent branch of $z^{s-1}$.

### Mellin transform of an interval indicator

↑ **Parent:** [Mellin transform](#mellin-transform)

For $0<b<c<\infty$, the [indicator function](measure-theory.md#indicator-function) $f(x)=\mathbf1_{[b,c]}(x)$ has [Mellin transform](#mellin-transform)

$$
\mathcal Mf(s)=\begin{cases}(c^s-b^s)/s,&s\ne0,\\ \log(c/b),&s=0.\end{cases}
$$

The [interval](real-analysis.md#interval-mathematics) stays away from both zero and infinity, so the [integral](integral.md) is [absolutely convergent](sequence-and-series.md#absolute-convergence) for every [complex number](complex-analysis.md#complex-number) $s$. Its [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) is the whole [complex plane](complex-analysis.md#complex-plane). Evaluating the [antiderivative](integral.md#antiderivative) $x^s/s$ proves the formula for $s\ne0$; at $s=0$, integrating $1/x$ gives the real [natural logarithm](calculus.md#natural-logarithm) $\log(c/b)$. The apparent division by zero is a [removable singularity](isolated-singularity.md#removable-singularity), since $c^s-b^s=s(\log c-\log b)+O(s^2)$ by the [Taylor series](calculus.md#taylor-series) of the [exponential function](calculus.md#exponential-function). The transform is an [entire function](holomorphic-function.md#entire-function).

For example, $\mathbf1_{[1,4]}$ gives $(4^s-1)/s$ with value $\log4$ at zero. On $s=i\tau$, the [Mellin transform](#mellin-transform) sums oscillations over the width $\log4$ of the [interval](real-analysis.md#interval-mathematics) in [natural logarithm](calculus.md#natural-logarithm) coordinates; this is the same cancellation mechanism as in the [Fourier transform of an interval indicator](fourier-transform.md#fourier-transform-of-an-interval-indicator).

### Fundamental strip of a Mellin transform

↑ **Parent:** [Mellin transform](#mellin-transform)

The fundamental strip of a [Mellin transform](#mellin-transform) is the interior of the [set](set.md) of [real parts](complex-analysis.md#real-part) $\sigma$ for which

$$
\int_0^\infty x^{\sigma-1}|f(x)|\,dx<\infty.
$$

Viewed in the [complex plane](complex-analysis.md#complex-plane), it is a vertical strip $\alpha<\operatorname{Re}s<\beta$; either bound may be infinite, and the interior may be empty. Both endpoints of the [improper integral](real-analysis.md#improper-integral) must be checked. Convergence on a boundary line, whether [absolute convergence](sequence-and-series.md#absolute-convergence) or [conditional convergence](sequence-and-series.md#conditional-convergence), requires a separate test. The [Mellin transform](#mellin-transform) is [holomorphic](holomorphic-function.md) throughout a nonempty fundamental strip.[Chapter 2, §2.5(i), equation 2.5.1 and the following description of the vertical domain of analyticity](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

A practical sufficient test uses [Big O notation](real-analysis.md#big-o-notation): if $f(x)=O(x^p)$ near zero and $f(x)=O(x^{-q})$ near infinity, with real $p,q$, then comparison with elementary [improper integrals](real-analysis.md#improper-integral) gives

$$
\int_0^1x^{\sigma+p-1}\,dx<\infty\ \Longleftrightarrow\ \sigma>-p,\qquad
\int_1^\infty x^{\sigma-q-1}\,dx<\infty\ \Longleftrightarrow\ \sigma<q.
$$

Thus $-p<\sigma<q$ guarantees [absolute convergence](sequence-and-series.md#absolute-convergence). These upper bounds on $|f|$ need not locate the maximal [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform); faster actual decay can widen it. The strip property itself follows by bounding the weight at any intermediate $\sigma$ by the sum of two weights already known to be integrable. On a closed narrower strip, neighboring integrable weights also dominate the [natural logarithm](calculus.md#natural-logarithm) factors introduced by [differentiation under the integral sign](analysis.md#differentiation-under-the-integral-sign), making the transform a [holomorphic function](holomorphic-function.md).

An exact two-endpoint example is

$$
f(x)=\begin{cases}x^2,&0<x\leq1,\\x^{-3},&x>1,\end{cases}\qquad
\mathcal Mf(s)=\frac1{s+2}+\frac1{3-s},\qquad -2<\operatorname{Re}s<3.
$$

Here both bounds are sharp: at $\sigma=-2$ the zero-end [absolute convergence](sequence-and-series.md#absolute-convergence) test contains $\int_0^1dx/x$, and at $\sigma=3$ the infinity-end test contains $\int_1^\infty dx/x$. The displayed [rational function](isolated-singularity.md#rational-function) continues meromorphically outside the [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) and has [simple poles](isolated-singularity.md#simple-pole) at $-2$ and $3$. Its other finite continued values outside the strip are values of a [meromorphic continuation](holomorphic-function.md#meromorphic-continuation), not of a convergent defining [integral](integral.md). More general endpoint information leads to [meromorphic continuation of a Mellin transform from an asymptotic expansion](#meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion).

<a id="image-two-endpoint-conditions-define-the-mellin-fundamental-strip"></a>
![](mellin-fundamental-strip-and-integral-values.png)

**[Figure 1](#image-two-endpoint-conditions-define-the-mellin-fundamental-strip). Two endpoint conditions define the Mellin fundamental strip**. Left: the [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) for $x^2$ below one and $x^{-3}$ above one is $-2<\operatorname{Re}s<3$. Crosses mark the two [poles](isolated-singularity.md#pole) of the continued [rational function](isolated-singularity.md#rational-function), not whole lines of [isolated singularities](isolated-singularity.md). Right: the formula and independently computed [integrals](integral.md) agree on the real slice inside the strip. The curve is drawn only where the defining [integral](integral.md) converges.

### Scaling property of the Mellin transform

↑ **Parent:** [Mellin transform](#mellin-transform)

For $a>0$, let $g(x)=f(ax)$. Whenever the [Mellin transform](#mellin-transform) of $f$ is [absolutely convergent](sequence-and-series.md#absolute-convergence),

$$
\mathcal Mg(s)=a^{-s}\mathcal Mf(s),\qquad a^{-s}=\exp(-s\log a).
$$

The [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) is unchanged: the corresponding [integrals](integral.md) of [absolute values](real-analysis.md#absolute-value) differ by the finite positive factor $a^{-\sigma}$. The [change of variables](multivariable-calculus.md#change-of-variables-formula) $y=ax$ gives $x^{s-1}dx=a^{-s}y^{s-1}dy$, proving the rule. For $s=\sigma+i\tau$, the transform's [absolute value](real-analysis.md#absolute-value) changes by $a^{-\sigma}$, while the factor $e^{-i\tau\log a}$ changes its [phase](wave.md#phase-waves). On the line $\sigma=0$, wherever [absolute convergence](sequence-and-series.md#absolute-convergence) holds, the transform's [absolute value](real-analysis.md#absolute-value) is preserved.

For the [Mellin transform of an interval indicator](#mellin-transform-of-an-interval-indicator), replacing $\mathbf1_{[1,4]}(x)$ by $\mathbf1_{[1,4]}(2x)=\mathbf1_{[1/2,2]}(x)$ gives

$$
\frac{2^s-(1/2)^s}{s}=2^{-s}\frac{4^s-1}{s}.
$$

At the [removable singularity](isolated-singularity.md#removable-singularity) $s=0$, both sides have value $\log4$. Scaling leaves the width measured by the [natural logarithm](calculus.md#natural-logarithm) unchanged. Likewise, the [exponential function](calculus.md#exponential-function) $e^{-ax}$ has [Mellin transform](#mellin-transform) $a^{-s}\Gamma(s)$ on $\operatorname{Re}s>0$.

<a id="image-scaling-a-positive-variable-translates-its-logarithmic-coordinate"></a>
![](mellin-scaling-and-logarithmic-translation.png)

**[Figure 2](#image-scaling-a-positive-variable-translates-its-logarithmic-coordinate). Scaling a positive variable translates its logarithmic coordinate**. Left: $f(2x)$ moves the support [interval](real-analysis.md#interval-mathematics) $[1,4]$ to $[1/2,2]$. Right: $u=\log x$ turns the same change into a [translation](geometry-and-topology.md#translation-geometry) to the left by $\log2$; the [interval](real-analysis.md#interval-mathematics) width remains $\log4$. The [scaling property of the Mellin transform](#scaling-property-of-the-mellin-transform) multiplies the transform by $2^{-s}$.

### Mellin transform in logarithmic coordinates

↑ **Parent:** [Mellin transform](#mellin-transform)

The [change of variables](multivariable-calculus.md#change-of-variables-formula) $x=e^u$, using the [exponential function](calculus.md#exponential-function), turns the [Mellin transform](#mellin-transform) into

$$
\mathcal Mf(s)=\int_{-\infty}^\infty e^{su}f(e^u)\,du.
$$

The factor $dx=e^u du$ changes $x^{s-1}$ to $e^{su}$; missing this factor would shift every exponent by one. With $h_\sigma(u)=e^{\sigma u}f(e^u)$ and the [Fourier transform](fourier-transform.md) convention $\widehat h(\omega)=\int_{\mathbb R}h(u)e^{-i\omega u}\,du$, the identity is

$$
\mathcal Mf(\sigma+i\tau)=\int_{\mathbb R}h_\sigma(u)e^{i\tau u}\,du=\widehat h_\sigma(-\tau).
$$

Choosing $\sigma$ inside the [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform) makes $h_\sigma$ a [Lebesgue integrable function](measure-theory.md#lebesgue-integrable-function). The minus sign in the [Fourier transform](fourier-transform.md) argument follows from the stated convention. For the [Mellin transform of an interval indicator](#mellin-transform-of-an-interval-indicator) with $[b,c]=[1,4]$ and $\sigma=0$, $h_0=\mathbf1_{[0,\log4]}$: the [Fourier transform of an interval indicator](fourier-transform.md#fourier-transform-of-an-interval-indicator) is literally the same computation in a different coordinate.

Splitting the [real line](real-analysis.md#real-line) at $u=0$ also connects the [Mellin transform](#mellin-transform) to two unilateral [Laplace transforms](#laplace-transform). If $k_+(v)=f(e^v)$ and $k_-(v)=f(e^{-v})$ for $v\geq0$, then

$$
\mathcal Mf(s)=\mathcal Lk_+(-s)+\mathcal Lk_-(s)
$$

where both [integrals](integral.md) converge absolutely. Their [Laplace convergence regions](#region-of-absolute-convergence-of-a-laplace-transform) impose opposite endpoint conditions, explaining the two sides of the [Mellin fundamental strip](#fundamental-strip-of-a-mellin-transform). Finally, $f(ae^u)=f(e^{u+\log a})$ shows that a change of scale is a [translation](geometry-and-topology.md#translation-geometry) in $u$. Weighted [Fourier transforms](fourier-transform.md) of this [translation](geometry-and-topology.md#translation-geometry) give exactly the factor $a^{-s}$ in the [scaling property of the Mellin transform](#scaling-property-of-the-mellin-transform). For a smooth [function](function.md) with [compact support](function.md#compact-support) inside $(0,\infty)$, the [Mellin inversion theorem](#mellin-inversion-theorem) follows from [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem); the existing formula states the corresponding hypotheses.

### Imaginary-part regularization at a zero Mellin exponent

↑ **Parent:** [Mellin transform](#mellin-transform)

At exponent zero the complex [integral](integral.md) $\int_0 x^{-1}e^{-tx}/(ia+\log x)\,dx$ fails absolute and ordinary convergence through its real part, proportional to $dx/(x\log x)$. The imaginary-part kernel displayed above instead decays as $dx/(x\log^2x)$ and is integrable. Thus a positive-exponent family can have a well-defined imaginary-part boundary limit even when its full complex limit is invalid. Endpoint expansion coefficients need not be uniform in that limiting exponent: a sine zero can cancel a gamma-function pole and introduce a new nonzero constant term.

### Mellin transform of call prices

↑ **Parent:** [Mellin transform](#mellin-transform)

For $C(k)=\mathbb E(e^\xi-e^k)^+$ and $\operatorname{Re}z>1$ in the [exponential moment](probability-distribution.md#exponential-moment) domain, the [moment-generating function](probability-distribution.md#moment-generating-function) satisfies $\mathbb Ee^{z\xi}=\int_{\mathbb R}C(k)z(z-1)e^{(z-1)k}dk$.

### Meromorphic continuation of a Mellin transform from an asymptotic expansion

↑ **Parent:** [Mellin transform](#mellin-transform)

Suppose $f$ decays faster than every power at infinity and, near zero, $f(y)=\sum_{j=1}^r c_jy^{\sigma_j}+O(y^{\sigma_{r+1}})$ for every $r$, with $\sigma_j$ strictly increasing and tending to infinity. Subtracting finitely many terms in the integral over $(0,1)$ gives

$$
\mathcal Mf(s)=\int_1^\infty f(y)y^{s-1}\,dy+\sum_{j=1}^r\frac{c_j}{s+\sigma_j}+\int_0^1\left(f(y)-\sum_{j=1}^r c_jy^{\sigma_j}\right)y^{s-1}\,dy.
$$

The last integral is [holomorphic](holomorphic-function.md) on $\operatorname{Re}s>-\sigma_{r+1}$. These expressions continue the [Mellin transform](#mellin-transform) meromorphically to the whole plane, with simple poles precisely at $-\sigma_j$ for nonzero $c_j$.

#### Accumulating asymptotic exponents obstruct Mellin continuation

↑ **Parent:** [Meromorphic continuation of a Mellin transform from an asymptotic expansion](#meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion)

Strict increase alone does not suffice in the preceding theorem. Let $\sigma_j=1-1/j$, $c_j=2^{-j}$ and $f(y)=\eta(y)\sum_{j\geq1}2^{-j}y^{1-1/j}$, where $\eta$ is continuous, equals one on $(0,1]$ and vanishes on $[2,\infty)$. After division by the next power, every finite remainder extends continuously to zero. Nevertheless the [Mellin transform](#mellin-transform) has genuine poles at $-\sigma_j$ accumulating at $-1$, so it cannot be a [meromorphic function](isolated-singularity.md#meromorphic-function) on the whole plane.

### Mellin inversion theorem

↑ **Parent:** [Mellin transform](#mellin-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mellin_inversion_theorem)

Under standard decay and regularity hypotheses,

$$
f(x)=\frac1{2\pi i}\int_{\sigma-i\infty}^{\sigma+i\infty}
\mathcal Mf(s)x^{-s}\,ds.
$$

If $f$ is smooth and compactly supported in $(0,\infty)$, its Mellin transform is entire, decays faster than every power on vertical lines, and the formula holds for every real $\sigma$ and every $x>0$.

## Laplace transform

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_transform)

The unilateral [Laplace transform](#laplace-transform) of a [function](function.md) $f:[0,\infty)\to\mathbb C$ is the [integral transform](integral-transform.md)

$$
F(s)=\mathcal L\{f\}(s)=\int_0^\infty e^{-st}f(t)\,dt,\qquad s=\sigma+i\omega\in\mathbb C.
$$

Here $s$ is a [complex number](complex-analysis.md#complex-number), $\sigma$ is its [real part](complex-analysis.md#real-part), and $i$ is the [imaginary unit](complex-analysis.md#imaginary-unit). The [exponential function](calculus.md#exponential-function) factor $e^{-\sigma t}$ weights the history, while $e^{-i\omega t}$ probes its oscillations. The [integral](integral.md) starts at zero, so it uses only the history from that starting time onward. This section concerns ordinary [functions](function.md); their value at the single endpoint does not change the [integral](integral.md). See [MIT 18.03SC, definition and elementary examples](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/d40ad07a62996f6dad93b832f8de0e04_MIT18_03SCF11_s27_1text.pdf).

The [Laplace transform](#laplace-transform) is useful because it packages an entire time history into a [function](function.md) of $s$: a [derivative](calculus.md#derivative) becomes multiplication by $s$ together with the initial value, and a [convolution](fourier-analysis.md#convolution) becomes a product. Thus a [linear differential equation](differential-equation.md#linear-differential-equation) can become an algebraic equation that already remembers its [initial value problem](differential-equation.md#initial-value-problem). The worked example below shows both descriptions of the same response.

If $f$ is a [piecewise continuous function](analysis.md#piecewise-continuous-function) and has [exponential order](#exponential-order) $a$, then its defining [integral](integral.md) is [absolutely convergent](sequence-and-series.md#absolute-convergence) for $\operatorname{Re}s>a$. This is a sufficient condition; the actual [Laplace convergence region](#region-of-absolute-convergence-of-a-laplace-transform) may be larger than the bound obtained from a chosen $a$. [MIT 18.03SC, domain and growth conditions](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/fff4420903d82c5c5c483e54566bc5ec_MIT18_03SCF11_s27_2text.pdf).

<a id="image-exponential-function-weighting-controls-the-laplace-convergence-region"></a>
![](laplace-transform-exponential-weight.png)

**[Figure 3](#image-exponential-function-weighting-controls-the-laplace-convergence-region). Exponential function weighting controls the Laplace convergence region**. Left: for $f(t)=e^{-2t}$, the weighted [function](function.md) $e^{-\sigma t}f(t)$ decays when $\sigma>-2$, stays at one when $\sigma=-2$, and grows when $\sigma<-2$. Right: the real-parameter [Laplace transforms](#laplace-transform) of $1$ and $e^{-2t}$ grow without bound as $s$ approaches their respective convergence boundaries from the right. Curves are drawn only where the defining [integrals](integral.md) converge.

The bound has a short explanation. For sufficiently large $t$, $|f(t)|\leq Me^{at}$, so $|e^{-st}f(t)|\leq Me^{-(\sigma-a)t}$, whose tail [integral](integral.md) is finite for $\sigma>a$. The finite initial [interval](real-analysis.md#interval-mathematics) is covered by [piecewise continuity](analysis.md#piecewise-continuous-function).

Three calculations make the convergence condition concrete. For the input $f(t)=1$, evaluate the finite-history [integral](integral.md) first:

$$
\int_0^T e^{-st}\,dt=\frac{1-e^{-sT}}s\quad(s\ne0),\qquad \mathcal L\{1\}(s)=\frac1s\quad(\operatorname{Re}s>0).
$$

At $s=0$ the finite-history [integral](integral.md) is $T$. For the [exponential function](calculus.md#exponential-function) input $f(t)=e^{-2t}$, the same calculation replaces $s$ by $s+2$, giving

$$
\mathcal L\{e^{-2t}\}(s)=\frac1{s+2},\qquad \operatorname{Re}s>-2.
$$

In particular, $s=-1$ is allowed for this decaying input: its weighted [integral](integral.md) is $\int_0^\infty e^{-t}\,dt=1$. For the [sine](geometry-and-topology.md#sine) input, [Euler's formula](complex-analysis.md#euler-s-formula) gives $\sin t=(e^{it}-e^{-it})/(2i)$; [linearity](vector-space.md#linearity) then yields

$$
\mathcal L\{\sin t\}(s)=\frac1{2i}\left(\frac1{s-i}-\frac1{s+i}\right)=\frac1{s^2+1},\qquad \operatorname{Re}s>0.
$$

The [Laplace convergence region](#region-of-absolute-convergence-of-a-laplace-transform) is part of the answer. For example, $1/s$ has an [analytic continuation](holomorphic-function.md#analytic-continuation) to $s=-1$, but the defining [integral](integral.md) for the input $1$ diverges there. The [sine](geometry-and-topology.md#sine) calculation is also developed in [MIT 18.03SC, further elementary transforms](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/2343f70cc426b469402f731015ac9719_MIT18_03SCF11_s27_3text.pdf).

To see why the initial value appears, suppose $f$ is an [absolutely continuous function](sobolev-space.md#absolutely-continuous-function) on every finite [interval](real-analysis.md#interval-mathematics) $[0,T]$, with $f(0+)$ its right [one-sided limit](calculus.md#one-sided-limit). At the chosen $s$, assume $e^{-st}f(t)$ and $e^{-st}f'(t)$ are [Lebesgue integrable functions](measure-theory.md#lebesgue-integrable-function) and $e^{-sT}f(T)\to0$. The [Laplace transform of a derivative](#laplace-transform-of-a-derivative) is then

$$
\mathcal L\{f'\}(s)=sF(s)-f(0+).
$$

For example, [exponential order](#exponential-order) bounds on both $f$ and $f'$ guarantee these conditions whenever $\operatorname{Re}s$ exceeds both growth bounds. The initial value is the lower-end boundary contribution of [integration by parts](calculus.md#integration-by-parts).

Consider the [initial value problem](differential-equation.md#initial-value-problem)

$$
y'(t)+2y(t)=1,\qquad y(0)=0,\qquad t\geq0.
$$

Write $Y=\mathcal L\{y\}$. The [Laplace transform of a derivative](#laplace-transform-of-a-derivative) and [linearity](vector-space.md#linearity) give $sY-0+2Y=1/s$ for $\operatorname{Re}s>0$. A [partial fraction decomposition](isolated-singularity.md#partial-fraction-decomposition) therefore gives

$$
Y(s)=\frac1{s(s+2)}=\frac12\left(\frac1s-\frac1{s+2}\right),\qquad y(t)=\frac{1-e^{-2t}}2.
$$

We recognize the two elementary [Laplace transforms](#laplace-transform) already computed. Directly verify the result: its [derivative](calculus.md#derivative) is $y'(t)=e^{-2t}$, so

$$
y'(t)+2y(t)-1=e^{-2t}+1-e^{-2t}-1=0,\qquad y(0)=\frac{1-1}2=0.
$$

This verifies both the [ordinary differential equation](differential-equation.md#ordinary-differential-equation) and the initial value, and shows that the resulting bounded [function](function.md) has the [Laplace transform](#laplace-transform) used above. The response rises from zero toward $1/2$: at that value the input $1$ balances the term $2y$. The general method is described in [MIT 18.03SC, solving initial value problems](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/pages/unit-iii-fourier-series-and-laplace-transform/laplace-transform-solving-initial-value-problems/).

<a id="image-a-heaviside-step-function-input-produces-a-response-equal-to-the-accumulated-convolution-kernel"></a>
![](laplace-transform-step-response.png)

**[Figure 4](#image-a-heaviside-step-function-input-produces-a-response-equal-to-the-accumulated-convolution-kernel). A Heaviside step function input produces a response equal to the accumulated convolution kernel**. Left: the solution $y(t)=(1-e^{-2t})/2$ and the [convolution kernel](fourier-analysis.md#convolution-kernel) $h(t)=e^{-2t}$ for $t\geq0$. Right: at $t=1$, the shaded [integral](integral.md) $\int_0^1e^{-2(1-\tau)}\,d\tau=(1-e^{-2})/2\approx0.4323$ includes only the available history $0\leq\tau\leq1$. The rising profile on the right is $h(1-\tau)$; recent inputs have had less time to decay.

The same solution is a [convolution](fourier-analysis.md#convolution). For [functions](function.md) defined on $[0,\infty)$, the unilateral [convolution](fourier-analysis.md#convolution) is

$$
(f*g)(t)=\int_0^t f(\tau)g(t-\tau)\,d\tau,\qquad t\geq0.
$$

The main [convolution](fourier-analysis.md#convolution) article integrates over the whole [real line](real-analysis.md#real-line); applying a [causal extension by zero](#causal-extension-by-zero) to both [functions](function.md) makes its formula identical to this one. Nonzero contributions require both $\tau\geq0$ and $t-\tau\geq0$, hence $0\leq\tau\leq t$. If $e^{-\sigma t}f(t)$ and $e^{-\sigma t}g(t)$ are [Lebesgue integrable functions](measure-theory.md#lebesgue-integrable-function) on $[0,\infty)$, the [convolution theorem for Laplace transforms](#convolution-theorem-for-laplace-transforms) states

$$
\mathcal L\{f*g\}(s)=F(s)G(s),\qquad \operatorname{Re}s=\sigma.
$$

For [piecewise continuous functions](analysis.md#piecewise-continuous-function) of [exponential order](#exponential-order) $a$ and $b$, it holds throughout $\operatorname{Re}s>\max(a,b)$. The weighted absolute double [integral](integral.md) factors into the two finite weighted absolute [integrals](integral.md); [Fubini's theorem](measure-theory.md#fubini-s-theorem) therefore permits exchanging the order, and setting $u=t-\tau$ separates the product. [MIT 18.03SC, convolution and system response](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/0d4d90053f2bb24f7551c78e2d1b21a2_MIT18_03SCF11_s30_5text.pdf).

For the [linear time-invariant system](electrical-engineering.md#linear-time-invariant-system) $y'+2y=f$ starting at zero, the [convolution kernel](fourier-analysis.md#convolution-kernel) is its [impulse response](green-s-function.md#impulse-response) $h(t)=e^{-2t}$ for $t\geq0$, extended by zero for $t<0$. With the [Heaviside step function](#heaviside-step-function) input, $f(t)=1$ for $t\geq0$, the accumulated response is

$$
y(t)=(h*f)(t)=\int_0^t e^{-2(t-\tau)}\,d\tau=\frac{1-e^{-2t}}2.
$$

Thus $Y(s)=(1/(s+2))(1/s)$ on $\operatorname{Re}s>0$ is both the algebraic solution and the [Laplace transform](#laplace-transform) of a finite-history [convolution](fourier-analysis.md#convolution). Each past input contributes an [exponential function](calculus.md#exponential-function) that decays with its age $t-\tau$, which makes the two descriptions easy to connect.

Finally, compare the [Fourier transform](fourier-transform.md) convention $\widehat g(\omega)=\int_{\mathbb R}g(t)e^{-i\omega t}\,dt$. If $f_0$ is the [causal extension by zero](#causal-extension-by-zero) of $f$, define $g_\sigma(t)=e^{-\sigma t}f_0(t)$. Whenever $g_\sigma$ is a [Lebesgue integrable function](measure-theory.md#lebesgue-integrable-function),

$$
F(\sigma+i\omega)=\widehat{g_\sigma}(\omega).
$$

A vertical slice of the [Laplace transform](#laplace-transform) is therefore the [Fourier transform](fourier-transform.md) of the zero-extended, weighted input. Positive $\sigma$ damps its positive-time history. A finite [window function](fourier-transform.md#window-function) instead gives $g_{\sigma,T}(t)=e^{-\sigma t}f_0(t)\mathbf1_{[0,T]}(t)$ and $\widehat{g_{\sigma,T}}(\omega)=\int_0^Te^{-(\sigma+i\omega)t}f(t)\,dt$; this approaches $F(\sigma+i\omega)$ in the [Laplace convergence region](#region-of-absolute-convergence-of-a-laplace-transform). Setting $\sigma=0$ directly requires an integrable zero-extended input: the input $1$ fails that condition, even though its [Laplace transform](#laplace-transform) exists for every $\sigma>0$.

The history of the [Laplace transform](#laplace-transform) spans several stages. Schiff's historical summary notes that Laplace's 1812 treatise acknowledged earlier work on [integral transforms](integral-transform.md) and describes later development of the modern [Laplace transform](#laplace-transform) method. [Schiff, The Laplace Transform: Theory and Applications, historical summary, pp. x–xi](https://oldversion.stu.edu.vn/uploads/documents/170509-091205.pdf#page=9).

### Exponential order

↑ **Parent:** [Laplace transform](#laplace-transform)

A [function](function.md) has exponential order $a\in\mathbb R$ if some $M>0$ and $T\geq0$ give the displayed bound. Bounded [functions](function.md), including [sine](geometry-and-topology.md#sine), have exponential order zero; $e^{-2t}$ has exponential order $-2$. The bound need not use the smallest possible $a$. Together with [piecewise continuity](analysis.md#piecewise-continuous-function), it guarantees a [Laplace transform](#laplace-transform) for $\operatorname{Re}s>a$.

### Region of absolute convergence of a Laplace transform

↑ **Parent:** [Laplace transform](#laplace-transform)

The [set](set.md) of [complex numbers](complex-analysis.md#complex-number) $s$ for which the displayed [integral](integral.md) is finite is the region of absolute convergence of a [Laplace transform](#laplace-transform). It depends only on the [real part](complex-analysis.md#real-part) $\sigma=\operatorname{Re}s$. Once the condition holds for one $\sigma$, it holds for every larger [real part](complex-analysis.md#real-part). For the [exponential function](calculus.md#exponential-function) $e^{-2t}$ it is exactly $\operatorname{Re}s>-2$; in general, convergence on the boundary must be checked separately. An [analytic continuation](holomorphic-function.md#analytic-continuation) outside this [set](set.md) need not equal a convergent defining [integral](integral.md).

### Causal extension by zero

↑ **Parent:** [Laplace transform](#laplace-transform)

Extend a [function](function.md) given for nonnegative time to the [real line](real-analysis.md#real-line) by setting it to zero before the starting time. This turns unilateral [convolution](fourier-analysis.md#convolution) into whole-line [convolution](fourier-analysis.md#convolution) and identifies a [Laplace transform](#laplace-transform) slice with a [Fourier transform](fourier-transform.md) after [exponential function](calculus.md#exponential-function) weighting.

<h3 id="ramanujan-s-function">Ramanujan's function</h3>

↑ **Parent:** [Laplace transform](#laplace-transform)

For $t>0$, this [Laplace transform](#laplace-transform) converges at zero because $dx/[x\log^2x]$ is integrable, and at infinity because of exponential damping. Its large-$t$ behavior is governed by a logarithmic zero-endpoint singularity and begins with $1/\log t$, rather than a power of $t$.

<h4 id="logarithmic-expansion-of-ramanujan-s-function">Logarithmic expansion of Ramanujan's function</h4>

↑ **Parent:** [Ramanujan's function](#ramanujan-s-function)

The [Gamma reflection formula](complex-analysis.md#gamma-reflection-formula) gives $(\sin\pi z/\pi)\Gamma(z)=1/\Gamma(1-z)$, analytic at zero with value one. A finite-parameter [Watson's lemma](analysis.md#watson-s-lemma) representation of [Ramanujan's function](#ramanujan-s-function) therefore gives the displayed coefficients. In particular $c_0=1$, $c_1=-\gamma$ and $c_2=\gamma^2-\pi^2/6$, with $\gamma$ [Euler's constant](complex-analysis.md#euler-s-constant). Obtaining this representation requires taking an imaginary part before sending its Mellin exponent to zero; the original complex [integral](integral.md) is divergent at that boundary.

### Newman Tauberian theorem

↑ **Parent:** [Laplace transform](#laplace-transform)

For bounded locally integrable $f$ on the nonnegative real line, suppose its [Laplace transform](#laplace-transform) $F$ extends holomorphically to an open neighborhood of the closed right half-plane. Then the ordinary improper integral converges to $F(0)$. [Contour damping for bounded Laplace transforms](#contour-damping-for-bounded-laplace-transforms) bounds the difference from the finite-interval transform by $2\|f\|_\infty/R$ in the limit for every radius $R$. Extension merely to the open right half-plane is insufficient, as the constant function and transform $1/z$ show.

#### Contour damping for bounded Laplace transforms

↑ **Parent:** [Newman Tauberian theorem](#newman-tauberian-theorem)

The displayed kernel has residue one at zero and vanishes at the endpoints of a radius-$R$ imaginary-axis segment. On either radius-$R$ semicircle, $|1+z^2/R^2|=2|\operatorname{Re}z|/R$, cancelling the inverse real-part bound on a bounded function's [Laplace transform](#laplace-transform) tail. Use the full transform only on a right semicircle and a thin analytic leftward path; deform the finite-interval entire transform to the large left semicircle. This proves the [Newman Tauberian theorem](#newman-tauberian-theorem) without assuming analytic continuation across an entire left half-disk.

### Convolution theorem for Laplace transforms

↑ **Parent:** [Laplace transform](#laplace-transform)

For [functions](function.md) $f,g$ on $[0,\infty)$ with $e^{-\sigma t}f(t)$ and $e^{-\sigma t}g(t)$ [Lebesgue integrable functions](measure-theory.md#lebesgue-integrable-function), their unilateral [convolution](fourier-analysis.md#convolution), defined [almost everywhere](measure-theory.md#almost-everywhere) if necessary, satisfies

$$
\mathcal L\{f*g\}(s)=F(s)G(s),\qquad (f*g)(t)=\int_0^tf(\tau)g(t-\tau)\,d\tau,\qquad \operatorname{Re}s=\sigma.
$$

Taking a [causal extension by zero](#causal-extension-by-zero) of both [functions](function.md) gives the existing whole-line [convolution](fourier-analysis.md#convolution) definition. [Absolute convergence](sequence-and-series.md#absolute-convergence) and [Fubini's theorem](measure-theory.md#fubini-s-theorem) justify the product rule: put $t=\tau+u$ in the double [integral](integral.md), so $e^{-st}=e^{-s\tau}e^{-su}$. For [piecewise continuous functions](analysis.md#piecewise-continuous-function) of [exponential order](#exponential-order) $a$ and $b$, the hypotheses hold for $\operatorname{Re}s>\max(a,b)$. The [Laplace transform](#laplace-transform) article works out the concrete example $h(t)=e^{-2t}$ and the [Heaviside step function](#heaviside-step-function) input, whose output is $(1-e^{-2t})/2$. [MIT 18.03SC, convolution and system response](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/0d4d90053f2bb24f7551c78e2d1b21a2_MIT18_03SCF11_s30_5text.pdf).

### Bromwich inversion formula

↑ **Parent:** [Laplace transform](#laplace-transform)

Under suitable regularity and growth conditions, a function with [Laplace transform](#laplace-transform) $F$ is recovered by the inverse contour integral

$$
f(t)=\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}e^{st}F(s)\,ds,
$$

where the vertical line lies to the right of every singularity of $F$.

#### Causality in finite-time Laplace contour inversion

↑ **Parent:** [Bromwich inversion formula](#bromwich-inversion-formula)

A [Laplace transform](#laplace-transform) $G_T(p)=\int_0^Te^{-ps}g(s)ds$ can grow exponentially as $\operatorname{Re}p\to-\infty$. At an evaluation time $t<T$, multiplying by $e^{pt}$ does not automatically permit closing the inverse contour to the left. Either retain the growth-bearing contour pieces, use a causal time convolution, or justify a deformation with the time-truncated transform. Resolvent-pole information alone is insufficient.

### Long-time asymptotics from a Laplace transform

↑ **Parent:** [Laplace transform](#laplace-transform)

Terms singular at $s=0$ in a [Laplace transform](#laplace-transform) encode persistent late-time behaviour. In particular,

$$
F(s)=\frac{A}{s^2}+\frac{B}{s}+O(1)
$$

contributes $At+B$ to the inverse transform; singularities farther into the left half-plane contribute decaying terms under the usual analyticity and growth assumptions.

### Laplace transform of a derivative

↑ **Parent:** [Laplace transform](#laplace-transform)

Suppose $f$ is an [absolutely continuous function](sobolev-space.md#absolutely-continuous-function) on every finite [interval](real-analysis.md#interval-mathematics) $[0,T]$, both $e^{-st}f(t)$ and $e^{-st}f'(t)$ are [Lebesgue integrable functions](measure-theory.md#lebesgue-integrable-function), and $e^{-sT}f(T)\to0$. Then [integration by parts](calculus.md#integration-by-parts) on $[0,T]$ followed by a [limit](calculus.md#limit-of-a-function) gives

$$
\int_0^T e^{-st}f'(t)\,dt=e^{-sT}f(T)-f(0+)+s\int_0^Te^{-st}f(t)\,dt,\qquad \mathcal L\{f'\}(s)=sF(s)-f(0+).
$$

Here $f(0+)$ is the right [one-sided limit](calculus.md#one-sided-limit). [Exponential order](#exponential-order) bounds on $f$ and $f'$ suffice when $\operatorname{Re}s$ exceeds both bounds. For $f(t)=e^{-2t}$, the identity reads $-2/(s+2)=s/(s+2)-1$ on $\operatorname{Re}s>-2$. This is the ordinary [derivative](calculus.md#derivative) on nonnegative time; differentiating a [causal extension by zero](#causal-extension-by-zero) at its jump instead introduces a [Dirac delta function](distribution-theory.md#dirac-delta-function). [MIT 18.03SC, derivative rules and initial data](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/22aba4126352ce0f76930d858d8dffa5_MIT18_03SCF11_s29_1text.pdf).

### Laplace transform shift theorem

↑ **Parent:** [Laplace transform](#laplace-transform)

For $a\geq0$, $\mathcal L\{f(t-a)H(t-a)\}(s)=e^{-as}\mathcal L\{f\}(s)$.

#### Laplace transform time-shift rule

↑ **Parent:** [Laplace transform shift theorem](#laplace-transform-shift-theorem)

The delayed unit step has

$$
\mathcal L\{H(t-t_0)\}(s)=\frac{e^{-st_0}}s,
\qquad \operatorname{Re}s>0.
$$

#### Heaviside step function

↑ **Parent:** [Laplace transform shift theorem](#laplace-transform-shift-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heaviside_step_function)

The Heaviside function is zero before its switching time and one after it, allowing delayed signals to be written algebraically.

### Laplace transform of a periodic function

↑ **Parent:** [Laplace transform](#laplace-transform)

If $g$ has period $T$, then

$$
\mathcal L\{g\}(s)=\frac{\int_0^T e^{-st}g(t)dt}{1-e^{-sT}}.
$$

### Matrix-valued Laplace transform

↑ **Parent:** [Laplace transform](#laplace-transform)

The Laplace transform of a matrix-valued function is obtained by transforming each entry. A constant matrix may be taken outside on the corresponding side of the integral; in particular, $\mathcal L\{AB\}=A\mathcal L\{B\}$ when $A$ is constant.

#### Laplace-transform solution of a constant-coefficient vector ODE

↑ **Parent:** [Matrix-valued Laplace transform](#matrix-valued-laplace-transform)

For

$$
y'=Ay+g,qquad y(0)=y_0,
$$

the derivative rule gives

$$
(sI-A)Y(s)=y_0+G(s),
$$

and hence $Y(s)=(sI-A)^{-1}(y_0+G(s))$ wherever the transforms converge and $sI-A$ is invertible.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (6)

- [Laplace transform](#laplace-transform)
- [Mellin transform](#mellin-transform)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328.md#1/ii/solution)
