# Asymptotic expansion

↑ **Parent:** [Analysis](analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_expansion)

An [asymptotic expansion](asymptotic-expansion-split.md) describes a [function](function-split.md) near a specified [limit](limit-of-a-function.md) by successively smaller scales. Each fixed finite truncation has a remainder smaller than its last retained scale. The central question is how the approximation improves as the parameter approaches the [limit](limit-of-a-function.md); convergence of the entire infinite [series](series-mathematics.md) at a fixed parameter is a separate question. For the inverse-power scale $1,z^{-1},z^{-2},\ldots$,

$$
f(z)\sim\sum_{k=0}^{\infty}a_kz^{-k}\quad(z\to+\infty)
$$

means that, for every fixed [nonnegative integer](natural-number.md) $m$,

$$
f(z)-\sum_{k=0}^ma_kz^{-k}=o(z^{-m}).
$$

The [little o notation](little-o-notation.md) makes the accuracy requirement precise. With expansions to all orders, this is also equivalent to an $O(z^{-m-1})$ remainder after the $m$th term; the implied bound may depend on $m$.[NIST Digital Library of Mathematical Functions, §2.1(iii), equations 2.1.13–2.1.15: fixed-order inverse-power expansions](nist-digital-library-of-mathematical-functions/2-1-definitions-and-elementary-properties.md)

For a quick convergent example, the finite [geometric series](geometric-series.md) identity gives

$$
\frac1{1+z^{-1}}
=1-\frac1z+\frac1{z^2}-\cdots+\frac{(-1)^m}{z^m}
+\frac{(-1)^{m+1}z^{-m-1}}{1+z^{-1}}.
$$

For $z>1$, both the [asymptotic expansion](asymptotic-expansion-split.md) as $z\to+\infty$ and the ordinary convergent [geometric series](geometric-series.md) describe this [function](function-split.md). The exact remainder displays the required extra inverse power.

The more surprising example under [a divergent factorial series can approximate a convergent integral](a-divergent-factorial-series-can-approximate-a-convergent-integral.md) has a convergent [integral](integral-split.md) but a divergent [series](series-mathematics.md) at every fixed positive $z$:

$$
F(z)=\int_0^\infty\frac{e^{-t}}{1+t/z}\,dt
\sim1-\frac1z+\frac{2!}{z^2}-\frac{3!}{z^3}+\cdots.
$$

A few terms can estimate $F(10)$ well, even though adding sufficiently many terms eventually destroys the approximation. [Optimal truncation](optimal-truncation.md) explains where to stop.

This makes [asymptotic expansions](asymptotic-expansion-split.md) useful when an exact expression is a complicated [integral](integral-split.md) or [differential equation](differential-equation-split.md) solution, but a parameter is very large or very small. The leading term reveals the scale; corrections reveal which effects matter next. The [asymptotic sequence](asymptotic-sequence.md) must be specified: integer powers, fractional powers, [logarithms](logarithm.md), and [exponential functions](exponential-function.md) can encode different kinds of behavior. A good finite approximation includes a remainder estimate or an independently checked range of use.

**Table of contents**

- [Uniform asymptotic approximation](uniform-asymptotic-approximation.md)
- [Lorentzian peak approaching an integration endpoint](lorentzian-peak-approaching-an-integration-endpoint.md)
- [Asymptotic power series](asymptotic-power-series.md)
  - [A divergent factorial series can approximate a convergent integral](a-divergent-factorial-series-can-approximate-a-convergent-integral.md)
- [Compactified approximation from endpoint asymptotics](compactified-approximation-from-endpoint-asymptotics.md)
- [Perturbation theory](perturbation-theory.md)
  - [Perturbation](perturbation.md)
