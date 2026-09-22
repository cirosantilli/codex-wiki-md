# Harmonic analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_analysis)

Harmonic analysis decomposes functions into elementary oscillations, generalizing [Fourier series](fourier-series.md) and the [Fourier transform](fourier-transform.md). On a locally compact Abelian group the elementary oscillations are [continuous unitary characters](topological-group.md#continuous-unitary-character), and [Haar measure](measure.md#haar-measure) supplies translation-invariant integration.

**Table of contents**

- [Carleson measure](#carleson-measure)
  - [Carleson embedding theorem on the disk](#carleson-embedding-theorem-on-the-disk)
  - [Carleson box](#carleson-box)
- [Non-tangential maximal function](#non-tangential-maximal-function)
  - [Poisson maximal function is dominated by the Hardy-Littlewood maximal function](#poisson-maximal-function-is-dominated-by-the-hardy-littlewood-maximal-function)
- [Hardy space](#hardy-space)
  - [H1 space on the unit disk](#h1-space-on-the-unit-disk)
    - [H1 non-tangential maximal inequality on the disk](#h1-non-tangential-maximal-inequality-on-the-disk)
    - [Normalized squared Cauchy kernel](#normalized-squared-cauchy-kernel)
  - [H-infinity space](#h-infinity-space)
    - [Fatou theorem for bounded holomorphic functions](#fatou-theorem-for-bounded-holomorphic-functions)
  - [F. and M. Riesz theorem](#f-and-m-riesz-theorem)
- [Calderón–Zygmund decomposition](#calderon-zygmund-decomposition)
- [Positive-definite function](#positive-definite-function)
  - [Cyclic unitary representation of a positive-definite function](#cyclic-unitary-representation-of-a-positive-definite-function)
  - [Bochner's theorem](#bochner-s-theorem)
    - [Bochner–Herglotz theorem](#bochner-herglotz-theorem)
      - [Wiener Fourier coefficient lemma](#wiener-fourier-coefficient-lemma)
    - [Bochner consistency identity for convolution squares](#bochner-consistency-identity-for-convolution-squares)

## Carleson measure

↑ **Parent:** [Harmonic analysis](harmonic-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carleson_measure)

A positive [Borel measure](measure.md#borel-measure) near a domain boundary is a Carleson measure when its mass in boundary neighborhoods is bounded by a constant times their boundary measure. On the [unit disc](topology.md#unit-disc), this becomes the displayed bound for every [Carleson box](#carleson-box). The equivalent [hyperbolic geodesic cap](hyperbolic-geometry.md#hyperbolic-geodesic-cap) version follows from the [geodesic-cap and Carleson-box comparison](hyperbolic-geometry.md#geodesic-cap-and-carleson-box-comparison). The [Carleson embedding theorem on the disk](#carleson-embedding-theorem-on-the-disk) explains why this geometric growth condition controls integration of analytic [Hardy spaces](#hardy-space).

### Carleson embedding theorem on the disk

↑ **Parent:** [Carleson measure](#carleson-measure)

A positive [Borel measure](measure.md#borel-measure) on the [unit disc](topology.md#unit-disc) satisfies $\int|f|\,d\mu\le N\|f\|_1$ for every [H1 space on the unit disk](#h1-space-on-the-unit-disk) function exactly when it is a [Carleson measure](#carleson-measure), with comparable optimal constants. The [normalized squared Cauchy kernel](#normalized-squared-cauchy-kernel) tests necessity. For sufficiency, the boundary shadow of every point with $|f(z)|>t$ lies inside a component arc of $\{Nf>t\}$. The [geodesic-cap and Carleson-box comparison](hyperbolic-geometry.md#geodesic-cap-and-carleson-box-comparison) bounds the measure of each shadow region by its component length, giving $\mu\{|f|>t\}\le C\|\mu\|_{\rm Carl}m\{Nf>t\}$. The [layer cake representation](metric-embedding.md#layer-cake-representation) and [H1 non-tangential maximal inequality on the disk](#h1-non-tangential-maximal-inequality-on-the-disk) give the embedding. The broader kernel and covering mechanism is discussed in [Terence Tao's harmonic-analysis notes, Exercise 2 after Lemma 4.1](https://www.math.ucla.edu/~tao/247b.1.07w/notes6.pdf); the analytic endpoint here uses the fractional-power argument just given.

### Carleson box

↑ **Parent:** [Carleson measure](#carleson-measure)

A boundary neighborhood over an arc $I$ of the [unit circle](complex-analysis.md#complex-unit-circle), with radial depth equal to its normalized angular length $m(I)$. Changing that depth by any fixed positive factor gives an equivalent [Carleson measure](#carleson-measure) condition. Large arcs and central mass can be handled separately by finitely many fixed neighborhoods covering the [unit disc](topology.md#unit-disc).

## Non-tangential maximal function

↑ **Parent:** [Harmonic analysis](harmonic-analysis.md)

This supremum function takes a supremum over a cone approaching the boundary point $x$; the positive number $a$ is its aperture. For an analytic upper-half-plane $H^1$ function, it belongs to $L^1$. To prove this without first assuming boundary absolute continuity, shift the function upwards, apply subharmonic Poisson comparison to its square root, and use the strong $L^2$ bound for the [Hardy-Littlewood maximal function](analysis.md#hardy-littlewood-maximal-function). [Fatou lemma](measure-theory.md#fatou-s-lemma) removes the shift.

### Poisson maximal function is dominated by the Hardy-Littlewood maximal function

↑ **Parent:** [Non-tangential maximal function](#non-tangential-maximal-function)

For integrable boundary data $g$ on the [unit circle](complex-analysis.md#complex-unit-circle), this follows from the [Poisson kernel](partial-differential-equation.md#poisson-kernel) bound $C_A\delta/(\delta^2+d^2)$ in a fixed [Stolz region](complex-analysis.md#stolz-region). The arc of radius $\delta$ and successive dyadic annuli contribute at most $C_A2^{-k}Mg(\xi)$, which sum to the displayed estimate. This links harmonic extension to the [Hardy-Littlewood maximal function](analysis.md#hardy-littlewood-maximal-function) and its strong $L^p$ bounds for $p>1$.

## Hardy space

↑ **Parent:** [Harmonic analysis](harmonic-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hardy_space)

For $0<p<∞$, an analytic [Hardy space](#hardy-space) controls the integral means of a [holomorphic function](holomorphic-function.md) as it approaches a domain boundary. On the disk, $H^p$ requires $\sup_{0<r<1}\int|F(re^{i\theta})|^p\,d\theta<\infty$; on the upper half-plane it requires $\sup_{y>0}\int_{\mathbb R}|f(x+iy)|^p\,dx<\infty$. For $p=\infty$ use a supremum norm. These analytic spaces differ from the [harmonic Hardy space of the upper half-space](partial-differential-equation.md#harmonic-hardy-space-of-the-upper-half-space); the [Hardy space of the circle](hilbert-space.md#hardy-space-of-the-circle) is the boundary Hilbert-space realization of the disk $H^2$ space.

### H1 space on the unit disk

↑ **Parent:** [Hardy space](#hardy-space)

This [Hardy space](#hardy-space) consists of [holomorphic functions](holomorphic-function.md) with $\|f\|_1=\sup_{r<1}\int_{\partial\mathbb D}|f(r\xi)|\,dm(\xi)<\infty$, where $m$ is normalized angular measure. The [H1 non-tangential maximal inequality on the disk](#h1-non-tangential-maximal-inequality-on-the-disk) controls their approach to the boundary, and the [Carleson embedding theorem on the disk](#carleson-embedding-theorem-on-the-disk) characterizes measures against which all these functions remain integrable.

#### H1 non-tangential maximal inequality on the disk

↑ **Parent:** [H1 space on the unit disk](#h1-space-on-the-unit-disk)

For an analytic [H1 space on the unit disk](#h1-space-on-the-unit-disk) function, its fixed-aperture [non-tangential maximal function](#non-tangential-maximal-function) obeys the displayed strong $L^1$ bound. First replace $f$ by $f_R(z)=f(Rz)$, $R<1$. The fact that [modulus powers of holomorphic functions are subharmonic](partial-differential-equation.md#modulus-powers-of-holomorphic-functions-are-subharmonic) gives $|f_R|^{1/2}\le P[|f(R\xi)|^{1/2}]$. Since a [Poisson maximal function is dominated by the Hardy-Littlewood maximal function](#poisson-maximal-function-is-dominated-by-the-hardy-littlewood-maximal-function), the strong $L^2$ [Hardy-Littlewood maximal inequality](analysis.md#hardy-littlewood-maximal-inequality) yields $\int N_Af_R\le C_A\int|f(R\xi)|\le C_A\|f\|_1$. Pointwise interior convergence and the [Fatou lemma](measure-theory.md#fatou-s-lemma) remove $R$. Analyticity permits this endpoint estimate; general $L^1$ boundary data have only a weak $L^1$ maximal bound.

#### Normalized squared Cauchy kernel

↑ **Parent:** [H1 space on the unit disk](#h1-space-on-the-unit-disk)

For $a\in\mathbb D$, this [holomorphic function](holomorphic-function.md) has [H1 space on the unit disk](#h1-space-on-the-unit-disk) norm one: its boundary modulus is the unit-mass [Poisson kernel on the circle](partial-differential-equation.md#poisson-kernel-on-the-circle). The radial integrals are bounded by that boundary integral by [subharmonic](partial-differential-equation.md#subharmonic-function) comparison and tend to it by continuity. Choosing $a$ at depth comparable to an arc's length makes $|f_a|$ bounded below by the reciprocal length throughout its [hyperbolic geodesic cap](hyperbolic-geometry.md#hyperbolic-geodesic-cap). It tests necessity in the [Carleson embedding theorem on the disk](#carleson-embedding-theorem-on-the-disk).

### H-infinity space

↑ **Parent:** [Hardy space](#hardy-space)

This [Hardy space](#hardy-space) consists of bounded [holomorphic functions](holomorphic-function.md) on the [unit disc](topology.md#unit-disc), with norm $\|f\|_\infty=\sup_{z\in\mathbb D}|f(z)|$. Its almost-everywhere boundary realization follows from the [Fatou theorem for bounded holomorphic functions](#fatou-theorem-for-bounded-holomorphic-functions).

#### Fatou theorem for bounded holomorphic functions

↑ **Parent:** [H-infinity space](#h-infinity-space)

A bounded [holomorphic function](holomorphic-function.md) on the [unit disc](topology.md#unit-disc) has finite [nontangential limits](complex-analysis.md#nontangential-limit) almost everywhere on its boundary. To outline a proof, bounded real and imaginary [harmonic](partial-differential-equation.md#harmonic-function) parts have $L^\infty$ boundary representations: apply the [Banach-Alaoglu theorem](functional-analysis.md#banach-alaoglu-theorem) to their circular traces and pass to the limit in the [Poisson integral on the unit disk](partial-differential-equation.md#poisson-integral-on-the-unit-disk). Almost every boundary point is a [Lebesgue point](measure-theory.md#lebesgue-point). The fact that a [Poisson integral converges nontangentially at Lebesgue points](partial-differential-equation.md#poisson-integral-converges-nontangentially-at-lebesgue-points) gives the desired limits. Their $L^\infty$ norm equals the interior supremum norm, and the [Poisson integral](partial-differential-equation.md#poisson-integral) recovers the original function. Exceptional points can lack even radial limits; $\exp(i\operatorname{Log}(1-z))$ is a bounded example at the boundary point one.

### F. and M. Riesz theorem

↑ **Parent:** [Hardy space](#hardy-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/F._and_M._Riesz_theorem)

If a finite complex [Borel measure](measure.md#borel-measure) $\mu$ on the circle has [Fourier coefficients](fourier-series.md#fourier-coefficient) $\widehat\mu(n)=0$ for all $n<0$, then it is absolutely continuous with respect to arc length. The reflected Fourier convention gives the equivalent theorem with positive coefficients vanishing. The [Poisson integral on the unit disk](partial-differential-equation.md#poisson-integral-on-the-unit-disk) is analytic because of the one-sided Fourier spectrum. Subharmonic comparison for its square root and an $L^2$ maximal estimate produce an integrable radial maximum. This maximum dominates the weak-star boundary measure, forcing [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures). The same proof on the real line says that a finite measure with [Fourier transform of a finite measure](fourier-transform.md#fourier-transform-of-a-finite-measure) supported in $[0,\infty)$ has a Lebesgue density.

<h2 id="calderon-zygmund-decomposition">Calderón–Zygmund decomposition</h2>

↑ **Parent:** [Harmonic analysis](harmonic-analysis.md)

For $f\in L^1(\mathbb R^d)$ and a positive threshold $\lambda$, take maximal dyadic cubes with mean of $|f|$ exceeding $\lambda$. They are disjoint, have total volume at most $\|f\|_1/\lambda$, and their means are at most $2^d\lambda$. Replace $f$ inside each selected cube by its mean to obtain $g$; write $b_Q=(f-f_Q)\mathbf1_Q$. Then $\|g\|_\infty\leq2^d\lambda$, $\|g\|_1\leq\|f\|_1$, $\int b_Q=0$, and $\sum_Q\|b_Q\|_1\leq2\|f\|_1$. The outside bound follows from the [Lebesgue differentiation theorem](measure-theory.md#lebesgue-differentiation-theorem). This separates a bounded part from localized cancellation errors.

## Positive-definite function

↑ **Parent:** [Harmonic analysis](harmonic-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive-definite_function)

A complex-valued function on a group is positive-definite when the displayed inequality holds for every finite choice of points and coefficients. This includes positive semidefinite, rather than necessarily strictly positive definite, Gram matrices. In particular $p(e)\geq0$ and $|p(x)|\leq p(e)$. On an Abelian group, every convolution square $u*u^*$ with $u\in C_c(G)$ is continuous and positive-definite: its quadratic form is the integral of $|\sum_i z_i u(t+x_i)|^2$.

### Cyclic unitary representation of a positive-definite function

↑ **Parent:** [Positive-definite function](#positive-definite-function)

For an Abelian group, on finite formal sums of group points, define $\langle[x],[y]\rangle=p(xy^{-1})$, with the first variable linear. Quotient by the null space of this [positive semidefinite](quadratic-form.md#positive-semidefinite-matrix) form and complete to a [Hilbert space](hilbert-space.md). Left translation is unitary, and $v=[e]$ generates a dense span of translated vectors. For continuous $p$, the equality $\|U_x[y]-[y]\|^2=2(p(e)-\operatorname{Re}p(x))$ gives [strong continuity](functional-analysis.md#strong-continuity). This realizes $p$ as a [matrix coefficient](representation-theory.md#matrix-coefficient) without assuming its integral representation.

<h3 id="bochner-s-theorem">Bochner's theorem</h3>

↑ **Parent:** [Positive-definite function](#positive-definite-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bochner's_theorem)

For a locally compact Hausdorff Abelian group, a continuous [positive-definite function](#positive-definite-function) $p$ is uniquely representable as $p(x)=\int_{\widehat G}\chi(x)\,d\mu_p(\chi)$ for a finite positive [Radon measure](measure.md#radon-measure) on the [Pontryagin dual group](group.md#pontryagin-dual-group). Its total mass is $p(e)$. Conversely every such finite positive measure defines a continuous positive-definite function.

<h4 id="bochner-herglotz-theorem">Bochner–Herglotz theorem</h4>

↑ **Parent:** [Bochner's theorem](#bochner-s-theorem)

A [positive-definite function](#positive-definite-function) $r$ on the discrete group $\mathbb Z$ is the sequence of [Fourier coefficients](fourier-series.md#fourier-coefficient) of a unique finite positive [Borel measure](measure.md#borel-measure) on the circle, with total mass $r(0)$. Positivity makes the finite sums $\sum_{|n|<N}(1-|n|/N)r(n)e^{-2\pi int}$ nonnegative. Their measures converge weakly to the required measure; uniqueness follows from density of [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) in continuous functions.

##### Wiener Fourier coefficient lemma

↑ **Parent:** [Bochner–Herglotz theorem](#bochner-herglotz-theorem)

For a finite positive [Borel measure](measure.md#borel-measure) on the circle, averaged squared [Fourier coefficients](fourier-series.md#fourier-coefficient) tend to the sum of squares of its atomic masses. Express each squared coefficient as a double integral and average the circle character. The averaged character is bounded by one, tends to one on the diagonal and to zero elsewhere, so the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) gives the diagonal mass. In particular an atomless measure has vanishing averaged absolute coefficients by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

#### Bochner consistency identity for convolution squares

↑ **Parent:** [Bochner's theorem](#bochner-s-theorem)

For finite sums of compactly supported convolution squares, $\widehat p,\widehat q\geq0$. Insert the [Bochner theorem](#bochner-s-theorem) representation of $q$ into $p*q$ and apply the [Fubini theorem](measure-theory.md#fubini-s-theorem): its representing measure is $\widehat p\,\mu_q$. Reversing $p,q$ and using uniqueness gives the displayed identity. It makes the local quotients $\mu_p/\widehat p$ consistent wherever $\widehat p>0$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Christopher E. Heil](mathematics.md#christopher-e-heil)