- [Integer-frequency endpoint expansion of cosine integrals](integer-frequency-endpoint-expansion-of-cosine-integrals.md)
- [Dominant balance](dominant-balance.md)
- [Regular perturbation](regular-perturbation.md)
- [Large roots near tangent poles](large-roots-near-tangent-poles.md)
- [Uniform error bound for nearby decaying exponentials](uniform-error-bound-for-nearby-decaying-exponentials.md)
- [Borel summation](borel-summation.md)
  - [Borel transform of a factorially divergent series](borel-transform-of-a-factorially-divergent-series.md)
  - [Borel integral with a simple pole](borel-integral-with-a-simple-pole.md)
- [Optimal truncation](optimal-truncation.md)
- [Dominant balance for algebraic roots](dominant-balance-for-algebraic-roots.md)
  - [Divergent algebraic root in a singular perturbation](divergent-algebraic-root-in-a-singular-perturbation.md)
  - [Regular perturbation of a simple algebraic root](regular-perturbation-of-a-simple-algebraic-root.md)
- [Endpoint transition of a regularized interior pole](endpoint-transition-of-a-regularized-interior-pole.md)
  - [Lorentzian contribution from shrinking regularization](lorentzian-contribution-from-shrinking-regularization.md)
- [Stokes phenomenon](stokes-phenomenon.md)
  - [Sectorial fundamental solution](sectorial-fundamental-solution.md)
  - [Stokes matrix](stokes-matrix.md)
  - [Cubic exponential integral Stokes sectors](cubic-exponential-integral-stokes-sectors.md)
    - [Borel remainder for a cubic exponential integral](borel-remainder-for-a-cubic-exponential-integral.md)
  - [Gaussian Cauchy transform and its Stokes jump](gaussian-cauchy-transform-and-its-stokes-jump.md)
  - [Gaussian saddle coalescing with a simple pole](gaussian-saddle-coalescing-with-a-simple-pole.md)
    - [Error-function smoothing of a Stokes multiplier](error-function-smoothing-of-a-stokes-multiplier.md)
      - [Gaussian pole transition for a large gamma parameter](gaussian-pole-transition-for-a-large-gamma-parameter.md)
  - [anti-Stokes line](anti-stokes-line.md)
  - [Stokes line](stokes-line.md)
- [Series reversion](series-reversion.md)
  - [Cubic series reversion](cubic-series-reversion.md)
- [Divide-and-conquer asymptotic expansion](divide-and-conquer-asymptotic-expansion.md)
- [Asymptotic sequence](asymptotic-sequence.md)
  - [Harmonic-mean refinement of an asymptotic sequence](harmonic-mean-refinement-of-an-asymptotic-sequence.md)
  - [Geometric-mean refinement of an asymptotic sequence](geometric-mean-refinement-of-an-asymptotic-sequence.md)
  - [Termwise equivalent asymptotic scales need not preserve expansions](termwise-equivalent-asymptotic-scales-need-not-preserve-expansions.md)
- [Laplace's method](laplace-s-method.md)
  - [Mixed cubic and quadratic Laplace endpoints](mixed-cubic-and-quadratic-laplace-endpoints.md)
  - [Laplace approximation](laplace-approximation.md)
  - [Localization condition for Laplace's method](localization-condition-for-laplace-s-method.md)
  - [Two-term monotone-endpoint Laplace expansion](two-term-monotone-endpoint-laplace-expansion.md)
  - [Endpoint asymptotics after odd Gaussian cancellation](endpoint-asymptotics-after-odd-gaussian-cancellation.md)
  - [Laplace endpoint estimate](laplace-endpoint-estimate.md)
  - [Laplace integral](laplace-integral.md)
    - [Laplace integral solution](laplace-integral-solution.md)
  - [Laplace's method at a nondegenerate stationary endpoint](laplace-s-method-at-a-nondegenerate-stationary-endpoint.md)
  - [Laplace's method with multiple global maxima](laplace-s-method-with-multiple-global-maxima.md)
  - [Degenerate endpoint in Laplace's method](degenerate-endpoint-in-laplace-s-method.md)
    - [Cubic endpoint-to-saddle transition](cubic-endpoint-to-saddle-transition.md)
  - [Discrete Laplace method](discrete-laplace-method.md)
  - [Laplace asymptotic for the derivative of the Gamma function](laplace-asymptotic-for-the-derivative-of-the-gamma-function.md)
- [Method of steepest descent](method-of-steepest-descent.md)
  - [Steepest descent contour](steepest-descent-contour.md)
  - [Quadratic complex endpoint descent path](quadratic-complex-endpoint-descent-path.md)
    - [Gaussian saddle and endpoint dominance by angle](gaussian-saddle-and-endpoint-dominance-by-angle.md)
  - [Simple-saddle contribution in steepest descent](simple-saddle-contribution-in-steepest-descent.md)
  - [Endpoint contribution in steepest descent](endpoint-contribution-in-steepest-descent.md)
    - [Endpoint at infinity](endpoint-at-infinity.md)

## ↑ Ancestors (4)

1. [Analysis](analysis-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (87)

- [A divergent factorial series can approximate a convergent integral](a-divergent-factorial-series-can-approximate-a-convergent-integral.md)
- [Asymptotic expansion](asymptotic-expansion-split.md)
- [Asymptotic power series](asymptotic-power-series.md)
- [Bessel inverse-power expansion at infinity](bessel-inverse-power-expansion-at-infinity.md)
- [Compactified approximation from endpoint asymptotics](compactified-approximation-from-endpoint-asymptotics.md)
- [Complementary error function](complementary-error-function.md)
- [Cubic exponential integral Stokes sectors](cubic-exponential-integral-stokes-sectors.md)
- [Dawson function](dawson-function.md)
- [Derivative of the gamma function](derivative-of-the-gamma-function.md)
- [Divisor summatory asymptotic](divisor-summatory-asymptotic.md)
- [Finite Fresnel integrals](finite-fresnel-integrals.md)
- [Fourier decay from a Green-function derivative jump](fourier-decay-from-a-green-function-derivative-jump.md)
- [Fresnel tail expansion](fresnel-tail-expansion.md)
- [Hankel function](hankel-function.md)
- [Laplacian as departure from a local average](laplacian-as-departure-from-a-local-average.md)
- [Large-argument asymptotic expansion of a modified Bessel function](large-argument-asymptotic-expansion-of-a-modified-bessel-function.md)
- [Logarithmic endpoint Fourier asymptotics](logarithmic-endpoint-fourier-asymptotics.md)
- [Logarithmic energy gain from a Peierls distortion](logarithmic-energy-gain-from-a-peierls-distortion.md)
- [Matched expansion with square-root and logarithmic corrections](matched-expansion-with-square-root-and-logarithmic-corrections.md)
- [Opaque barrier approximation](opaque-barrier-approximation.md)
- [Optimal truncation](optimal-truncation.md)
- [Outer expansion](outer-expansion.md)
- [Overlap region](overlap-region.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2a/section-a/16/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-50/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-48/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-79/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-79/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/30a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-48/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-81/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-68/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-68/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-68/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/27c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-72/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/29e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/30e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-336/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-336/2/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/31b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/30a/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/30a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/3g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/30a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-336/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/31e/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-320/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/16d/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-336/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-314/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-332/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/15/d/solution.md)
- [Perturbation theory](perturbation-theory.md)
- [Principal-value Fourier transform of a real pole](principal-value-fourier-transform-of-a-real-pole.md)
- [Regular perturbation](regular-perturbation.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Singular perturbation](singular-perturbation-split.md)
- [Slip-enhanced swimming speed of a transverse sheet](slip-enhanced-swimming-speed-of-a-transverse-sheet.md)
- [Stokes matrix](stokes-matrix.md)
- [Stokes phenomenon](stokes-phenomenon.md)
- [Strong-field steady magnetoconvection varying along the field](strong-field-steady-magnetoconvection-varying-along-the-field.md)
- [Two-loop inverse-coupling logarithmic remainder](two-loop-inverse-coupling-logarithmic-remainder.md)
- [Zero-dimensional quartic perturbation series](zero-dimensional-quartic-perturbation-series.md)
