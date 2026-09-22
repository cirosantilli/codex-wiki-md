# Brownian motion

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_motion)

A standard Brownian motion starts at zero, has almost surely continuous paths, and has independent Gaussian increments

$$
W_t-W_s\sim N(0,t-s)
\qquad(0\leq s<t).
$$

**Table of contents**

- [Strict comparison of one-sided and absolute Brownian maxima](#strict-comparison-of-one-sided-and-absolute-brownian-maxima)
- [Brownian sign transform](#brownian-sign-transform)
- [Cylindrical Brownian motion](#cylindrical-brownian-motion)
- [Brownian motion under a quadratic time change](#brownian-motion-under-a-quadratic-time-change)
- [Rotational invariance of Brownian motion](#rotational-invariance-of-brownian-motion)
- [Brownian moment recursion](#brownian-moment-recursion)
  - [Centered Brownian powers need not be martingales](#centered-brownian-powers-need-not-be-martingales)
- [Planar Brownian motion avoids a fixed point](#planar-brownian-motion-avoids-a-fixed-point)
- [Lévy area](#levy-area)
- [Projection criterion for Brownian avoidance of affine subspaces](#projection-criterion-for-brownian-avoidance-of-affine-subspaces)
- [Wiener sausage](#wiener-sausage)
  - [Survival among independently moving Poisson traps](#survival-among-independently-moving-poisson-traps)
- [Blumenthal zero-one law](#blumenthal-zero-one-law)
- [Brownian increment](#brownian-increment)
- [Brownian fluctuations exceed the square-root scale](#brownian-fluctuations-exceed-the-square-root-scale)
- [Integrated Brownian motion](#integrated-brownian-motion)
- [Integrated square of Brownian motion](#integrated-square-of-brownian-motion)
  - [Laplace transform of the integrated square of Brownian motion](#laplace-transform-of-the-integrated-square-of-brownian-motion)
- [Brownian time reversal on a finite interval](#brownian-time-reversal-on-a-finite-interval)
  - [Independent Brownian arms at a deterministic time](#independent-brownian-arms-at-a-deterministic-time)
- [Longitudinal Brownian field with transverse covariance](#longitudinal-brownian-field-with-transverse-covariance)
- [Local maximum of Brownian motion](#local-maximum-of-brownian-motion)
- [Nowhere monotonicity of Brownian motion](#nowhere-monotonicity-of-brownian-motion)
- [Brownian hitting of lattice spheres](#brownian-hitting-of-lattice-spheres)
- [Brownian paths are not uniformly continuous on the half-line](#brownian-paths-are-not-uniformly-continuous-on-the-half-line)
- [Brownian filtration](#brownian-filtration)
  - [Natural Brownian filtration](#natural-brownian-filtration)
- [Martingale representation theorem](#martingale-representation-theorem)
  - [Brownian martingale representation theorem](#brownian-martingale-representation-theorem)
    - [Clark-Ocone formula for a smooth Brownian terminal payoff](#clark-ocone-formula-for-a-smooth-brownian-terminal-payoff)
- [Exponential martingale for Brownian motion](#exponential-martingale-for-brownian-motion)
- [Integral of Brownian motion](#integral-of-brownian-motion)
  - [Brownian motion transform by three times its running average](#brownian-motion-transform-by-three-times-its-running-average)
- [Diffusion coefficient](#diffusion-coefficient)
  - [Solutal diffusivity](#solutal-diffusivity)
- [Orthogonal invariance of Brownian motion](#orthogonal-invariance-of-brownian-motion)
- [Meeting time of two independent Brownian motions](#meeting-time-of-two-independent-brownian-motions)
- [Wiener measure](#wiener-measure)
  - [Wiener theorem](#wiener-theorem)
  - [Cameron-Martin space of Wiener measure](#cameron-martin-space-of-wiener-measure)
    - [Cameron-Martin theorem](#cameron-martin-theorem)
      - [Cameron-Martin shifts on infinite Wiener path space](#cameron-martin-shifts-on-infinite-wiener-path-space)
      - [Cameron-Martin theorem for a linear drift](#cameron-martin-theorem-for-a-linear-drift)
        - [First-passage density of Brownian motion with positive drift](#first-passage-density-of-brownian-motion-with-positive-drift)
- [Brownian Hölder regularity](#brownian-holder-regularity)
- [Brownian zero set](#brownian-zero-set)
- [Reflection invariance of Brownian motion](#reflection-invariance-of-brownian-motion)
- [Critical exponential moment of a drifted Brownian hitting time](#critical-exponential-moment-of-a-drifted-brownian-hitting-time)
- [Bessel process](#bessel-process)
  - [Two-dimensional Bessel transition law](#two-dimensional-bessel-transition-law)
  - [Squared Bessel process](#squared-bessel-process)
    - [Additivity of independently driven squared Bessel processes](#additivity-of-independently-driven-squared-bessel-processes)
  - [Oppositely driven Bessel exit probability](#oppositely-driven-bessel-exit-probability)
  - [Truncation construction of a positive Bessel strong solution](#truncation-construction-of-a-positive-bessel-strong-solution)
  - [Three-dimensional Bessel process](#three-dimensional-bessel-process)
    - [Logarithmic escape rate of three-dimensional Brownian motion](#logarithmic-escape-rate-of-three-dimensional-brownian-motion)
  - [Beta integral for strict ordering of coupled Bessel lifetimes](#beta-integral-for-strict-ordering-of-coupled-bessel-lifetimes)
  - [Reciprocal three-dimensional Bessel strict local martingale](#reciprocal-three-dimensional-bessel-strict-local-martingale)
  - [Bessel power local martingale](#bessel-power-local-martingale)
    - [Stopped inverse radial power martingale classification](#stopped-inverse-radial-power-martingale-classification)
    - [All-time minimum of a transient Bessel process](#all-time-minimum-of-a-transient-bessel-process)
  - [Hitting-zero classification for a Bessel process](#hitting-zero-classification-for-a-bessel-process)
    - [Finite-time access to zero for Bessel dimensions below two](#finite-time-access-to-zero-for-bessel-dimensions-below-two)
  - [Scaling invariance of a Bessel process](#scaling-invariance-of-a-bessel-process)
  - [Exponential Brownian-to-Bessel time change](#exponential-brownian-to-bessel-time-change)
    - [Logarithmic growth of an exponential Brownian clock with positive drift](#logarithmic-growth-of-an-exponential-brownian-clock-with-positive-drift)
  - [Power time change of a Bessel process](#power-time-change-of-a-bessel-process)
- [Reflected Brownian motion](#reflected-brownian-motion)
  - [Reflected Brownian motion with negative drift](#reflected-brownian-motion-with-negative-drift)
    - [Stationary law of negatively drifted reflected Brownian motion](#stationary-law-of-negatively-drifted-reflected-brownian-motion)
- [Brownian occupation time](#brownian-occupation-time)
  - [Infinite occupation time of one-dimensional Brownian motion](#infinite-occupation-time-of-one-dimensional-brownian-motion)
    - [Divergence of a driftless Brownian exponential clock](#divergence-of-a-driftless-brownian-exponential-clock)
  - [Occupation-times formula](#occupation-times-formula)
- [Planar Brownian motion](#planar-brownian-motion)
  - [Area of a planar Brownian path](#area-of-a-planar-brownian-path)
  - [Logarithmic radius of planar Brownian motion](#logarithmic-radius-of-planar-brownian-motion)
    - [Winding at logarithmic radial passage levels](#winding-at-logarithmic-radial-passage-levels)
  - [Planar Brownian stochastic area](#planar-brownian-stochastic-area)
    - [Orthogonality of the radial martingale and planar Brownian area](#orthogonality-of-the-radial-martingale-and-planar-brownian-area)
      - [Common-clock Brownian representation of radius and area](#common-clock-brownian-representation-of-radius-and-area)
  - [Brownian excursion in the upper half-plane](#brownian-excursion-in-the-upper-half-plane)
    - [Restriction probability of a Brownian half-plane excursion](#restriction-probability-of-a-brownian-half-plane-excursion)
      - [Boundary derivative is an excursion avoidance probability](#boundary-derivative-is-an-excursion-avoidance-probability)
  - [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)
    - [Small-radius Brownian winding law](#small-radius-brownian-winding-law)
    - [Cauchy exit law from a Brownian half-plane](#cauchy-exit-law-from-a-brownian-half-plane)
    - [Complex exponential construction of planar Brownian motion](#complex-exponential-construction-of-planar-brownian-motion)
    - [Power-map reduction for Brownian exit from a wedge](#power-map-reduction-for-brownian-exit-from-a-wedge)
      - [Brownian wedge-exit probability](#brownian-wedge-exit-probability)
    - [Conformal Brownian clock](#conformal-brownian-clock)
      - [Finite exit from a conformal image of a bounded planar domain](#finite-exit-from-a-conformal-image-of-a-bounded-planar-domain)
  - [Rotational invariance of planar Brownian motion](#rotational-invariance-of-planar-brownian-motion)
  - [Recurrence of planar Brownian motion](#recurrence-of-planar-brownian-motion)
    - [Polar point for planar Brownian motion](#polar-point-for-planar-brownian-motion)
    - [Divergence of a positive planar Brownian occupation integral](#divergence-of-a-positive-planar-brownian-occupation-integral)
  - [Brownian reflection coupling](#brownian-reflection-coupling)
  - [Harmonic measure](#harmonic-measure)
    - [Brownian exit law from a quadrant](#brownian-exit-law-from-a-quadrant)
    - [Harmonic capacity from infinity in the upper half-plane](#harmonic-capacity-from-infinity-in-the-upper-half-plane)
      - [Reflection lower bound for harmonic hull capacity](#reflection-lower-bound-for-harmonic-hull-capacity)
      - [Radius gives no positive lower bound for disconnected harmonic hull capacity](#radius-gives-no-positive-lower-bound-for-disconnected-harmonic-hull-capacity)
      - [Subadditivity of harmonic hull capacity](#subadditivity-of-harmonic-hull-capacity)
    - [Harmonic-measure asymptotic at infinity](#harmonic-measure-asymptotic-at-infinity)
    - [Möbius calculation of circular Brownian exit](#mobius-calculation-of-circular-brownian-exit)
    - [Reflection identity for Brownian exit from a half-disc](#reflection-identity-for-brownian-exit-from-a-half-disc)
    - [Bottom-boundary harmonic measure of a strip](#bottom-boundary-harmonic-measure-of-a-strip)
    - [Upper-half-plane harmonic measure of the positive half-axis](#upper-half-plane-harmonic-measure-of-the-positive-half-axis)
    - [Planar Brownian annulus hitting probability](#planar-brownian-annulus-hitting-probability)
    - [Brownian entrance law to a disc from infinity](#brownian-entrance-law-to-a-disc-from-infinity)
- [Coordinatewise coalescing coupling of Brownian motions](#coordinatewise-coalescing-coupling-of-brownian-motions)
- [Strong law for Brownian motion](#strong-law-for-brownian-motion)
- [Brownian loop measure](#brownian-loop-measure)
  - [Pinned Brownian loop measure at an interior point](#pinned-brownian-loop-measure-at-an-interior-point)
  - [Conformal restriction measure on simple loops](#conformal-restriction-measure-on-simple-loops)
    - [Recovery of a loop measure from conformal deficits](#recovery-of-a-loop-measure-from-conformal-deficits)
- [Nowhere differentiability of Brownian motion](#nowhere-differentiability-of-brownian-motion)
- [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion)
  - [Lévy characterization of multidimensional Brownian motion](#levy-characterization-of-multidimensional-brownian-motion)
- [Brownian scaling](#brownian-scaling)
- [Recurrence of one-dimensional Brownian motion](#recurrence-of-one-dimensional-brownian-motion)
- [Transience of Brownian motion in dimension at least three](#transience-of-brownian-motion-in-dimension-at-least-three)
  - [Brownian sphere-hitting probability in dimension three](#brownian-sphere-hitting-probability-in-dimension-three)
    - [Last visit to a bounded ball for three-dimensional Brownian motion](#last-visit-to-a-bounded-ball-for-three-dimensional-brownian-motion)
- [Brownian exit time](#brownian-exit-time)
  - [Brownian hitting probability of a ball](#brownian-hitting-probability-of-a-ball)
    - [Small-ball Brownian hitting asymptotic](#small-ball-brownian-hitting-asymptotic)
  - [Brownian exit-time expectation in an orthant](#brownian-exit-time-expectation-in-an-orthant)
  - [Uniform ball sampling by Brownian stopping](#uniform-ball-sampling-by-brownian-stopping)
    - [Brownian exit-time ball averaging identity](#brownian-exit-time-ball-averaging-identity)
      - [Finiteness propagation of Brownian mean exit times](#finiteness-propagation-of-brownian-mean-exit-times)
  - [Brownian exit from an interval](#brownian-exit-from-an-interval)
    - [Asymmetric Brownian interval-exit transform](#asymmetric-brownian-interval-exit-transform)
    - [Brownian exit-time skeleton](#brownian-exit-time-skeleton)
      - [Gaussian limit of a Brownian exit skeleton](#gaussian-limit-of-a-brownian-exit-skeleton)
      - [Brownian exit-skeleton clock convergence](#brownian-exit-skeleton-clock-convergence)
    - [Laplace transform of symmetric Brownian interval-exit time](#laplace-transform-of-symmetric-brownian-interval-exit-time)
    - [Brownian symmetric interval-exit moments](#brownian-symmetric-interval-exit-moments)
    - [Conditional Brownian interval-exit time](#conditional-brownian-interval-exit-time)
  - [Dynkin formula for Brownian motion](#dynkin-formula-for-brownian-motion)
- [Brownian bridge](#brownian-bridge)
  - [Time reversal of a Brownian bridge](#time-reversal-of-a-brownian-bridge)
  - [Stochastic integral representation of a Brownian bridge](#stochastic-integral-representation-of-a-brownian-bridge)
  - [F-Brownian bridge](#f-brownian-bridge)
  - [Brownian bridge independence from its endpoint](#brownian-bridge-independence-from-its-endpoint)
  - [Brownian-bridge crossing probability](#brownian-bridge-crossing-probability)
- [Exponential Brownian martingale](#exponential-brownian-martingale)
  - [Parameter derivative of the exponential Brownian martingale](#parameter-derivative-of-the-exponential-brownian-martingale)
- [Gaussian-process characterization of Brownian motion](#gaussian-process-characterization-of-brownian-motion)
- [Time inversion of Brownian motion](#time-inversion-of-brownian-motion)
- [Brownian motion with drift](#brownian-motion-with-drift)
  - [Drifted Brownian interval-exit probability](#drifted-brownian-interval-exit-probability)
  - [Infinite-horizon singularity of Brownian motion with constant drift](#infinite-horizon-singularity-of-brownian-motion-with-constant-drift)
  - [Finite-horizon maximum of Brownian motion with negative drift](#finite-horizon-maximum-of-brownian-motion-with-negative-drift)
  - [Infinite-horizon crossing probability for Brownian motion with negative drift](#infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift)
  - [Last passage time above a level for Brownian motion with negative drift](#last-passage-time-above-a-level-for-brownian-motion-with-negative-drift)
- [Reflection principle (Wiener process)](#reflection-principle-wiener-process)
  - [Brownian terminal-to-maximum ratio](#brownian-terminal-to-maximum-ratio)
  - [Brownian reflection at a stopping time](#brownian-reflection-at-a-stopping-time)
  - [Brownian running maximum](#brownian-running-maximum)
    - [Gaussian maximal bound for Brownian motion](#gaussian-maximal-bound-for-brownian-motion)
    - [Atomless maxima on separated Brownian intervals](#atomless-maxima-on-separated-brownian-intervals)
    - [Finite-horizon maximum of Brownian motion with drift](#finite-horizon-maximum-of-brownian-motion-with-drift)
      - [Joint endpoint and maximum law for drifted Brownian motion](#joint-endpoint-and-maximum-law-for-drifted-brownian-motion)
    - [Integral lower envelope for the Brownian maximum](#integral-lower-envelope-for-the-brownian-maximum)
    - [Brownian barrier survival asymptotic](#brownian-barrier-survival-asymptotic)
    - [Maximum before a lower Brownian barrier](#maximum-before-a-lower-brownian-barrier)
    - [Joint distribution of Brownian motion and its running maximum](#joint-distribution-of-brownian-motion-and-its-running-maximum)
    - [Lévy identity for Brownian motion](#levy-identity-for-brownian-motion)
    - [Time of the Brownian maximum](#time-of-the-brownian-maximum)
      - [Brownian motion shifted at its finite-horizon maximum](#brownian-motion-shifted-at-its-finite-horizon-maximum)
- [Brownian transition semigroup](#brownian-transition-semigroup)
  - [Brownian transition density](#brownian-transition-density)
    - [Killed Brownian transition density](#killed-brownian-transition-density)
  - [Brownian compensator martingale](#brownian-compensator-martingale)
- [Exponential test-function characterization of Brownian motion](#exponential-test-function-characterization-of-brownian-motion)
  - [Conditional characteristic-function criterion for Brownian increments](#conditional-characteristic-function-criterion-for-brownian-increments)

## Strict comparison of one-sided and absolute Brownian maxima

↑ **Parent:** [Brownian motion](brownian-motion.md)

For $t>0$, let $M_t=\sup_{s\leq t}B_s$ and $A_t=\sup_{s\leq t}|B_s|$. The [Brownian reflection principle](#reflection-principle-wiener-process) gives $M_t\overset d=|B_t|$, hence $\|M_t\|_2=\sqrt t$. Also $A_t\geq M_t$, with strict inequality on the positive-probability event $\{B_t<-\lambda,M_t<\lambda\}$: reflection gives its probability as $\mathbb P(B_t>\lambda)-\mathbb P(B_t>3\lambda)>0$. The [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) bounds $\|A_t\|_2\leq2\sqrt t$, so $\sqrt t<\|A_t\|_2\leq2\sqrt t$. At $t=0$ all quantities vanish and the lower inequality is equality.

// Target: probability-theory.bigb

## Brownian sign transform

↑ **Parent:** [Brownian motion](brownian-motion.md)

The sign transform of standard [Brownian motion](brownian-motion.md) is itself standard Brownian motion. The integrand is [predictable](martingale.md#predictable-process) because it is a Borel function of a continuous adapted process. Brownian motion spends zero Lebesgue time at a specified level: integrate $\mathbb P(B_s=0)=0$ over positive times. Consequently the transform's [quadratic variation](stochastic-calculus.md#quadratic-variation) is $t$, regardless of the chosen sign value at zero. The [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion) applies.

## Cylindrical Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

On a real [Hilbert space](hilbert-space.md) $H$, this centered jointly [Gaussian process](stochastic-process.md#gaussian-process) is linear in its test vector $h$ and has the displayed covariance, with independent increments in time. Equivalently choose an orthonormal basis and independent real [Brownian motions](brownian-motion.md) $W^j$, and define stochastic integration by $\int\langle v_s,dW_s\rangle=\sum_j\int\langle v_s,e_j\rangle dW_s^j$ whenever $\int\|v_s\|^2ds<\infty$. In infinite dimension it need not be an $H$-valued [random variable](random-variable.md); the integral is the meaningful object.

## Brownian motion under a quadratic time change

↑ **Parent:** [Brownian motion](brownian-motion.md)

The process $M_t=B_{t^2}$ is a martingale in the filtration $\mathcal G_t=\mathcal F_{t^2}$ and has [quadratic variation](stochastic-calculus.md#quadratic-variation) $t^2$. The integral $W_t=\int_0^t(2s)^{-1/2}dM_s$ is well defined because its bracket is $\int_0^t(2s)^{-1}d(s^2)=t$. The [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion) makes $W$ Brownian in this filtration, and stochastic-integral associativity gives the displayed representation. The resulting integrand is continuous at zero despite the singular inverse integrand.

## Rotational invariance of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

For standard [Brownian motion](brownian-motion.md) started at zero in $\mathbb R^n$, every fixed [orthogonal transformation](linear-algebra.md#orthogonal-transformation) preserves the process law. Its transformed increments remain [independent](random-variable.md#independent-random-variables) centred [Gaussian random vectors](probability-and-statistics.md#gaussian-random-vector) with [covariance](variance.md#covariance) $(t-s)I$, and its paths remain continuous. Consequently its exit law from any centred sphere is normalized surface measure. Translations give the same assertion for spheres centred at its starting point.

## Brownian moment recursion

↑ **Parent:** [Brownian motion](brownian-motion.md)

For standard one-dimensional Brownian motion, the Itô formula for $B^k$ gives this recursion. Stop at exits from $[-n,n]$ to make the stochastic integral a true martingale. Gaussian tail integrability and the [Doob Lp maximal inequality](martingale.md#doob-lp-maximal-inequality) dominate all stopped powers on a fixed horizon, justifying the limit. Odd moments vanish and $\mathbb EB_t^{2k}=(2k)!t^k/(2^kk!)$.

// Target: probability-and-statistics.bigb

### Centered Brownian powers need not be martingales

↑ **Parent:** [Brownian moment recursion](#brownian-moment-recursion)

The process $B_t^k-\mathbb EB_t^k$ is a martingale only for $k=1,2$. For higher powers its finite-variation drift is $k(k-1)(B_t^{k-2}-\mathbb EB_t^{k-2})/2$, which is not identically zero. Subtracting the random compensator $k(k-1)\int_0^tB_s^{k-2}ds/2$ instead produces a true martingale on each finite horizon.

// Target: probability-and-statistics.bigb

## Planar Brownian motion avoids a fixed point

↑ **Parent:** [Brownian motion](brownian-motion.md)

Planar Brownian motion started away from zero does not hit zero. Stopping the harmonic function $\log|x|$ on an annulus gives probability $(\log R-\log|x|)/(\log R-\log\varepsilon)$ of reaching its inner circle before its outer circle. This tends to zero as $\varepsilon\downarrow0$. Exhausting the plane by outer circles proves point avoidance at finite times.

// Target: probability-and-statistics.bigb

<h2 id="levy-area">Lévy area</h2>

↑ **Parent:** [Brownian motion](brownian-motion.md)

Lévy area is the antisymmetric second-level integral of multidimensional [Brownian motion](brownian-motion.md). For distinct independent components the integrals are also [Itô integrals](stochastic-calculus.md#ito-integral). Combined with the symmetric tensor $\tfrac12 B_{s,t}^{\otimes2}$, it gives the second level of [enhanced Brownian motion](analysis.md#enhanced-brownian-motion). It is not continuously determined by the uniform norm of the Brownian path.

## Projection criterion for Brownian avoidance of affine subspaces

↑ **Parent:** [Brownian motion](brownian-motion.md)

A [Brownian motion](brownian-motion.md) starting outside a fixed affine subspace of codimension at least two almost surely never hits it. Choose a two-dimensional orthogonal projection annihilating the subspace's direction and with nonzero projected initial displacement. The projected process is planar [Brownian motion](brownian-motion.md) starting away from zero, and a hit of the subspace would hit zero in that projection. The [polar point for planar Brownian motion](#polar-point-for-planar-brownian-motion) result excludes this. In three dimensions this shows avoidance of every fixed line when started outside it.

## Wiener sausage

↑ **Parent:** [Brownian motion](brownian-motion.md)

A Wiener sausage is the region swept out by a ball of fixed radius along a [Brownian motion](brownian-motion.md) path. A deterministic continuous displacement $f(s)$ gives the variant $\bigcup_{s\leq t}\mathcal B(B_s+f(s),r)$. On each bounded time interval it has finite expected volume: the region lies inside a ball whose radius is the path's maximum displacement plus $r$, and the Brownian maximum has Gaussian tail bounds and finite moments of every order.

### Survival among independently moving Poisson traps

↑ **Parent:** [Wiener sausage](#wiener-sausage)

Start traps at a unit-intensity [Poisson random measure](probability-theory.md#poisson-random-measure) in Euclidean space and attach mutually [independent](random-variable.md#independent-random-variables) [Brownian motions](brownian-motion.md), [independent](random-variable.md#independent-random-variables) of the initial measure. For a deterministic target path $f$, independently thin initial positions according to whether their marked path comes within radius one of the target by time $t$. The retention [probability](probability-theory.md#probability) $p_t(x)$ integrates, by the [Tonelli theorem](measure-theory.md#tonelli-theorem), to the expected volume of the sausage along $f-B$. Symmetry of [Brownian motion](brownian-motion.md) makes this the expected volume of the sausage along $f+B$. The Poisson zero-count [probability](probability-theory.md#probability) proves the displayed survival formula. This derives the formula directly from [independent](random-variable.md#independent-random-variables) thinning, without assuming a separate marking or displacement theorem.

## Blumenthal zero-one law

↑ **Parent:** [Brownian motion](brownian-motion.md)

For the completed natural [Brownian filtration](#brownian-filtration), every event in the germ sigma-field of [Brownian motion](brownian-motion.md) has probability zero or one. Indeed, an event measurable at every positive time is independent of all increments after each such time. Letting that time decrease to zero and using path continuity makes the event independent of the entire Brownian path sigma-field. Since it is itself measurable in that sigma-field, its probability equals its square.

## Brownian increment

↑ **Parent:** [Brownian motion](brownian-motion.md)

An increment of a [Brownian motion](brownian-motion.md) between deterministic times $s<t$ is $W_t-W_s$. It has [normal distribution](probability-theory.md#normal-distribution) $N(0,t-s)$ and is independent of the filtration up to time $s$. Increments on disjoint time intervals are independent. Their [covariance](variance.md#covariance) is the length of overlap of the corresponding intervals; this also follows from the [Brownian covariance kernel](random-variable.md#brownian-covariance-kernel).

## Brownian fluctuations exceed the square-root scale

↑ **Parent:** [Brownian motion](brownian-motion.md)

At integer times, $B_n/\sqrt n$ has the same standard [normal distribution](probability-theory.md#normal-distribution) for every $n$. The event that its limit superior exceeds a fixed finite level is a [tail event](probability-theory.md#tail-event) of the independent unit-time Brownian increments, since changing any finite initial segment contributes only a term tending to zero. The [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law) applies. Its probability is positive because each fixed-time exceedance has the same positive probability, giving a positive probability of infinitely many exceedances by the decreasing union-of-tail-events argument. Thus its probability is one. Intersecting over integer levels proves the stated divergence, without the lower iterated-logarithm bound.

## Integrated Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

The ordinary time integral of standard [Brownian motion](brownian-motion.md) is a centered [Gaussian process](stochastic-process.md#gaussian-process) with continuously differentiable paths and derivative $B_t$. For $0\leq s\leq t$, its [covariance](variance.md#covariance) is $\mathbb E(I_sI_t)=s^2(3t-s)/6$, obtained by integrating the Brownian [covariance](variance.md#covariance) $\min(u,v)$. Consequently $I_t$ has [normal distribution](probability-theory.md#normal-distribution) $N(0,t^3/3)$. This time integral is distinct from the [Itô integral](stochastic-calculus.md#ito-integral) with respect to [Brownian motion](brownian-motion.md).

## Integrated square of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

The quadratic functional $Q=\int_0^1W_t^2dt$ is finite almost surely. The [Brownian half-integer sine expansion](statistical-modelling.md#brownian-half-integer-sine-expansion) writes it as a sum of independent scaled squared standard normals. Its mean is $1/2$, and its Laplace transform is determined by a hyperbolic cosine product.

### Laplace transform of the integrated square of Brownian motion

↑ **Parent:** [Integrated square of Brownian motion](#integrated-square-of-brownian-motion)

The independent squared-normal series for the [integrated square of Brownian motion](#integrated-square-of-brownian-motion) gives the product $\prod_n(1+2\lambda/((n-1/2)^2\pi^2))^{-1/2}$. The half-integer cosine product reduces this to $(\cosh\sqrt{2\lambda})^{-1/2}$. Expanding at zero gives mean $1/2$ and variance $1/3$.

## Brownian time reversal on a finite interval

↑ **Parent:** [Brownian motion](brownian-motion.md)

For standard [Brownian motion](brownian-motion.md) and deterministic $T>0$, the process $R_s=B_T-B_{T-s}$, $0\leq s\leq T$, is standard [Brownian motion](brownian-motion.md) on that interval in its own [natural filtration](stochastic-process.md#natural-filtration). Disjoint reversed time intervals give independent centered normal increments with the correct variances. This is different from an arbitrary random-time shift, which can depend on future data. It is also different from the [time inversion of Brownian motion](#time-inversion-of-brownian-motion) transformation $tB_{1/t}$.

### Independent Brownian arms at a deterministic time

↑ **Parent:** [Brownian time reversal on a finite interval](#brownian-time-reversal-on-a-finite-interval)

For a deterministic $h>0$, the processes $B_{h-t}-B_h$, $0\leq t\leq h$, and $B_{h+t}-B_h$, $t\geq0$, are independent standard [Brownian motions](brownian-motion.md). The first uses reversed, sign-changed past increments; the second uses future increments independent of the entire past. The first process is not generally independent of $B_h$, but translating a range by $B_h$ preserves its [Lebesgue measure](measure-theory.md#lebesgue-measure) pathwise.

## Longitudinal Brownian field with transverse covariance

↑ **Parent:** [Brownian motion](brownian-motion.md)

A longitudinal Brownian field $\mathcal B_x(z)$ is a centered [Gaussian random field](stochastic-process.md#gaussian-random-field) with

$$
 \mathbb E[\mathcal B_x(z)\mathcal B_{x'}(z')]=\min(x,x')B(z-z'),\qquad x,x'\geq0,
$$

where $B$ is a valid transverse [covariance kernel](random-variable.md#covariance-kernel). For each fixed $z$ it is a scaled [Brownian motion](brownian-motion.md), and increments over disjoint longitudinal intervals are independent. Such a field drives a Markov model of [wave propagation in a random medium](physics.md#wave-propagation-in-a-random-medium). Its formal longitudinal derivative is [Gaussian white noise](stochastic-process.md#gaussian-white-noise) in $x$, with transverse correlations described by $B$; it is not in general a Brownian sheet.

## Local maximum of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

The times of [local maxima](analysis.md#local-maximum) of a [Brownian motion](brownian-motion.md) path are dense in the half-line [almost surely](convergence-of-random-variables.md#almost-sure-convergence), and every such [local maximum](analysis.md#local-maximum) is a [strict local maximum](analysis.md#strict-local-maximum). Density follows from [nowhere monotonicity of Brownian motion](#nowhere-monotonicity-of-brownian-motion) and the [extreme value theorem](real-analysis.md#extreme-value-theorem). Strictness follows by checking that maxima over separated rational compact time intervals are unequal; the increment across their gap supplies an independent nondegenerate [normal distribution](probability-theory.md#normal-distribution).

## Nowhere monotonicity of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

Almost surely, no restriction of a [Brownian motion](brownian-motion.md) path to an interval of positive length is a [monotone function](calculus.md#monotonic-function). On a fixed interval, monotonicity forces the independent centered [normal random variables](probability-theory.md#gaussian-random-variable) given by every dyadic subdivision's increments to have the same sign. The probability is at most $2^{1-2^m}$ for a subdivision into $2^m$ pieces. A countable union over rational intervals gives the simultaneous pathwise assertion.

## Brownian hitting of lattice spheres

↑ **Parent:** [Brownian motion](brownian-motion.md)

For three-dimensional [Brownian motion](brownian-motion.md), every radius $r>0$ and every initial point satisfy

$$
\mathbb P_x\bigl(\exists t\geq0,\ z\in\mathbb Z^3:\ |B_t+z|=r\bigr)=1.
$$

If the initial point is on one of the [spheres](geometry-and-topology.md#sphere), it is already a hit at time zero. If it is inside a lattice-centered [open ball](topology.md#open-ball), its eventual exit hits that [sphere](geometry-and-topology.md#sphere). Otherwise choose at each integer time a nearest lattice center. The current displacement from it has norm at most $\sqrt3/2$, so the [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) of the next unit increment gives a uniform positive chance of entering its radius-$r/2$ [open ball](topology.md#open-ball). The [geometric tail bound from a uniform escape probability](martingale.md#geometric-tail-bound-from-a-uniform-escape-probability) makes eventual entry certain, and continuity forces a boundary crossing. This periodic-family recurrence does not contradict the [Brownian sphere-hitting probability in dimension three](#brownian-sphere-hitting-probability-in-dimension-three) for one fixed [sphere](geometry-and-topology.md#sphere).

## Brownian paths are not uniformly continuous on the half-line

↑ **Parent:** [Brownian motion](brownian-motion.md)

For every fixed mesh $1/k$, [independent increments](stochastic-process.md#independent-increments) with the [normal distribution](probability-theory.md#normal-distribution) imply increments of absolute value greater than one occur infinitely often [almost surely](convergence-of-random-variables.md#almost-sure-convergence), by the second [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas). A countable intersection over $k$ contradicts [uniform continuity](topological-analysis.md#uniform-continuity) on $[0,\infty)$.

## Brownian filtration

↑ **Parent:** [Brownian motion](brownian-motion.md)

A [filtration](stochastic-process.md#filtration-probability-theory) $(\mathcal F_t)$ is a [Brownian filtration](#brownian-filtration) for $B$ when $B$ is an [adapted process](stochastic-process.md#adapted-process) and each future increment $B_t-B_s$ is independent of $\mathcal F_s$. The [natural filtration](stochastic-process.md#natural-filtration) of a [Brownian motion](brownian-motion.md) has this property. Arbitrary enlargement by future information need not preserve it.

### Natural Brownian filtration

↑ **Parent:** [Brownian filtration](#brownian-filtration)

The natural Brownian filtration is the [natural filtration](stochastic-process.md#natural-filtration) generated by a [Brownian motion](brownian-motion.md). Its usual augmentation adds null events and makes it right-continuous; the [Brownian martingale representation theorem](#brownian-martingale-representation-theorem) holds for this augmented natural filtration. A larger [Brownian filtration](#brownian-filtration) can preserve independence of future increments while containing additional randomness, so it need not have martingale representation with respect to the specified [Brownian motion](brownian-motion.md).

## Martingale representation theorem

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Martingale_representation_theorem)

A martingale representation theorem states conditions under which every martingale in a filtration can be represented as a stochastic integral with respect to one or more fundamental martingales.

### Brownian martingale representation theorem

↑ **Parent:** [Martingale representation theorem](#martingale-representation-theorem)

Every square-integrable random variable measurable with respect to a Brownian filtration can be written as its expectation plus an [Itô integral](stochastic-calculus.md#ito-integral) against that Brownian motion. Equivalently, every square-integrable martingale in that filtration has the form

$$
M_t=M_0+\int_0^tH_s\,dW_s
$$

for a predictable square-integrable process $H$.

#### Clark-Ocone formula for a smooth Brownian terminal payoff

↑ **Parent:** [Brownian martingale representation theorem](#brownian-martingale-representation-theorem)

In the completed natural [Brownian filtration](#brownian-filtration), a bounded continuously differentiable $\phi$ with bounded derivative satisfies

$$
\phi(W_T)=\mathbb E\phi(W_T)+\int_0^T\mathbb E[\phi'(W_T)\mid\mathcal F_t]\,dW_t.
$$

The integrand is unique up to $d\mathbb P\,dt$-almost everywhere equality. [Gaussian integration by parts](probability-theory.md#stein-s-lemma-probability) first gives the duality between the payoff and every square-integrable [Itô integral](stochastic-calculus.md#ito-integral). The [Brownian martingale representation theorem](#brownian-martingale-representation-theorem) then identifies the integrand as the projection of $\phi'(W_T)\mathbf1_{\{t\le T\}}$ onto the [predictable processes](martingale.md#predictable-process) in the product $L^2$ space. This explains the [conditional expectation](measure-theory.md#conditional-expectation) in the formula, rather than a nonadapted terminal derivative.

## Exponential martingale for Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

For every $\theta\in\mathbb R$ and standard [Brownian motion](brownian-motion.md) $B$,

$$
\exp\left(\theta B_t-\frac12\theta^2t\right)
$$

is a positive martingale. Applying [Itô formula](stochastic-calculus.md#ito-s-lemma) cancels the drift, and its expectation is one by the moment-generating function of the [normal distribution](probability-theory.md#normal-distribution).

## Integral of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

For Brownian motion started at $x$, the time integral is a [Gaussian random variable](probability-theory.md#gaussian-random-variable) with

$$
\mathbb E_x\int_0^tB_sds=xt,
\qquad
\operatorname{Var}\left(\int_0^tB_sds\right)=\frac{t^3}{3}.
$$

The variance follows by integrating the covariance kernel $\operatorname{cov}(B_r,B_s)=\min(r,s)$ twice.

### Brownian motion transform by three times its running average

↑ **Parent:** [Integral of Brownian motion](#integral-of-brownian-motion)

The displayed continuous centered [Gaussian process](stochastic-process.md#gaussian-process), with value zero at time zero, has the [Brownian covariance kernel](random-variable.md#brownian-covariance-kernel). Hence it is a [Brownian motion](brownian-motion.md) in its own natural filtration. More generally, replacing three by $c$ gives covariance $s+c(c-3)(s/2-s^2/(6t))$ for $0<s\leq t$, so three is the only nonzero valid coefficient. Its conditional future increment in the original Brownian filtration is $3(t-s)t^{-1}(s^{-1}\int_0^sW_u\,du-W_s)$, and is generally nonzero.

## Diffusion coefficient

↑ **Parent:** [Brownian motion](brownian-motion.md)

The diffusion coefficient sets the linear growth of mean-square displacement. In one dimension the convention $\mathbb E[(X_t-X_0)^2]=2Dt$ is common.

### Solutal diffusivity

↑ **Parent:** [Diffusion coefficient](#diffusion-coefficient)

Solutal diffusivity is the [diffusion coefficient](#diffusion-coefficient) governing transport of a dissolved constituent down its [concentration](physics.md#concentration) gradient. For uniform $D$ and a stationary solvent, the [diffusion equation](diffusion-equation.md) is $C_t=D\nabla^2 C$. It need not equal the [thermal diffusivity](thermodynamics.md#thermal-diffusivity).

## Orthogonal invariance of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

If $B$ is Brownian motion in $\mathbb R^d$ and $U$ is an orthogonal matrix, then $UB$ is Brownian motion. Its increments remain independent centered Gaussian vectors and have covariance $(t-s)UIU^T=(t-s)I$.

## Meeting time of two independent Brownian motions

↑ **Parent:** [Brownian motion](brownian-motion.md)

Two independent one-dimensional Brownian motions started at $-a$ and $a$ meet at the first time a Brownian motion started at $\sqrt2a$ hits zero. The meeting time has density

$$
f_T(u)=\frac{a}{\sqrt{\pi u^3}}e^{-a^2/u},
\qquad u>0.
$$

An orthogonal sum coordinate is independent of this hitting time and makes the meeting position conditionally $N(0,u/2)$.

## Wiener measure

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wiener_measure)

Wiener measure is the [probability distribution](probability-theory.md#probability-distribution) of [Brownian motion](brownian-motion.md) on a continuous-path space, usually $C_0([0,T])$ or $C_0([0,\infty))$.

### Wiener theorem

↑ **Parent:** [Wiener measure](#wiener-measure)

There exists a [probability measure](probability-theory.md#probability-measure) on $C_0([0,\infty),\mathbb R)$ under which the coordinate process is standard [Brownian motion](brownian-motion.md), and its distribution there is unique. Construct consistent centered [Gaussian](probability-theory.md#normal-distribution) finite-dimensional laws with [covariance](variance.md#covariance) $\min(s,t)$ and use the [Kolmogorov extension theorem](stochastic-process.md#kolmogorov-extension-theorem). The fourth increment moment $3|t-s|^2$ supplies a continuous modification by the [Kolmogorov continuity theorem](stochastic-process.md#kolmogorov-continuity-theorem). Its [independent increments](stochastic-process.md#independent-increments) and [normal](probability-theory.md#normal-distribution) increment distributions are unchanged. Uniqueness follows because coordinate evaluations at rational times generate the [Borel sigma-algebra](measure-theory.md#borel-sigma-algebra) of continuous-path space.

### Cameron-Martin space of Wiener measure

↑ **Parent:** [Wiener measure](#wiener-measure)

On $C_0([0,T])$, the Cameron-Martin space consists of the [absolutely continuous functions](sobolev-space.md#absolutely-continuous-function) $h$ with $h(0)=0$ and $h'\in L^2[0,T]$. Its norm is

$$
\lVert h\rVert_H^2=\int_0^T|h'(s)|^2ds.
$$

#### Cameron-Martin theorem

↑ **Parent:** [Cameron-Martin space of Wiener measure](#cameron-martin-space-of-wiener-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cameron-Martin_theorem)

Translation of [Wiener measure](#wiener-measure) by a path $h$ is equivalent to Wiener measure exactly when $h$ belongs to the [Cameron-Martin space of Wiener measure](#cameron-martin-space-of-wiener-measure). In that case the density is

$$
\exp\left(\int_0^Th'(s)\,dB_s-\frac12\int_0^T|h'(s)|^2ds\right).
$$

Translation by any continuous path outside that space produces a singular measure.

##### Cameron-Martin shifts on infinite Wiener path space

↑ **Parent:** [Cameron-Martin theorem](#cameron-martin-theorem)

If $h(t)=\int_0^tg_sds$ with deterministic $g\in L^2(0,\infty)$, the finite-time [Cameron-Martin theorem](#cameron-martin-theorem) densities have second moments $e^{\int_0^tg_s^2ds}$ bounded uniformly in time. Their [uniformly integrable martingale](martingale.md#uniformly-integrable-martingale) limit is the strictly positive displayed density, giving equivalence on the full infinite continuous-path space. Finite-time densities alone do not guarantee such a global density: a nonzero constant drift has infinite energy and its infinite-horizon path law is singular, distinguished by the limiting ratio $B_t/t$.

##### Cameron-Martin theorem for a linear drift

↑ **Parent:** [Cameron-Martin theorem](#cameron-martin-theorem)

For the [Cameron-Martin space of Wiener measure](#cameron-martin-space-of-wiener-measure) path $h(s)=\mu s$, the [Cameron-Martin theorem](#cameron-martin-theorem) says that translation of [Brownian motion](brownian-motion.md) by this [linear function](vector-space.md#linear-function) changes its law through time $t$ by the density

$$
\exp\!\left(\mu W_t-\frac12\mu^2t\right).
$$

###### First-passage density of Brownian motion with positive drift

↑ **Parent:** [Cameron-Martin theorem for a linear drift](#cameron-martin-theorem-for-a-linear-drift)

For $\tau_{a,b}=\inf\{t\geq0:B_t+bt=a\}$ with $a,b>0$,

$$
\mathbb P(\tau_{a,b}\in dt)
=\frac{a}{\sqrt{2\pi t^3}}
\exp\left(-\frac{(a-bt)^2}{2t}\right)dt.
$$

The Cameron-Martin likelihood at a driftless path hitting $a$ at time $t$ is $e^{ab-b^2t/2}$.

<h2 id="brownian-holder-regularity">Brownian Hölder regularity</h2>

↑ **Parent:** [Brownian motion](brownian-motion.md)

On every compact time interval, a Brownian path is almost surely a [Hölder continuous function](sobolev-space.md#holder-condition) of every exponent $\alpha<1/2$, and of no exponent $\alpha\geq1/2$. In particular, $B_t=o(t^\gamma)$ as $t\downarrow0$ for every $\gamma<1/2$ after choosing a Hölder exponent strictly between $\gamma$ and $1/2$.

## Brownian zero set

↑ **Parent:** [Brownian motion](brownian-motion.md)

The zero set $\{t\geq0:B_t=0\}$ of one-dimensional [Brownian motion](brownian-motion.md) is almost surely closed, uncountable, and has zero [Lebesgue measure](measure-theory.md#lebesgue-measure). The last fact follows from [Tonelli theorem](measure-theory.md#tonelli-theorem) because $\mathbb P(B_t=0)=0$ for every $t>0$.

## Reflection invariance of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

If $B$ is standard Brownian motion, then $-B$ is also standard Brownian motion. More generally, applying an orthogonal transformation to a multidimensional Brownian motion preserves its law.

## Critical exponential moment of a drifted Brownian hitting time

↑ **Parent:** [Brownian motion](brownian-motion.md)

For $a>0$ and $T_a=\inf\{t\geq0:B_t+t=a\}$,

$$
\mathbb E e^{T_a/2}=e^a.
$$

Changing measure with the density $e^{-B_t-t/2}$ turns $B_t+t$ into Brownian motion. At $T_a$ the density equals $e^{-a+T_a/2}$, and Brownian motion hits $a$ almost surely.

## Bessel process

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bessel_process)

A Bessel process of dimension $d$ is the radial part of $d$-dimensional [Brownian motion](brownian-motion.md). Away from zero it solves the [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation)

$$
dR_t=\frac{d-1}{2R_t}\,dt+dW_t.
$$

This equation also defines noninteger dimensions through its [weak solutions](partial-differential-equation.md#weak-solution).

### Two-dimensional Bessel transition law

↑ **Parent:** [Bessel process](#bessel-process)

A dimension-two [Bessel process](#bessel-process) starting at $r>0$ has the displayed marginal law, where $G_1,G_2$ are independent standard [normal random variables](probability-theory.md#gaussian-random-variable). Take the norm of a [planar Brownian motion](#planar-brownian-motion) starting at $(r,0)$. [Planar Brownian motion avoids a fixed point](#planar-brownian-motion-avoids-a-fixed-point), so the norm stays positive; [Itô formula](stochastic-calculus.md#ito-s-lemma) gives drift $1/(2R)$ and a martingale term of bracket $t$. The [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion) identifies that term as its driving Brownian motion. The squared radius divided by $t$ has a [noncentral chi-squared distribution](probability-theory.md#noncentral-chi-squared-distribution) with two degrees of freedom and noncentrality $r^2/t$.

### Squared Bessel process

↑ **Parent:** [Bessel process](#bessel-process)

A squared Bessel process of dimension $\delta\ge0$ is a nonnegative continuous solution of the displayed [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation). It extends the squared radial part of integer-dimensional [Brownian motion](brownian-motion.md) to arbitrary nonnegative dimensions. Before hitting zero its square root solves $dR=dB+(\delta-1)(2R)^{-1}dt$. At dimension zero, a process started at zero remains there. The coefficients are not Lipschitz at zero, so positivity or uniqueness must not be justified by a global Lipschitz theorem.

#### Additivity of independently driven squared Bessel processes

↑ **Parent:** [Squared Bessel process](#squared-bessel-process)

For independently driven nonnegative [squared Bessel processes](#squared-bessel-process) $X,Y$, put $Z=X+Y$. Where $Z>0$, use Brownian weights $\sqrt{X/Z}$ and $\sqrt{Y/Z}$. Where $Z=0$, fill the weights with $(1,0)$. Their squared norm is always one and their cross-variation is zero, so their stochastic integral is [Brownian motion](brownian-motion.md) by the [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion). Multiplying by $2\sqrt Z$ recovers the sum's martingale part even at zero, and the drifts add to $\alpha+\beta$.

### Oppositely driven Bessel exit probability

↑ **Parent:** [Bessel process](#bessel-process)

For $0<a<1/2$, couple $dX=dB+aX^{-1}dt$ and $dY=-dB+aY^{-1}dt$ from positive $x,y$, killing each at zero. Their sum has no Brownian term and increases, so simultaneous extinction is impossible. The ratio $U=Y/(X+Y)$ has time-changed generator $\frac12\partial_u^2+a(1-2u)[u(1-u)]^{-1}\partial_u$. Its scale density is $u^{-2a}(1-u)^{-2a}$, integrable at both endpoints. Optional stopping of its normalized scale function at the first extinction gives the displayed regularized [incomplete beta function](complex-analysis.md#incomplete-beta-function). At $a=1/3$ this is [Cardy's formula](stochastic-process.md#cardy-boundary-crossing-formula).

### Truncation construction of a positive Bessel strong solution

↑ **Parent:** [Bessel process](#bessel-process)

For $0<\varepsilon<x$, the drift $g_\varepsilon(y)=a/(y\vee\varepsilon)$ is globally Lipschitz and bounded. Solve its equation strongly for the prescribed [Brownian motion](brownian-motion.md), and stop at the first hit of $\varepsilon$. Local uniqueness makes these stopped solutions agree up to the larger threshold; their [stopping times](martingale.md#stopping-time) increase as the threshold decreases. With $\nu=2a-1>0$, Itô's formula for $X^{-\nu}$ gives $\mathbb P(T_\varepsilon\leq t)\leq(\varepsilon/x)^\nu$ on every finite horizon. Hence the patched lifetime is infinite. Localization away from zero proves [pathwise uniqueness](stochastic-calculus.md#pathwise-uniqueness) of the positive global solution. Uniqueness before a [stopping time](martingale.md#stopping-time) refers to the stopped solution, not to arbitrary unconstrained continuations afterward.

### Three-dimensional Bessel process

↑ **Parent:** [Bessel process](#bessel-process)

The radial part of three-dimensional [Brownian motion](brownian-motion.md) started away from the origin is a [Bessel process](#bessel-process) of dimension three. The radial [Laplacian](calculus.md#laplacian) is $\Delta|x|=2/|x|$, so the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives the displayed equation. The radial martingale has unit [quadratic variation](stochastic-calculus.md#quadratic-variation) rate and is [Brownian motion](brownian-motion.md) by the [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion). The reciprocal $1/R$ is a [local martingale](martingale.md#local-martingale). Stopping it on $(\varepsilon,M)$ gives $\mathbb P_x(T_\varepsilon<T_M)=\varepsilon(M-x)/(x(M-\varepsilon))$. Letting $\varepsilon\downarrow0$ shows that zero is not hit.

#### Logarithmic escape rate of three-dimensional Brownian motion

↑ **Parent:** [Three-dimensional Bessel process](#three-dimensional-bessel-process)

For $W$ started at a point of radius one, its radial process has the law of the inverse-clock process $e^{B_{J_t}+J_t/2}$, where $J$ inverts $H_s=\int_0^se^{2B_r+r}dr$. The [logarithmic growth of an exponential Brownian clock with positive drift](#logarithmic-growth-of-an-exponential-brownian-clock-with-positive-drift) gives $\log H_s/s\to1$, whereas $\log(e^{B_s+s/2})/s\to1/2$. Substituting $s=J_t$ proves the displayed almost sure escape rate and divergence of the radius. Independently, [Brownian scaling](#brownian-scaling) gives the same rate in probability; if an almost sure logarithmic rate is already known to exist, that identifies its value.

### Beta integral for strict ordering of coupled Bessel lifetimes

↑ **Parent:** [Bessel process](#bessel-process)

Couple $dX=dB+aX^{-1}dt$ and $dY=dB+aY^{-1}dt$ from $0<x<y$, with $1/4<a<1/2$. Suppose their finite lifetimes end at zero and $\int_0^{\sigma_y}Y_t^{-2}dt=\infty$. Their difference is positive and has derivative $-a(Y-X)/(XY)$, so $\sigma_x\leq\sigma_y$. For $\Theta=(Y-X)/Y$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives

$$
d\Theta=-\Theta Y^{-1}dB+\Theta Y^{-2}\left(1-a-\frac a{1-\Theta}\right)dt.
$$

The normalized [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) $I_\Theta(4a-1,1-2a)$ is a bounded [local martingale](martingale.md#local-martingale). Its finite [quadratic variation](stochastic-calculus.md#quadratic-variation) and the divergent $Y^{-2}$ clock force $\Theta\to0$ on simultaneous extinction; on strict extinction $\Theta\to1$. Its terminal value is therefore the strict-extinction indicator, proving the formula by [optional sampling theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale). For [SLE](stochastic-process.md#schramm-loewner-evolution) boundary images, $a=2/\kappa$; this compares strict and simultaneous [boundary swallowing times](stochastic-process.md#boundary-point-swallowing-time-for-a-loewner-chain) for $4<\kappa<8$.

### Reciprocal three-dimensional Bessel strict local martingale

↑ **Parent:** [Bessel process](#bessel-process)

For a three-dimensional [Bessel process](#bessel-process) started at one, $R$ stays strictly positive and satisfies $dR=dW+R^{-1}dt$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) makes its reciprocal a [local martingale](martingale.md#local-martingale), but $\mathbb E[R_t^{-1}]=2\Phi(1/\sqrt t)-1<1$ for $t>0$. Thus the reciprocal is a [strict local martingale](martingale.md#strict-local-martingale). It can deflate the market with constant bank account and stock price $R$ without yielding a true pricing density for the bank account.

### Bessel power local martingale

↑ **Parent:** [Bessel process](#bessel-process)

For a [Bessel process](#bessel-process) of dimension $\delta$, started at $x>0$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives

$$
d(X_t^{2-\delta})=(2-\delta)X_t^{1-\delta}\,dW_t
$$

on its stochastic interval before hitting zero. Thus the power is a [local martingale](martingale.md#local-martingale) after localization away from zero. For $\delta\geq2$ this interval is the whole lifetime; at $\delta=2$ the power is constant. The unqualified assertion fails for a reflecting Bessel process of dimension one, which acquires [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale) at zero.

#### Stopped inverse radial power martingale classification

↑ **Parent:** [Bessel power local martingale](#bessel-power-local-martingale)

For [Brownian motion](brownian-motion.md) started at radius $x>0$, the displayed process is a [continuous local martingale](martingale.md#continuous-local-martingale). It is a bounded true [martingale](martingale.md) when $0<a\leq x$, but a [strict local martingale](martingale.md#strict-local-martingale) when $a=0$ or $a>x$. In the latter case the boundary is outside the starting point, so stopping does not remove the singularity at the origin. Brownian scaling gives $\mathbb E\|B_t\|^{2-d}=O(t^{-(d-2)/2})$; when $a>x$, the stopped expectation tends to $a^{2-d}<x^{2-d}$.

#### All-time minimum of a transient Bessel process

↑ **Parent:** [Bessel power local martingale](#bessel-power-local-martingale)

For a [Bessel process](#bessel-process) of dimension $\delta>2$ started at $x>0$, its [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) gives $\mathbb P_x(\tau_r<\infty)=(r/x)^{\delta-2}$ for $0<r<x$. In particular, $\inf_{t\geq0}X_t>0$ almost surely. The minimum is attained because the process tends to infinity; the hitting formula alone already implies positivity of the infimum.

### Hitting-zero classification for a Bessel process

↑ **Parent:** [Bessel process](#bessel-process)

A [Bessel process](#bessel-process) of dimension $d>0$ started away from zero hits zero almost surely exactly when $d<2$. For $d\ne2$, its [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) is $s(x)=x^{2-d}$; for $d=2$ it is $s(x)=\log x$. The [boundary hitting probability from a diffusion scale function](stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function) then gives the classification by taking the inner boundary to zero and the outer boundary to infinity.

#### Finite-time access to zero for Bessel dimensions below two

↑ **Parent:** [Hitting-zero classification for a Bessel process](#hitting-zero-classification-for-a-bessel-process)

For $dX=dB+aX^{-1}dt$, put $\gamma=1-2a\in(0,1)$ and $v_R(x)=(R^{2-\gamma}x^\gamma-x^2)/(1+2a)$. It is nonnegative on $[0,R]$, vanishes at both endpoints and solves $\frac12v_R''+(a/x)v_R'=-1$ on $(0,R)$. Optional stopping at $T_\varepsilon\wedge T_R$ gives $\mathbb E(T_\varepsilon\wedge T_R)\leq v_R(x)$ uniformly as $\varepsilon\downarrow0$. Thus the limiting exit to zero or $R$ occurs in finite time, not merely as an asymptotic approach to zero. Scale probabilities give $\mathbb P_x(T_0<T_R)=1-(x/R)^\gamma$; letting $R\to\infty$ gives almost sure finite hitting of zero.

### Scaling invariance of a Bessel process

↑ **Parent:** [Bessel process](#bessel-process)

If $X$ is a Bessel process of dimension $d$ started at $x$ and $r>0$, then

$$
(rX_{t/r^2})_{t\geq0}
$$

is a Bessel process of dimension $d$ started at $rx$. This follows from [Brownian scaling](#brownian-scaling) in the stochastic differential equation and [uniqueness in law](stochastic-calculus.md#uniqueness-in-law).

### Exponential Brownian-to-Bessel time change

↑ **Parent:** [Bessel process](#bessel-process)

For $Z_t=e^{B_t+at}$, use the clock $C_t=\int_0^tZ_s^2ds$. After the inverse time change, the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) gives

$$
dZ_{\tau_u}=dW_u+\frac{a+1/2}{Z_{\tau_u}}du,
$$

so the time-changed process is a [Bessel process](#bessel-process) of dimension $d=2a+2$. Its lifetime is $C_\infty$, which is finite almost surely exactly when $d<2$.

#### Logarithmic growth of an exponential Brownian clock with positive drift

↑ **Parent:** [Exponential Brownian-to-Bessel time change](#exponential-brownian-to-bessel-time-change)

The [strong law for Brownian motion](#strong-law-for-brownian-motion) gives $B_s/s\to0$. For every $0<\varepsilon<\mu$, eventually $e^{(2\mu-2\varepsilon)s}\leq e^{2B_s+2\mu s}\leq e^{(2\mu+2\varepsilon)s}$. Integrating these bounds, taking logarithms and dividing by $t$ squeezes the growth rate between $2\mu-2\varepsilon$ and $2\mu+2\varepsilon$. Let $\varepsilon\downarrow0$. The corresponding inverse clock grows like $(\log t)/(2\mu)$.

### Power time change of a Bessel process

↑ **Parent:** [Bessel process](#bessel-process)

If $X$ is a Bessel process of dimension $d$ and $\alpha>0$, then $X^\alpha$, after the clock $\alpha^2\int X_s^{2\alpha-2}ds$, is a Bessel process of dimension

$$
d'=2+\frac{d-2}{\alpha}.
$$

## Reflected Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflected_Brownian_motion)

One-dimensional reflected Brownian motion on $[0,\infty)$ has the same law as $|B_t|$. The [Tanaka formula](stochastic-calculus.md#tanaka-s-formula) represents it as a Brownian motion plus a nondecreasing [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale) that grows only at zero.

### Reflected Brownian motion with negative drift

↑ **Parent:** [Reflected Brownian motion](#reflected-brownian-motion)

Apply the [Skorokhod reflection map on the half-line](stochastic-process.md#skorokhod-reflection-map-on-the-half-line) to [Brownian motion](brownian-motion.md) with negative constant [drift](stochastic-calculus.md#drift-coefficient) and positive variance parameter $\sigma^2$. The result is kept nonnegative by a regulator acting only at zero. It has a [stationary distribution](markov-process.md#stationary-distribution), unlike zero-drift reflection on the whole half-line.

#### Stationary law of negatively drifted reflected Brownian motion

↑ **Parent:** [Reflected Brownian motion with negative drift](#reflected-brownian-motion-with-negative-drift)

The stationary law is the law of $\sup_{t\ge0}(\sigma B(t)-dt)$. Let $\kappa=2d/\sigma^2$. The [Exponential martingale for Brownian motion](#exponential-martingale-for-brownian-motion) $e^{\kappa(\sigma B_t-dt)}$, stopped on first hitting $b$, is bounded by $e^{\kappa b}$. On no hitting, the driving path tends to minus infinity. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) and [optional stopping](martingale.md#optional-sampling-theorem-for-a-supermartingale) therefore give $1=e^{\kappa b}\mathbb P(\text{hit }b)$. The reflected process started at zero converges to this supremum law: its value at time $t$ has the law of the driving path's maximum up to $t$, by reversing the increments. The resulting density is $(2d/\sigma^2)e^{-2dx/\sigma^2}$ for $x\ge0$.

## Brownian occupation time

↑ **Parent:** [Brownian motion](brownian-motion.md)

The occupation time of a measurable set $A$ through time $t$ is $\int_0^t\mathbf1_{\{B_s\in A\}}ds$. The [occupation-times formula](#occupation-times-formula) expresses such integrals through [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale). Recurrence and the [Strong Markov property](markov-process.md#strong-markov-property) imply that one-dimensional Brownian motion spends an unbounded total time in every nonempty open interval.

### Infinite occupation time of one-dimensional Brownian motion

↑ **Parent:** [Brownian occupation time](#brownian-occupation-time)

A one-dimensional [Brownian motion](brownian-motion.md) spends an infinite total time in every nonempty open interval [almost surely](convergence-of-random-variables.md#almost-sure-convergence). To prove this for $(-1,1)$ after first hitting zero, alternate exits from that interval with returns to zero. By [recurrence of one-dimensional Brownian motion](#recurrence-of-one-dimensional-brownian-motion) all these [stopping times](martingale.md#stopping-time) are finite, and the [Strong Markov property](markov-process.md#strong-markov-property) makes the successive exit durations [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) that are strictly positive. Some fixed positive duration is exceeded with positive probability, so the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) makes the sum of the durations infinite. Translate and scale for other intervals. In particular, if a nonnegative function is bounded below by a positive constant on such an interval, its infinite-horizon [Brownian occupation time](#brownian-occupation-time) integral diverges. Recurrent visits alone, without this duration argument, would not prove divergence of an integral.

#### Divergence of a driftless Brownian exponential clock

↑ **Parent:** [Infinite occupation time of one-dimensional Brownian motion](#infinite-occupation-time-of-one-dimensional-brownian-motion)

For any real constant $c$, one-dimensional [Brownian motion](brownian-motion.md) repeatedly returns to zero. Consider successive segments from zero until exiting $(-1,1)$, separated by returns to zero. Their capped durations are independent identically distributed positive bounded random variables by the [Strong Markov property](markov-process.md#strong-markov-property), so their sum diverges by the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers). On each such segment $e^{cB_s}\geq e^{-|c|}$. Thus the exponential clock has infinite lifetime, despite arbitrarily deep negative excursions.

### Occupation-times formula

↑ **Parent:** [Brownian occupation time](#brownian-occupation-time)

For a continuous semimartingale $X$ with [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale) $L_t^a(X)$,

$$
\int_0^tf(X_s)d[X]_s=\int_{\mathbb R}f(a)L_t^a(X)da
$$

for every nonnegative measurable function $f$.

## Planar Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

Planar Brownian motion is the random vector $(B_t^{(1)},B_t^{(2)})$ formed from two independent standard one-dimensional Brownian motions.

### Area of a planar Brownian path

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

A [planar Brownian motion](#planar-brownian-motion) range has zero two-dimensional [Lebesgue measure](measure-theory.md#lebesgue-measure) almost surely. Assuming finite expected area, [Brownian scaling](#brownian-scaling) gives half that expected area for each half-time range. Inclusion-exclusion then makes their expected overlap zero. Translate their ranges by the midpoint position; the [independent Brownian arms at a deterministic time](#independent-brownian-arms-at-a-deterministic-time) make the expected overlap the integral of the squared point-hitting [probabilities](probability-theory.md#probability) for a half-time range. Those [probabilities](probability-theory.md#probability) vanish almost everywhere, so the half-time expected area, and hence the full-time expected area, vanish. This argument does not assert zero hitting [probability](probability-theory.md#probability) for every individual point solely from an almost-everywhere integral conclusion.

### Logarithmic radius of planar Brownian motion

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

Started at radius one, [planar Brownian motion](#planar-brownian-motion) avoids the origin, and its logarithmic radius is a [continuous local martingale](martingale.md#continuous-local-martingale) because the logarithmic potential is harmonic away from zero. It is a [strict local martingale](martingale.md#strict-local-martingale): at deterministic $t>0$, the [angular average of a logarithmic potential](partial-differential-equation.md#angular-average-of-a-logarithmic-potential) gives $\mathbb E\log|B_t|=\int_1^\infty e^{-r^2/(2t)}\,dr/r>0$, whereas the initial value is zero. Absolute integrability follows from integrability of $r|\log r|$ near zero and the Gaussian tail. Its positive [expectation](probability-theory.md#expected-value) does not contradict nonnegative-local-martingale bounds, since this process takes both signs.

#### Winding at logarithmic radial passage levels

↑ **Parent:** [Logarithmic radius of planar Brownian motion](#logarithmic-radius-of-planar-brownian-motion)

For [planar Brownian motion](#planar-brownian-motion) started at $1$, continuous winding angles sampled at the displayed radii have independent stationary increments. At $T_r$, apply the [Strong Markov property](markov-process.md#strong-markov-property), rotate by the current angle, and rescale space by $e^r$ and time by $e^{-2r}$. The future radial-level winding increment has the original law and is independent of the past. The logarithmic radius and winding angle are independent Brownian coordinates on the common clock $\int|B_s|^{-2}ds$. At radial passage they are therefore $U_{\eta_r}=-r$ and $V_{\eta_r}$, where $\eta_r$ is a [Brownian first-passage time](markov-process.md#brownian-first-passage-time). Its [Laplace transform](analysis.md#laplace-transform) gives the displayed characteristic function. The level process is a symmetric [Cauchy process](stochastic-process.md#cauchy-process); replacing the passage clock by its right-continuous version supplies a [càdlàg](calculus.md#cadlag) modification without changing any fixed-level law.

### Planar Brownian stochastic area

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

For independent coordinate Brownian motions, the stochastic area with the stated orientation is $Z_t=\int_0^tY_s\,dX_s-X_s\,dY_s$. Its bracket is $\int_0^t(X_s^2+Y_s^2)\,ds$. Reversing orientation changes its sign but not its law or quadratic variation.

#### Orthogonality of the radial martingale and planar Brownian area

↑ **Parent:** [Planar Brownian stochastic area](#planar-brownian-stochastic-area)

The radial martingale $H=\int X\,dX+Y\,dY$ and the [planar Brownian stochastic area](#planar-brownian-stochastic-area) $Z=\int Y\,dX-X\,dY$ have common bracket $A=\int(X^2+Y^2)ds$ and zero cross variation, because their integrand vectors $(X,Y)$ and $(Y,-X)$ are orthogonal. The Itô formula also gives $X_t^2+Y_t^2=2H_t+2t$.

##### Common-clock Brownian representation of radius and area

↑ **Parent:** [Orthogonality of the radial martingale and planar Brownian area](#orthogonality-of-the-radial-martingale-and-planar-brownian-area)

Jointly time-change the radial and area martingales by the inverse of $A=\int R^2ds$. The bracket matrix becomes $uI_2$, so the [Lévy characterization of multidimensional Brownian motion](#levy-characterization-of-multidimensional-brownian-motion) gives two independent Brownian coordinates. The clock is strictly increasing; if it were finite at infinity, the radial martingale would converge and $R_t^2=2t+O(1)$ would force its integral to diverge. Thus $R_t^2=2W_{A(t)}+2t$ and $Z_t=B_{A(t)}$ with $W,B$ independent.

### Brownian excursion in the upper half-plane

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

The excursion from $0$ to infinity is the [Doob h-transform](markov-process.md#doob-h-transform) of killed [planar Brownian motion](#planar-brownian-motion) with $h(z)=\operatorname{Im}z$, using the entrance law at zero. Equivalently, its real part is a standard [Brownian motion](brownian-motion.md) and its independent imaginary part is a [Bessel process](#bessel-process) of dimension three started at zero. This planar, infinite-duration excursion differs from the one-dimensional excursion on a finite time interval.

#### Restriction probability of a Brownian half-plane excursion

↑ **Parent:** [Brownian excursion in the upper half-plane](#brownian-excursion-in-the-upper-half-plane)

For a [compact H-hull](stochastic-process.md#compact-h-hull) avoiding zero, let $\psi_A$ map its complement to the half-plane, fix zero, and have derivative one at infinity. The [Brownian excursion in the upper half-plane](#brownian-excursion-in-the-upper-half-plane) avoids $A$ with probability $\psi_A'(0)$. From an interior starting point $z$, the corresponding transformed process avoids $A$ with probability $\operatorname{Im}g_A(z)/\operatorname{Im}z$; taking $z=i\varepsilon$ and $\varepsilon\downarrow0$ gives the boundary derivative.

##### Boundary derivative is an excursion avoidance probability

↑ **Parent:** [Restriction probability of a Brownian half-plane excursion](#restriction-probability-of-a-brownian-half-plane-excursion)

For a [compact H-hull](stochastic-process.md#compact-h-hull) $A$ whose closure avoids a real boundary point $x$, the [Brownian excursion in the upper half-plane](#brownian-excursion-in-the-upper-half-plane) from $x$ to infinity avoids $A$ with the displayed probability. From an interior point $z$, the corresponding [Doob h-transform](markov-process.md#doob-h-transform) avoidance probability is $\operatorname{Im}g_A(z)/\operatorname{Im}z$. Letting $z=x+i\varepsilon$ approach the boundary and using the [Schwarz reflection principle](complex-analysis.md#schwarz-reflection-principle) gives the derivative. In particular $0<g_A'(x)\leq1$ at every regular real boundary point away from the hull.

### Conformal invariance of planar Brownian motion

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

If $B$ is planar [Brownian motion](brownian-motion.md) in a domain $D$ and $f:D\to D'$ is a nonconstant [holomorphic function](complex-analysis.md#holomorphic-function), then $f(B)$, run with the clock $\int_0^t|f'(B_s)|^2ds$, is planar Brownian motion in $D'$ until the relevant exit time. In particular, [conformal maps](geometry-and-topology.md#conformal-map) transport [harmonic measure](#harmonic-measure) between planar domains.

#### Small-radius Brownian winding law

↑ **Parent:** [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)

For planar [Brownian motion](brownian-motion.md) started at radius $\varepsilon$ and stopped on first hitting radius one, the net winding count divided by $\log\varepsilon$ converges to a standard [Cauchy random variable](probability-theory.md#cauchy-random-variable) divided by $2\pi$. The complex exponential maps Brownian coordinates in the left half-plane to the punctured unit disk after the [conformal Brownian clock](#conformal-brownian-clock). The unwrapped argument at exit is the vertical half-plane exit coordinate, with the [Cauchy exit law from a Brownian half-plane](#cauchy-exit-law-from-a-brownian-half-plane). Counting integer turns introduces only a uniformly bounded error in winding units.

#### Cauchy exit law from a Brownian half-plane

↑ **Parent:** [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)

Planar [Brownian motion](brownian-motion.md) started at $(-x,0)$ exits the left half-plane with ordinate distributed as $x$ times a standard [Cauchy random variable](probability-theory.md#cauchy-random-variable). Conditional on the independent horizontal hitting time, the ordinate is normal with variance equal to that time. The [inverse-square Gaussian law of Brownian first passage](markov-process.md#inverse-square-gaussian-law-of-brownian-first-passage) turns this into a ratio of independent standard normals. Its exit density is $x/(\pi(x^2+y^2))$.

#### Complex exponential construction of planar Brownian motion

↑ **Parent:** [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)

For independent one-dimensional [Brownian motions](brownian-motion.md) $\beta,\theta$, the real and imaginary parts of $Z$ are continuous local martingales with equal bracket $A$ and zero cross bracket. The [Divergence of a driftless Brownian exponential clock](#divergence-of-a-driftless-brownian-exponential-clock) makes $A_\infty=\infty$, and the [common-clock time change of orthogonal local martingales](martingale.md#common-clock-time-change-of-orthogonal-local-martingales) makes $Z_{A^{-1}(r)}$ planar Brownian motion started at $1$. The exponential never vanishes, proving that this Brownian motion never hits zero. Recurrent visits of $\beta$ to arbitrarily negative levels prove visits arbitrarily near zero at arbitrarily large Brownian times.

#### Power-map reduction for Brownian exit from a wedge

↑ **Parent:** [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)

The map $z\mapsto z^{\pi/\alpha}$ takes a wedge of opening $\alpha$ to a half-plane and the circular boundary of radius $r$ to radius $r^{\pi/\alpha}$. [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion) preserves which boundary part is reached first, although it changes the clock. Use the branch defined by the wedge argument; the origin is a [polar point for planar Brownian motion](#polar-point-for-planar-brownian-motion), so localization handles the vertex.

##### Brownian wedge-exit probability

↑ **Parent:** [Power-map reduction for Brownian exit from a wedge](#power-map-reduction-for-brownian-exit-from-a-wedge)

A [planar Brownian motion](#planar-brownian-motion) starting at $1$ exits the disk of radius $r>1$ before leaving a wedge of opening $\alpha\in(0,2\pi]$, centered on the positive axis, with probability $(4/\pi)\arctan(r^{-\pi/\alpha})$. The [power-map reduction for Brownian exit from a wedge](#power-map-reduction-for-brownian-exit-from-a-wedge), the [reflection identity for Brownian exit from a half-disc](#reflection-identity-for-brownian-exit-from-a-half-disc) and the [Möbius calculation of circular Brownian exit](#mobius-calculation-of-circular-brownian-exit) give the formula. Its large-radius decay exponent is $\pi/\alpha$.

#### Conformal Brownian clock

↑ **Parent:** [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)

For a [conformal bijection](complex-analysis.md#biholomorphism) $\phi$ and [planar Brownian motion](#planar-brownian-motion) $B$, this increasing clock measures the common [quadratic variation](stochastic-calculus.md#quadratic-variation) of the two coordinates of $\phi(B)$. The transformed Brownian path is $\phi(B_{A^{-1}(t)})$. The inverse clock runs from image time to original time.

##### Finite exit from a conformal image of a bounded planar domain

↑ **Parent:** [Conformal Brownian clock](#conformal-brownian-clock)

A [planar Brownian motion](#planar-brownian-motion) exits a conformal image of a bounded planar domain in finite time [almost surely](convergence-of-random-variables.md#almost-sure-convergence). If the image lifetime were infinite, the inverse derivative is bounded away from zero on a small interior disc. [Recurrence of planar Brownian motion](#recurrence-of-planar-brownian-motion) and the [Strong Markov property](markov-process.md#strong-markov-property) give infinite [Brownian occupation time](#brownian-occupation-time) there, forcing the inverse [conformal Brownian clock](#conformal-brownian-clock) to diverge. It cannot exceed the finite original exit time. The expected image exit time can nevertheless be infinite.

### Rotational invariance of planar Brownian motion

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

Applying any fixed orthogonal transformation to planar Brownian motion produces another planar Brownian motion. In particular, rotationally invariant initial data produce rotationally invariant hitting distributions.

### Recurrence of planar Brownian motion

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

Planar Brownian motion almost surely visits every neighborhood of every point. Equivalently, it hits every disc almost surely, although it does not hit any prescribed point with positive probability.

#### Polar point for planar Brownian motion

↑ **Parent:** [Recurrence of planar Brownian motion](#recurrence-of-planar-brownian-motion)

A prescribed point is almost surely never visited by [planar Brownian motion](#planar-brownian-motion) started elsewhere. The [harmonic function](partial-differential-equation.md#harmonic-function) $\log|z-w|$ gives an annular hitting probability that tends to zero as the inner radius decreases to zero. This does not contradict [recurrence of planar Brownian motion](#recurrence-of-planar-brownian-motion), which concerns neighbourhoods.

#### Divergence of a positive planar Brownian occupation integral

↑ **Parent:** [Recurrence of planar Brownian motion](#recurrence-of-planar-brownian-motion)

If $f$ is a continuous probability density on $\mathbb R^2$ and $B$ is planar [Brownian motion](brownian-motion.md), then

$$
\int_0^tf(B_s)\,ds\longrightarrow\infty
$$

almost surely. The density is bounded below on some disc, recurrence supplies infinitely many visits to a smaller concentric disc, and the [Strong Markov property](markov-process.md#strong-markov-property) gives infinitely many visits of a fixed positive duration.

### Brownian reflection coupling

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)

To couple Brownian motions starting at points exchanged by reflection in a hyperplane, reflect one path until the first path hits that hyperplane and then make the paths agree. Reflection invariance and the strong Markov property give the correct marginal laws.

### Harmonic measure

↑ **Parent:** [Planar Brownian motion](#planar-brownian-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_measure)

The harmonic measure of a boundary set $A\subseteq\partial D$ viewed from $x\in D$ is the probability that Brownian motion started at $x$ first exits $D$ through $A$. As a function of $x$, it is harmonic in $D$.

#### Brownian exit law from a quadrant

↑ **Parent:** [Harmonic measure](#harmonic-measure)

Planar [Brownian motion](brownian-motion.md) started at $a+ia$, $a>0$, exits the positive quadrant through either positive coordinate axis with [probability](probability-theory.md#probability) one-half. The density along each axis is $q_a(r)$ for $r>0$, measured with respect to distance along that axis. Squaring maps the quadrant to the upper half-plane and sends the starting point to $2ia^2$. The boundary square therefore has the centered [Cauchy distribution](probability-theory.md#cauchy-distribution) of scale $2a^2$; pulling it back by $r\mapsto r^2$ gives the displayed density. The radius has distribution function $2\arctan(r^2/(2a^2))/\pi$, independently of which axis is chosen. There is no atom at the origin.

#### Harmonic capacity from infinity in the upper half-plane

↑ **Parent:** [Harmonic measure](#harmonic-measure)

This capacity measures the asymptotic probability that [planar Brownian motion](#planar-brownian-motion) hits a [compact H-hull](stochastic-process.md#compact-h-hull) before the real axis. It scales linearly with length and is distinct from [half-plane capacity](stochastic-process.md#half-plane-capacity). A vertical slit of height $h$ has capacity $2h$; a half-disc of radius $r$ has capacity $4r$. Monotonicity of Brownian hitting probabilities gives $\operatorname{cap}(K)\le4\operatorname{rad}(K)$, where the radius is that of the least real-centred enclosing half-disc. For finite slit hulls the capacity is the length of the image of the two-sided absorbing boundary under the [mapping-out function](stochastic-process.md#mapping-out-function-of-a-compact-h-hull).

##### Reflection lower bound for harmonic hull capacity

↑ **Parent:** [Harmonic capacity from infinity in the upper half-plane](#harmonic-capacity-from-infinity-in-the-upper-half-plane)

For a connected slit joining $0$ to $x+iy$ with $x^2+y^2=1$, reflect across the vertical line through $x$. The two slits separate the vertical segment below the common tip and the intervening real boundary from infinity. Brownian reflection symmetry bounds the corresponding model hitting probability by twice the original hull-hitting probability. Mapping out the vertical segment gives total boundary-image length $1+y$ for its two banks together with the real interval between $0$ and $x$. The [harmonic-measure asymptotic at infinity](#harmonic-measure-asymptotic-at-infinity) gives the displayed bound. This argument requires a separating connected barrier; [radius gives no positive lower bound for disconnected harmonic hull capacity](#radius-gives-no-positive-lower-bound-for-disconnected-harmonic-hull-capacity).

##### Radius gives no positive lower bound for disconnected harmonic hull capacity

↑ **Parent:** [Harmonic capacity from infinity in the upper half-plane](#harmonic-capacity-from-infinity-in-the-upper-half-plane)

For $c=\sqrt{1-\varepsilon^2}$, three vertical slits of height $\varepsilon$ rooted at $-c,0,c$ form a [compact H-hull](stochastic-process.md#compact-h-hull) of enclosing radius one. [Subadditivity of harmonic hull capacity](#subadditivity-of-harmonic-hull-capacity) gives capacity at most $6\varepsilon$, which can tend to zero. Thus a uniform lower bound requires additional geometric hypotheses.

##### Subadditivity of harmonic hull capacity

↑ **Parent:** [Harmonic capacity from infinity in the upper half-plane](#harmonic-capacity-from-infinity-in-the-upper-half-plane)

When a finite union is a [compact H-hull](stochastic-process.md#compact-h-hull), hitting that union before the real axis implies hitting at least one member before the real axis. The [union bound](probability-inequality.md#boole-s-inequality) followed by the defining limit proves subadditivity of [harmonic capacity from infinity in the upper half-plane](#harmonic-capacity-from-infinity-in-the-upper-half-plane).

#### Harmonic-measure asymptotic at infinity

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For a [compact H-hull](stochastic-process.md#compact-h-hull) and a Borel subset of the [intrinsic boundary of a simply connected domain](geometry-and-topology.md#intrinsic-boundary-of-a-simply-connected-domain), [hydrodynamic normalization at infinity](stochastic-process.md#hydrodynamic-normalization-at-infinity) and the [Poisson kernel for the upper half-plane](partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) give this limit as $y\to\infty$ with $x/y\to0$. After multiplying the kernel by $\pi y$, it tends pointwise to one and is eventually uniformly bounded. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) proves the finite-measure case and [Fatou's lemma](measure-theory.md#fatou-s-lemma) proves the infinite-measure case.

<h4 id="mobius-calculation-of-circular-brownian-exit">Möbius calculation of circular Brownian exit</h4>

↑ **Parent:** [Harmonic measure](#harmonic-measure)

A [planar Brownian motion](#planar-brownian-motion) beginning at $a\in(0,1)$ in the [unit disc](topology.md#unit-disc) has circular exit law obtained by pulling back uniform angular measure through $\psi_a(w)=(w-a)/(1-aw)$. This [Möbius transformation](group-theory.md#mobius-transformation) sends the starting point to zero. The right semicircle maps to an arc with endpoints at angles $\pm(\pi/2+2\arctan a)$, giving positive-half-plane exit probability $1/2+(2/\pi)\arctan a$.

#### Reflection identity for Brownian exit from a half-disc

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For [planar Brownian motion](#planar-brownian-motion) starting on the positive real axis inside a disk, let $T$ be circular exit and $S$ first contact with the imaginary axis. Reflecting the path after $S$ fixes the disk and swaps positive and negative circular exits. The [Strong Markov property](markov-process.md#strong-markov-property) makes their probabilities equal on $S<T$. Therefore $\mathbb P(T<S)=\mathbb P(\operatorname{Re}B_T>0)-\mathbb P(\operatorname{Re}B_T<0)$.

#### Bottom-boundary harmonic measure of a strip

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For [planar Brownian motion](#planar-brownian-motion) started at $x+iy$ in $0<y<\pi$, this is its unconditional exit density on the bottom boundary. Its mass is $1-y/\pi$; the remaining mass $y/\pi$ lies on the top boundary. The [conformal bijection](complex-analysis.md#biholomorphism) $z\mapsto e^z$, the [Poisson kernel for the upper half-plane](partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) and the boundary [Jacobian determinant](calculus.md#jacobian-determinant) derive the formula. Conditional bottom-boundary density requires division by its mass.

#### Upper-half-plane harmonic measure of the positive half-axis

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For planar [Brownian motion](brownian-motion.md) started at $(x,y)$ with $y>0$, the probability that its first hit of the real axis lies in $(0,\infty)$ is

$$
\frac12+\frac1\pi\arctan\frac{x}{y}
=1-\frac1\pi\arg(x+iy).
$$

This is the bounded [harmonic function](partial-differential-equation.md#harmonic-function) in the upper half-plane with boundary values zero on the negative half-axis and one on the positive half-axis.

#### Planar Brownian annulus hitting probability

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For planar Brownian motion started at $x$ with $0<r<|x|<R$,

$$
\mathbb P_x(T_r<T_R)=\frac{\log R-\log|x|}{\log R-\log r}.
$$

This is optional stopping applied to the harmonic function $\log|x|$ on the annulus.

#### Brownian entrance law to a disc from infinity

↑ **Parent:** [Harmonic measure](#harmonic-measure)

For planar Brownian motion started at $iy$, the distribution of its first hit of the closed unit disc converges as $y\to\infty$ to normalized arc length on the unit circle. Inversion maps the exterior disc to the punctured disc and the starting point to $-i/y\to0$, where rotational invariance makes harmonic measure uniform.

## Coordinatewise coalescing coupling of Brownian motions

↑ **Parent:** [Brownian motion](brownian-motion.md)

Two Brownian motions in $\mathbb R^d$ can be coupled by letting corresponding coordinates evolve independently until they meet and then using the same increments in that coordinate. One-dimensional recurrence makes every coordinate meeting time finite almost surely, so the two processes eventually coalesce while each marginal remains Brownian.

## Strong law for Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

For Brownian motion, $B_t/t\to0$ almost surely as $t\to\infty$. Apply the strong law of large numbers to unit-time increments and control the oscillations on the intervening unit intervals.

## Brownian loop measure

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_loop_measure)

Brownian loop measure is a conformally invariant sigma-finite measure on unrooted planar Brownian loops. Taking outer boundaries connects it to conformal-restriction measures on self-avoiding loops.

### Pinned Brownian loop measure at an interior point

↑ **Parent:** [Brownian loop measure](#brownian-loop-measure)

In the unit disc, the relevant pointed [Brownian loop measure](#brownian-loop-measure) is rooted at $0$ and normalized by its conformal deficit: for simply connected $U$ containing $0$, its mass of loops not contained in $U$ is minus the logarithm of the [conformal radius](geometry-and-topology.md#conformal-radius). Its outer-boundary pushforward gives the corresponding pointed simple-loop restriction measure. It is not the full unrooted loop measure or a probability law of a fixed-duration Brownian bridge.

### Conformal restriction measure on simple loops

↑ **Parent:** [Brownian loop measure](#brownian-loop-measure)

A [sigma-finite measure](measure-theory.md#sigma-finite-measure) on [simple closed curves](geometry-and-topology.md#simple-closed-curve) has conformal restriction if restricting to loops in a simply connected domain and then applying a [conformal map](geometry-and-topology.md#conformal-map) agrees with first transporting the domain and restricting there. The usual nontrivial measures are finite on bounded macroscopic cutoff windows and are determined up to normalization by their pointed conformal deficits.

#### Recovery of a loop measure from conformal deficits

↑ **Parent:** [Conformal restriction measure on simple loops](#conformal-restriction-measure-on-simple-loops)

For simple loops surrounding a marked point, containment in two simply connected domains is containment in their intersection component containing that point. Finite deficits therefore determine all finite intersections of avoidance events by [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle). Restrict to finite windows $H_r=\mathbf L_D\setminus\mathbf L_{rD}$ and use the [sigma-finite uniqueness theorem for measures](measure-theory.md#sigma-finite-uniqueness-theorem-for-measures); as $r\downarrow0$ these windows exhaust the pointed loop space. Finiteness of the windows is essential to this argument.

## Nowhere differentiability of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nowhere_differentiability_of_Brownian_motion)

Brownian paths are almost surely nowhere differentiable. An increment over duration $h$ is typically of order $\sqrt h$, so its difference quotient is of order $h^{-1/2}$ rather than approaching a finite limit.

<h2 id="levy-characterization-of-brownian-motion">Lévy characterization of Brownian motion</h2>

↑ **Parent:** [Brownian motion](brownian-motion.md)

A continuous local martingale $M$ with $M_0=0$ is standard Brownian motion exactly when its [quadratic variation](stochastic-calculus.md#quadratic-variation) satisfies $[M]_t=t$.

The characterization asserts that a continuous [local martingale](martingale.md#local-martingale) starting at zero with quadratic variation $t$ is [Brownian motion](brownian-motion.md).

<h3 id="levy-characterization-of-multidimensional-brownian-motion">Lévy characterization of multidimensional Brownian motion</h3>

↑ **Parent:** [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion)

A continuous vector-valued [local martingale](martingale.md#local-martingale) $M$ starting at zero is standard multidimensional [Brownian motion](brownian-motion.md) if its [quadratic covariations](stochastic-calculus.md#quadratic-covariation) satisfy $[M^i,M^j]_t=\delta_{ij}t$. For each deterministic vector $\xi$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) makes $\exp(i\xi\cdot M_t+|\xi|^2t/2)$ a complex [local martingale](martingale.md#local-martingale). Its absolute value is bounded on each finite horizon, so it is a true [martingale](martingale.md). Its [conditional expectation](measure-theory.md#conditional-expectation) identity gives

$$
\mathbb E[e^{i\xi\cdot(M_t-M_s)}\mid\mathcal F_s]=e^{-|\xi|^2(t-s)/2}.
$$

This conditional [characteristic function](probability-theory.md#characteristic-function) identifies a centered [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) with covariance $(t-s)I$, independent of the past. Thus the coordinates are independent [Brownian motions](brownian-motion.md). The converse follows immediately from the standard coordinate [quadratic covariations](stochastic-calculus.md#quadratic-covariation).

## Brownian scaling

↑ **Parent:** [Brownian motion](brownian-motion.md)

For every $c>0$, the process $(c^{-1/2}B_{ct})_{t\geq0}$ is again [Brownian motion](brownian-motion.md).

This is a rescaling invariance of the [Brownian motion](brownian-motion.md) law.

## Recurrence of one-dimensional Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

One-dimensional [Brownian motion](brownian-motion.md) satisfies

$$
\limsup_{t\to\infty}B_t=+\infty,
\qquad
\liminf_{t\to\infty}B_t=-\infty
$$

almost surely. Its continuous path therefore visits every point, including zero, infinitely often.

## Transience of Brownian motion in dimension at least three

↑ **Parent:** [Brownian motion](brownian-motion.md)

Brownian motion in $\mathbb R^d$ is transient for $d\geq3$: its distance from the origin tends to infinity almost surely. In dimension three, the positive local martingale $|B_t|^{-1}$ and [Brownian scaling](#brownian-scaling) give a short proof.

It is a dimension-dependent long-time property of [Brownian motion](brownian-motion.md).

### Brownian sphere-hitting probability in dimension three

↑ **Parent:** [Transience of Brownian motion in dimension at least three](#transience-of-brownian-motion-in-dimension-at-least-three)

For standard three-dimensional [Brownian motion](brownian-motion.md) started at $x$ with $r<|x|<R$,

$$
\mathbb P_x(\tau_r<\tau_R)=\frac{|x|^{-1}-R^{-1}}{r^{-1}-R^{-1}}.
$$

The [harmonic function](partial-differential-equation.md#harmonic-function) $x\mapsto1/|x|$ gives a bounded [stopped martingale](martingale.md#stopped-martingale) in the annulus, so the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) gives the formula. Taking $R\to\infty$ yields $\mathbb P_x(\tau_r<\infty)=r/|x|$ for $|x|>r$. This limit uses path continuity on the finite interval before a hit, rather than assuming transience to prove transience.

#### Last visit to a bounded ball for three-dimensional Brownian motion

↑ **Parent:** [Brownian sphere-hitting probability in dimension three](#brownian-sphere-hitting-probability-in-dimension-three)

For [Brownian motion](brownian-motion.md) started at zero in dimension three, let $\sigma_R$ be its first hit of the sphere of radius $R>r$. The [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) applied to $|B_t|^2-3t$ proves that $\sigma_R$ is finite almost surely. The [Strong Markov property](markov-process.md#strong-markov-property) and the [Brownian sphere-hitting probability in dimension three](#brownian-sphere-hitting-probability-in-dimension-three) then give the displayed return probability. Choose radii $R_m=2^m r$. The return events after $\sigma_{R_m}$ decrease and their probabilities tend to zero. Almost surely one of these exit times is followed by no visit to the closed ball of radius $r$. Apply this to all positive integer $r$ to obtain $|B_t|\to\infty$ almost surely. This gives full [transience of Brownian motion in dimension at least three](#transience-of-brownian-motion-in-dimension-at-least-three), rather than only a positive escape probability.

## Brownian exit time

↑ **Parent:** [Brownian motion](brownian-motion.md)

For a domain $D$, the Brownian exit time is $T_D=\inf\{t\geq0:B_t\notin D\}$. It is a [stopping time](martingale.md#stopping-time), and it has finite expectation when $D$ is bounded.

### Brownian hitting probability of a ball

↑ **Parent:** [Brownian exit time](#brownian-exit-time)

For $d\geq3$ and $|x|>\varepsilon$, stop the [harmonic function](partial-differential-equation.md#harmonic-function) $u(x)=|x|^{2-d}$ at the two boundaries of $\{\varepsilon<|x|<R\}$. Bounded [optional stopping](martingale.md#optional-sampling-theorem-for-a-supermartingale) gives the probability of hitting the inner sphere first as $(u(x)-u(R))/(u(\varepsilon)-u(R))$. Letting $R\to\infty$ gives the displayed formula; a finite hitting path is contained in some finite-radius ball.

#### Small-ball Brownian hitting asymptotic

↑ **Parent:** [Brownian hitting probability of a ball](#brownian-hitting-probability-of-a-ball)

For $d\geq3$, fixed $x\ne0$ and $t>0$, apply [optional stopping](martingale.md#optional-sampling-theorem-for-a-supermartingale) to $u(B_{t\wedge T_\varepsilon})$ with $u(z)=|z|^{2-d}$. The resulting identity is $\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)=u(x)-\mathbb Eu(B_t)+\mathbb E[u(B_t);T_\varepsilon\leq t]$. The last term tends to zero by [integrability](measure-theory.md#integrability) of $u(B_t)$ and the vanishing total hitting probability. The [Newtonian potential of the Brownian heat kernel](diffusion-equation.md#newtonian-potential-of-the-brownian-heat-kernel) identifies the remaining difference.

### Brownian exit-time expectation in an orthant

↑ **Parent:** [Brownian exit time](#brownian-exit-time)

For [independent](random-variable.md#independent-random-variables) coordinates of standard [Brownian motion](brownian-motion.md) and $x_i>0$, the [Brownian reflection principle](#reflection-principle-wiener-process) gives $\mathbb P_x(T>t)=\prod_i[2\Phi(x_i/\sqrt t)-1]$. This is asymptotic to $(2/\pi)^{n/2}\prod_ix_i\,t^{-n/2}$. The [tail integral formula for expectation](probability-theory.md#tail-integral-formula-for-expectation) therefore proves the stated criterion, with logarithmic divergence in dimension two.

### Uniform ball sampling by Brownian stopping

↑ **Parent:** [Brownian exit time](#brownian-exit-time)

For standard [Brownian motion](brownian-motion.md) started at zero, choose an [independent](random-variable.md#independent-random-variables) radius $R$ with $\mathbb P(R\leq s)=(s/r)^n$, $0\leq s\leq r$, and stop on first reaching that radius. [Rotational invariance of Brownian motion](#rotational-invariance-of-brownian-motion) makes the conditional exit position uniform on each sphere. Mixing with radius density $ns^{n-1}/r^n$ gives the uniform [probability distribution](probability-theory.md#probability-distribution) on the ball. In dimension one, the conditional sign has probabilities $1/2,1/2$. The stopped point samples volume measure even though each conditional exit law is supported on a boundary.

#### Brownian exit-time ball averaging identity

↑ **Parent:** [Uniform ball sampling by Brownian stopping](#uniform-ball-sampling-by-brownian-stopping)

Let $g_D(x)=\mathbb E_xT_D$, possibly infinite, and suppose the closed ball $\overline{B(x,r)}$ lies in the open set $D$. A [Strong Markov property](markov-process.md#strong-markov-property) decomposition at an [independent](random-variable.md#independent-random-variables) random-radius exit time, using [uniform ball sampling by Brownian stopping](#uniform-ball-sampling-by-brownian-stopping), gives the displayed identity in the nonnegative extended reals. Indeed the expected exit time from a radius-$s$ ball started at its centre is $s^2/n$, and averaging this against $ns^{n-1}/r^n$ gives $r^2/(n+2)$. The identity gives local integrability whenever $g_D(x)$ is finite.

##### Finiteness propagation of Brownian mean exit times

↑ **Parent:** [Brownian exit-time ball averaging identity](#brownian-exit-time-ball-averaging-identity)

For a connected open set $D$, finiteness of the [Brownian exit time](#brownian-exit-time) [expectation](probability-theory.md#expected-value) at one point implies finiteness everywhere. The [Brownian exit-time ball averaging identity](#brownian-exit-time-ball-averaging-identity) gives integrability on a ball centred at any finite point. Every point of that ball has a smaller centred ball contained in it; the same identity then gives a finite value there. The set of finite points is open. It is also relatively closed: near a limit point in $D$, choose a fixed ball radius smaller than a quarter of its distance to $D^c$ and centre it at a nearby finite point. The limit point lies in that ball and hence is finite. [Connectedness](geometry-and-topology.md#connected-space) completes the proof.

### Brownian exit from an interval

↑ **Parent:** [Brownian exit time](#brownian-exit-time)

For one-dimensional Brownian motion started at zero and $T=\tau_b\wedge\tau_{-a}$ with $a,b>0$,

$$
\mathbb P(B_T=b)=\frac{a}{a+b},
\qquad
\mathbb E[T]=ab.
$$

Optional stopping of $B_t$ and $B_t^2-t$ proves the two identities.

#### Asymmetric Brownian interval-exit transform

↑ **Parent:** [Brownian exit from an interval](#brownian-exit-from-an-interval)

For standard [Brownian motion](brownian-motion.md) started at zero and exit time $T$ from $(-b,a)$, $a,b>0$, stop the two [exponential Brownian martingales](#exponential-brownian-martingale) with parameters $\lambda$ and $-\lambda$. Their stopped values are bounded by $e^{|\lambda|\max(a,b)}$. The [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) and [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) give $e^{\lambda a}p+e^{-\lambda b}q=1$ and $e^{-\lambda a}p+e^{\lambda b}q=1$, where $p,q$ are the discounted upper and lower exit probabilities. Solving gives the displayed formula and $q=\sinh(\lambda a)/\sinh(\lambda(a+b))$. Thus

$$
\mathbb E e^{-\lambda^2T/2}=\frac{\cosh(\lambda(a-b)/2)}{\cosh(\lambda(a+b)/2)}.
$$

At $\lambda=0$, the first ratio has its removable value $b/(a+b)$, and the second equals one. Finiteness of $T$ follows from a uniformly positive one-unit-time chance to leave any fixed bounded interval.

#### Brownian exit-time skeleton

↑ **Parent:** [Brownian exit from an interval](#brownian-exit-from-an-interval)

Successive exits from intervals of radius $a$ around the current position embed a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk) into [Brownian motion](brownian-motion.md). The [Strong Markov property](markov-process.md#strong-markov-property) makes the durations independent with common law $a^2\sigma_1$; the displacements divided by $a$ are independent symmetric signs. The displacement sequence is independent across exits; no [independence](random-variable.md#independent-random-variables) between a given displacement and its duration is needed for these conclusions.

##### Gaussian limit of a Brownian exit skeleton

↑ **Parent:** [Brownian exit-time skeleton](#brownian-exit-time-skeleton)

The position is the sum of $k$ independent symmetric signs. Its [characteristic function](probability-theory.md#characteristic-function) after division by $\sqrt k$ is $\cos(u/\sqrt k)^k\to e^{-u^2/2}$. The [Lévy continuity theorem](probability-theory.md#levy-continuity-theorem) gives the [normal distribution](probability-theory.md#normal-distribution) limit. Scaling the same skeleton to radius $2^{-n}$ and using [Brownian exit-skeleton clock convergence](#brownian-exit-skeleton-clock-convergence) identifies its other limit as $B_{\mathbb E\sigma_1}$, forcing $\mathbb E\sigma_1=1$.

##### Brownian exit-skeleton clock convergence

↑ **Parent:** [Brownian exit-time skeleton](#brownian-exit-time-skeleton)

Unit-radius [Brownian exit time](#brownian-exit-time) has finite [variance](variance.md), since independent unit-time increments give an exponential upper tail. The [Brownian exit-time skeleton](#brownian-exit-time-skeleton) clock after $2^{2n}$ radius-$2^{-n}$ exits has mean $\mathbb E\sigma_1$ and [variance](variance.md) $2^{-2n}\operatorname{Var}(\sigma_1)$. [Chebyshev's inequality](probability-inequality.md#chebyshev-inequality) and the [Borel-Cantelli first lemma](probability-theory.md#borel-cantelli-first-lemma) yield the displayed pathwise convergence. [Independence](random-variable.md#independent-random-variables) between different rows indexed by $n$ is unnecessary.

#### Laplace transform of symmetric Brownian interval-exit time

↑ **Parent:** [Brownian exit from an interval](#brownian-exit-from-an-interval)

For standard [Brownian motion](brownian-motion.md) started at zero and first exit $\tau_x$ from $(-x,x)$, the [Laplace transform](analysis.md#laplace-transform) is $1/\cosh(x\sqrt{2\lambda})$ for $\lambda>0$. The [stochastic process](stochastic-process.md) $e^{-\lambda t}\cosh(\sqrt{2\lambda}B_t)$ is the average of two copies of the [Exponential martingale for Brownian motion](#exponential-martingale-for-brownian-motion). Its values stopped at $t\wedge\tau_x$ are bounded, so bounded-time application of the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) followed by [dominated convergence](measure-theory.md#dominated-convergence-theorem) evaluates the transform without assuming [uniform integrability](convergence-of-random-variables.md#uniform-integrability) of an unstopped exponential [martingale](martingale.md) on the infinite horizon.

#### Brownian symmetric interval-exit moments

↑ **Parent:** [Brownian exit from an interval](#brownian-exit-from-an-interval)

For standard [Brownian motion](brownian-motion.md) started at zero, let $\tau_x$ be its first exit from $(-x,x)$, with $x>0$. Bounded-time stopping of $B_t^2-t$ first proves integrability of the exit time and then gives its mean $x^2$. Stopping the quartic [Hermite polynomial martingale](numerical-analysis.md#space-time-hermite-polynomial) gives a uniform bound on $\mathbb E(t\wedge\tau_x)^2$, proving second-moment integrability before passing to the limit. The resulting second moment is $5x^4/3$ and the [variance](variance.md) is $2x^4/3$.

#### Conditional Brownian interval-exit time

↑ **Parent:** [Brownian exit from an interval](#brownian-exit-from-an-interval)

The exit time conditioned on leaving through the upper endpoint satisfies

$$
\mathbb E[\tau_b\mid\tau_b<\tau_{-a}]
=\frac{b^2+2ab}{3}.
$$

Optional stopping of the cubic martingale $B_t^3-3tB_t$, together with the lower moments of the interval exit, gives the formula.

### Dynkin formula for Brownian motion

↑ **Parent:** [Brownian exit time](#brownian-exit-time)

For a suitable twice differentiable function $u$ and an integrable stopping time $T$,

$$
\mathbb E_xu(B_T)=u(x)+\mathbb E_x\int_0^T\frac12\Delta u(B_t)\,dt.
$$

It is the [Dynkin's formula](stochastic-process.md#dynkin-s-formula) with the [Brownian motion](brownian-motion.md) generator $\tfrac12\Delta$.

## Brownian bridge

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_bridge)

A standard Brownian bridge is the centered Gaussian process $B(t)=W(t)-tW(1)$ on $[0,1]$. Its covariance is $\min(s,t)-st$ and it satisfies $B(0)=B(1)=0$.

### Time reversal of a Brownian bridge

↑ **Parent:** [Brownian bridge](#brownian-bridge)

The [Brownian bridge covariance kernel](random-variable.md#brownian-bridge-covariance-kernel) is invariant under reversing both times, and its mean is zero. The two centered [Gaussian processes](stochastic-process.md#gaussian-process) therefore have equal finite-dimensional laws. Equality on countably many rational coordinates transfers the event of continuity at zero to the reversed endpoint. Interior continuity then extends the rational-time limit to all times. This proves the terminal continuity of the [stochastic integral representation of a Brownian bridge](#stochastic-integral-representation-of-a-brownian-bridge).

### Stochastic integral representation of a Brownian bridge

↑ **Parent:** [Brownian bridge](#brownian-bridge)

For $t<1$ this [stochastic integral](stochastic-calculus.md#stochastic-integral) solves $dX_t=dB_t-X_t(1-t)^{-1}dt$. The [Itô product rule](stochastic-calculus.md#ito-product-rule) also gives $X_t=B_t-(1-t)\int_0^tB_s(1-s)^{-2}ds$. The process is centered [Gaussian](probability-theory.md#normal-distribution), with [covariance](variance.md#covariance) $\min(s,t)-st$, and has a continuous extension $X_1=0$. [Time reversal of a Brownian bridge](#time-reversal-of-a-brownian-bridge) proves endpoint continuity without assuming it at the start.

### F-Brownian bridge

↑ **Parent:** [Brownian bridge](#brownian-bridge)

For a [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $F$ and a standard [Brownian bridge](#brownian-bridge) $\mathbb G$, the F-Brownian bridge is the centred [Gaussian process](stochastic-process.md#gaussian-process) $\mathbb G_F=\mathbb G\circ F$. Its [covariance](variance.md#covariance) is $F(\min(s,t))-F(s)F(t)$, by substituting $F(s),F(t)$ into the bridge covariance. It can jump when $F$ jumps. Its law is tight in the [supremum norm](functional-analysis.md#supremum-norm), since composition with $F$ is a continuous map from the separable space of continuous bridge paths.

### Brownian bridge independence from its endpoint

↑ **Parent:** [Brownian bridge](#brownian-bridge)

For standard [Brownian motion](brownian-motion.md), the [Brownian bridge](#brownian-bridge) $U_t=B_t-tB_1$, $0\leq t\leq1$, is independent of $B_1$. Every finite vector of bridge coordinates is jointly [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) with $B_1$, and its cross-[covariances](variance.md#covariance) with $B_1$ vanish. The [independence of uncorrelated jointly normal variables](probability-and-statistics.md#independence-of-uncorrelated-jointly-normal-variables) and [independence extended from generating pi-systems](probability-theory.md#independence-extended-from-generating-pi-systems) prove independence of the whole [stochastic process](stochastic-process.md).

### Brownian-bridge crossing probability

↑ **Parent:** [Brownian bridge](#brownian-bridge)

For a one-dimensional diffusion of variance rate $2D$ conditioned to start at $x>0$ and end at $y>0$ after time $\Delta t$, the bridge crosses zero with probability $\exp[-xy/(D\Delta t)]$. This corrects endpoint-only absorption tests in time-stepping schemes.

## Exponential Brownian martingale

↑ **Parent:** [Brownian motion](brownian-motion.md)

For every real $c$,

$$
M_t=\exp\left(cW_t-\frac12c^2t\right)
$$

is a martingale. Conditional expectation factors at time $s$ because the Gaussian increment $W_t-W_s$ is independent of the past and has exponential moment $e^{c^2(t-s)/2}$.

### Parameter derivative of the exponential Brownian martingale

↑ **Parent:** [Exponential Brownian martingale](#exponential-brownian-martingale)

Every parameter derivative

$$
\frac{\partial^n}{\partial\lambda^n}
\exp(\lambda B_t-\lambda^2t/2)
$$

is a [martingale](martingale.md). Differentiation passes through conditional expectation because Gaussian exponential moments dominate every derivative locally uniformly in $\lambda$. At $\lambda=0$ these derivatives yield the time-space Hermite martingales, beginning with $B_t$, $B_t^2-t$, and $B_t^3-3tB_t$.

## Gaussian-process characterization of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

A centered [Gaussian process](stochastic-process.md#gaussian-process) with almost surely continuous paths and covariance $\mathbb E[B_sB_t]=\min(s,t)$ is a standard [Brownian motion](brownian-motion.md).

## Time inversion of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

If $W$ is [Brownian motion](brownian-motion.md), then

$$
B_0=0,
\qquad B_t=tW_{1/t}\quad(t>0)
$$

is also Brownian motion. Its covariance is $\min(s,t)$, and continuity at zero follows from $W_u/u\to0$ almost surely.

## Brownian motion with drift

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_motion_with_drift)

A Brownian motion with drift $\mu$ is $X_t=W_t+\mu t$ for a standard [Brownian motion](brownian-motion.md) $W$.

### Drifted Brownian interval-exit probability

↑ **Parent:** [Brownian motion with drift](#brownian-motion-with-drift)

For [Brownian motion with drift](#brownian-motion-with-drift) $dX=dB+\mu\,dt$ in $(-b,b)$, the displayed probability of exiting at $-b$ follows by stopping the harmonic function $e^{-2\mu X}$. A unit-time increment larger than $2b$ has a uniform positive probability and forces exit, so the exit time has a [geometric tail bound from a uniform escape probability](martingale.md#geometric-tail-bound-from-a-uniform-escape-probability) and all polynomial moments. At zero drift the limiting probability is $(b-x)/(2b)$.

### Infinite-horizon singularity of Brownian motion with constant drift

↑ **Parent:** [Brownian motion with drift](#brownian-motion-with-drift)

The laws on continuous paths of a standard [Brownian motion](brownian-motion.md) and a [Brownian motion with drift](#brownian-motion-with-drift) $\mu\ne0$ are [mutually singular measures](measure-theory.md#mutually-singular-measures) on the whole half-line. The event $\lim_{t\to\infty}\omega(t)/t=0$ has full measure for the former and zero measure for the latter by the [strong law for Brownian motion](#strong-law-for-brownian-motion). On every fixed finite horizon, their laws are equivalent by the [Girsanov theorem](stochastic-calculus.md#girsanov-theorem). The finite-horizon densities $e^{\mu B_t-\mu^2t/2}$ tend to zero [almost surely](convergence-of-random-variables.md#almost-sure-convergence) while retaining [expectation](probability-theory.md#expected-value) one, so they lack [uniform integrability](convergence-of-random-variables.md#uniform-integrability) over all time.

### Finite-horizon maximum of Brownian motion with negative drift

↑ **Parent:** [Brownian motion with drift](#brownian-motion-with-drift)

For $a,b>0$,

$$
\mathbb P\!\left(\sup_{0\leq s\leq t}(W_s-as)\leq b\right)
=\Phi\!\left(\frac{b+at}{\sqrt t}\right)
-e^{-2ab}\Phi\!\left(\frac{at-b}{\sqrt t}\right).
$$

This follows from the [Brownian reflection principle](#reflection-principle-wiener-process) weighted by the [Cameron-Martin theorem for a linear drift](#cameron-martin-theorem-for-a-linear-drift).

### Infinite-horizon crossing probability for Brownian motion with negative drift

↑ **Parent:** [Brownian motion with drift](#brownian-motion-with-drift)

For $a,y>0$,

$$
\mathbb P\!\left(\sup_{u\geq0}(W_u-au)>y\right)=e^{-2ay}.
$$

### Last passage time above a level for Brownian motion with negative drift

↑ **Parent:** [Brownian motion with drift](#brownian-motion-with-drift)

For $a,b>0$ and the convention $\sup\varnothing=0$,

$$
\mathbb P(T\leq t)
=\Phi\!\left(a\sqrt t+\frac b{\sqrt t}\right)
-e^{-2ab}\Phi\!\left(\frac b{\sqrt t}-a\sqrt t\right),
\qquad t>0.
$$

## Reflection principle (Wiener process)

↑ **Parent:** [Brownian motion](brownian-motion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflection_principle_(Wiener_process))

Reflecting a Brownian path after its first hit of a level $b>0$ preserves Wiener measure and maps an endpoint $x\leq b$ to $2b-x\geq b$.

### Brownian terminal-to-maximum ratio

↑ **Parent:** [Reflection principle (Wiener process)](#reflection-principle-wiener-process)

The ratio of the terminal value of a standard [Brownian motion](brownian-motion.md) to its running maximum at time one has density $(2-r)^{-2}$ for $r<1$ and zero otherwise. The [Brownian reflection principle](#reflection-principle-wiener-process) gives joint density $2(2m-w)\varphi(2m-w)$ for $m>0,w<m$. Substituting $w=rm$ and integrating the Jacobian factor $m$ proves the density; its integral on $(-\infty,1)$ is one.

### Brownian reflection at a stopping time

↑ **Parent:** [Reflection principle (Wiener process)](#reflection-principle-wiener-process)

Reflecting a [Brownian motion](brownian-motion.md) $B$ after a [stopping time](martingale.md#stopping-time) $T$ by $\widehat B_t=2B_T-B_t$ for $t>T$, and leaving it unchanged for $t\leq T$, preserves its path [probability distribution](probability-theory.md#probability-distribution). For finite $T$, the [Strong Markov property](markov-process.md#strong-markov-property) and symmetry of the future [Brownian motion](brownian-motion.md) prove this. When $T=\infty$, the path is left unchanged.

### Brownian running maximum

↑ **Parent:** [Reflection principle (Wiener process)](#reflection-principle-wiener-process)

For $M_t=\sup_{0\leq s\leq t}B_s$, the reflection principle gives

$$
\mathbb P(M_t\geq x)=2\mathbb P(B_t\geq x)
=\mathbb P(|B_t|\geq x),
$$

so $M_t$ and $|B_t|$ have the same distribution.

#### Gaussian maximal bound for Brownian motion

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

Stop the [Exponential martingale for Brownian motion](#exponential-martingale-for-brownian-motion) $e^{\theta B_s-\theta^2s/2}$ when $B$ first reaches $\delta$ or at $t$. On the hitting event its value is at least $e^{\theta\delta-\theta^2t/2}$, so that event has [probability](probability-theory.md#probability) at most $e^{-\theta\delta+\theta^2t/2}$. Minimize over $\theta>0$ and apply the same bound to $-B$. The union bound gives the displayed inequality for $t>0$; at zero the [probability](probability-theory.md#probability) is zero.

#### Atomless maxima on separated Brownian intervals

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

For [Brownian motion](brownian-motion.md), write the later maximum as $B_b+Z+H$, where $Z=B_c-B_b$ has a nondegenerate [normal distribution](probability-theory.md#normal-distribution) and $H=\sup_{0\leq u\leq d-c}(B_{c+u}-B_c)$. The [independent increments](stochastic-process.md#independent-increments) make $Z$ independent of the earlier history and of $H$. Conditional on those two objects, equality of the two maxima prescribes one value of $Z$, an event of probability zero. This argument uses the positive gap $c-b$ and does not assume independence of the two absolute maxima.

#### Finite-horizon maximum of Brownian motion with drift

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

For $a>0$ and $t>0$, the distribution function is $\Phi((a-\nu t)/\sqrt t)-e^{2a\nu}\Phi((-a-\nu t)/\sqrt t)$. The [Brownian reflection principle](#reflection-principle-wiener-process) gives the zero-drift terminal density below the barrier as $\phi_t(y)-\phi_t(2a-y)$ for $y<a$. Weight it by $e^{\nu y-\nu^2t/2}$ using the [Girsanov theorem](stochastic-calculus.md#girsanov-theorem) and complete squares in the two Gaussian integrals.

##### Joint endpoint and maximum law for drifted Brownian motion

↑ **Parent:** [Finite-horizon maximum of Brownian motion with drift](#finite-horizon-maximum-of-brownian-motion-with-drift)

For $W_t^\nu=B_t+\nu t$, $M_t^\nu=\sup_{s\le t}W_s^\nu$, $a>0$ and $x\le a$, the joint distribution function is $\Phi((x-\nu t)/\sqrt t)-e^{2a\nu}\Phi((x-2a-\nu t)/\sqrt t)$. The [Brownian reflection principle](#reflection-principle-wiener-process) gives killed endpoint density $\phi_t(y)-\phi_t(2a-y)$ at zero drift. Multiplication by $e^{\nu y-\nu^2t/2}$ and completion of squares gives the formula.

#### Integral lower envelope for the Brownian maximum

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

Let $f$ be positive, continuous and nondecreasing, with $\int_0^1f(t)\,dt/t<\infty$. The small-value [probability](probability-theory.md#probability) for the [Brownian running maximum](#brownian-running-maximum) is at most a constant times the value. [Brownian scaling](#brownian-scaling) and dyadic integral comparison make the exceptional [probabilities](probability-theory.md#probability) $\mathbb P(S_{2^{-n-1}}<2^{-n/2}f(2^{-n}))$ summable. The [Borel-Cantelli first lemma](probability-theory.md#borel-cantelli-first-lemma) and monotonicity interpolate between dyadic times. Apply this argument to $mf$ for every positive integer $m$ on a countable intersection of probability-one events to obtain the infinite lower limit.

#### Brownian barrier survival asymptotic

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

For standard one-dimensional [Brownian motion](brownian-motion.md) and a fixed $h>0$, the [Brownian reflection principle](#reflection-principle-wiener-process) gives the survival [probability](probability-theory.md#probability) $2\Phi(h/\sqrt t)-1$. The [standard normal distribution function](probability-theory.md#standard-normal-distribution-function) has derivative $1/\sqrt{2\pi}$ at zero, giving the displayed asymptotic. Thus the persistence exponent is one half, with leading constant $h\sqrt{2/\pi}$.

#### Maximum before a lower Brownian barrier

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

Stopping Brownian motion at its first crossing below $-b$, the nonnegative local martingale $(W_{t\wedge\tau}+b)/b$ starts at one and ends at zero. The [maximal identity for a continuous nonnegative local martingale tending to zero](martingale.md#maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero) gives tail $b/(b+x)$ for the stopped maximum, hence density $b/(b+x)^2$ for $x>0$. There is no atom at zero.

#### Joint distribution of Brownian motion and its running maximum

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

Let $M_t=\sup_{0\leq s\leq t}B_s$ for a standard [Brownian motion](brownian-motion.md). For $m\geq0$, the [Brownian reflection principle](#reflection-principle-wiener-process) gives

$$
\mathbb P(B_t\leq b,M_t\leq m)=
\begin{cases}
\Phi(b/\sqrt t)+\Phi((2m-b)/\sqrt t)-1,&b\leq m,\\
2\Phi(m/\sqrt t)-1,&b>m.
\end{cases}
$$

On $b<m$, the pair $(B_t,M_t)$ therefore has [joint probability density](continuous-probability-distribution.md#joint-probability-density)

$$
f_{B_t,M_t}(b,m)=
\frac{2(2m-b)}{\sqrt{2\pi}\,t^{3/2}}
e^{-(2m-b)^2/(2t)}.
$$

<h4 id="levy-identity-for-brownian-motion">Lévy identity for Brownian motion</h4>

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

For a standard [Brownian motion](brownian-motion.md) $B$, its [Brownian running maximum](#brownian-running-maximum) $M$, and its [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale) $L^0$ at zero, the process pairs satisfy

$$
(M_t-B_t,M_t)_{t\geq0}
\overset d=
(|B_t|,L_t^0)_{t\geq0}.
$$

In particular, $M-B$ and $|B|$ are both [Reflected Brownian motion](#reflected-brownian-motion) and have the same law as processes.

#### Time of the Brownian maximum

↑ **Parent:** [Brownian running maximum](#brownian-running-maximum)

Brownian motion attains its maximum on $[0,1]$ at a unique time $M^*$ almost surely. This time has the arcsine distribution

$$
\mathbb P(M^*\leq s)=\frac2\pi\arcsin\sqrt s,
\qquad 0\leq s\leq1.
$$

##### Brownian motion shifted at its finite-horizon maximum

↑ **Parent:** [Time of the Brownian maximum](#time-of-the-brownian-maximum)

Let $\tau$ be the first attainment of the maximum of standard [Brownian motion](brownian-motion.md) on $[0,T]$, with $T>0$. Time reversal shows $\tau<T$ with probability one. Then $Y_t\leq0$ for $0\leq t\leq T-\tau$, an initial interval of positive length. Standard [Brownian motion](brownian-motion.md) has probability zero of this property by the [Brownian reflection principle](#reflection-principle-wiener-process), so $Y$ is not Brownian. Moreover $\tau$ is not a [stopping time](martingale.md#stopping-time) for the [natural Brownian filtration](#natural-brownian-filtration): for $0<t<T$, $\mathbb P(\tau\leq t\mid\mathcal F_t)=2\Phi((M_t-B_t)/\sqrt{T-t})-1$, which is strictly between zero and one on $\{B_t<0\}$. The [Strong Markov property](markov-process.md#strong-markov-property) is therefore inapplicable at this random time.

## Brownian transition semigroup

↑ **Parent:** [Brownian motion](brownian-motion.md)

For suitable $f$,

$$
(P_tf)(x)=\mathbb E[f(x+\sqrt tZ)]
$$

defines the Brownian transition semigroup. Its generator identity is

$$
\frac d{dt}P_tf=\frac12P_tf''.
$$

Each Gaussian-convolution operator is a rescaled [Weierstrass transform](analysis.md#weierstrass-transform); the semigroup combines all times.

### Brownian transition density

↑ **Parent:** [Brownian transition semigroup](#brownian-transition-semigroup)

The transition density of standard Brownian motion in $\mathbb R^d$ is the [heat kernel](diffusion-equation.md#heat-kernel)

$$
p_t(x,y)=\frac{1}{(2\pi t)^{d/2}}
\exp\left(-\frac{|y-x|^2}{2t}\right),
\qquad t>0.
$$

Thus $\mathbb P_x(X_t\in A)=\int_Ap_t(x,y)\,dy$.

#### Killed Brownian transition density

↑ **Parent:** [Brownian transition density](#brownian-transition-density)

The area density of $\mathbb P_z(B_t\in dw,\ t<T_D)$ for [planar Brownian motion](#planar-brownian-motion) killed on its first exit from $D$. Its total mass is the survival probability, not generally one. Integrating this density over time gives the [Green function of killed planar Brownian motion](analysis.md#green-function-of-killed-planar-brownian-motion).

### Brownian compensator martingale

↑ **Parent:** [Brownian transition semigroup](#brownian-transition-semigroup)

For a twice differentiable integrable test function $f$ and Brownian motion $W$,

$$
f(W_t)-\frac12\int_0^tf''(W_s)\,ds
$$

is a martingale. This is the one-dimensional generator form of Dynkin's formula.

## Exponential test-function characterization of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion.md)

Let $W$ be continuous with $W_0=0$. If

$$
e^{cW_t}-\frac{c^2}{2}\int_0^te^{cW_s}\,ds
$$

is a martingale for every real $c$, then conditional expectations solve

$$
\mathbb E[e^{cW_t}\mid\mathcal F_s]
=e^{cW_s+c^2(t-s)/2}.
$$

Thus $W_t-W_s$ is independent of $\mathcal F_s$ and distributed as $N(0,t-s)$, so $W$ is Brownian motion.

### Conditional characteristic-function criterion for Brownian increments

↑ **Parent:** [Exponential test-function characterization of Brownian motion](#exponential-test-function-characterization-of-brownian-motion)

For an adapted continuous process starting at zero, the displayed conditional [characteristic function](probability-theory.md#characteristic-function) identifies every increment as $N(0,t-s)$ and makes it independent of the preceding sigma-field. Multiply by the indicator of an event in that sigma-field, then use the [uniqueness theorem for characteristic functions](probability-theory.md#uniqueness-theorem-for-characteristic-functions) for finite measures. Thus the process is a [Brownian motion](brownian-motion.md) in the given filtration.

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process.md)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (456)

- [Addition law for square-root branching diffusions](stochastic-calculus.md#addition-law-for-square-root-branching-diffusions)
- [Additivity of independently driven squared Bessel processes](#additivity-of-independently-driven-squared-bessel-processes)
- [Arctangent transform of a two-noise affine diffusion](stochastic-calculus.md#arctangent-transform-of-a-two-noise-affine-diffusion)
- [Asymmetric Brownian interval-exit transform](#asymmetric-brownian-interval-exit-transform)
- [Atomless maxima on separated Brownian intervals](#atomless-maxima-on-separated-brownian-intervals)
- [Bessel process](#bessel-process)
- [Binary Brownian drift filter](time-series.md#binary-brownian-drift-filter)
- [Blumenthal zero-one law](#blumenthal-zero-one-law)
- [Bounded Girsanov density for exit of an unstable linear diffusion](stochastic-calculus.md#bounded-girsanov-density-for-exit-of-an-unstable-linear-diffusion)
- [Brownian barrier survival asymptotic](#brownian-barrier-survival-asymptotic)
- [Brownian bridge independence from its endpoint](#brownian-bridge-independence-from-its-endpoint)
- [Brownian conditioning by a stopped Bessel density](stochastic-calculus.md#brownian-conditioning-by-a-stopped-bessel-density)
- [Brownian covariance kernel](random-variable.md#brownian-covariance-kernel)
- [Brownian excursion in the upper half-plane](#brownian-excursion-in-the-upper-half-plane)
- [Brownian exit law from a quadrant](#brownian-exit-law-from-a-quadrant)
- [Brownian exit-time expectation in an orthant](#brownian-exit-time-expectation-in-an-orthant)
- [Brownian exit-time skeleton](#brownian-exit-time-skeleton)
- [Brownian filtration](#brownian-filtration)
- [Brownian first-passage Laplace transform](markov-process.md#brownian-first-passage-laplace-transform)
- [Brownian first-passage subordinator](stochastic-process.md#brownian-first-passage-subordinator)
- [Brownian first-passage time](markov-process.md#brownian-first-passage-time)
- [Brownian hitting of lattice spheres](#brownian-hitting-of-lattice-spheres)
- [Brownian increment](#brownian-increment)
- [Brownian local time](stochastic-calculus.md#brownian-local-time)
- [Brownian martingale proof of Gaussian concentration](stochastic-process.md#brownian-martingale-proof-of-gaussian-concentration)
- [Brownian motion shifted at its finite-horizon maximum](#brownian-motion-shifted-at-its-finite-horizon-maximum)
- [Brownian motion transform by three times its running average](#brownian-motion-transform-by-three-times-its-running-average)
- [Brownian motion with drift](#brownian-motion-with-drift)
- [Brownian portfolio exposures](mathematical-finance.md#brownian-portfolio-exposures)
- [Brownian reflection at a stopping time](#brownian-reflection-at-a-stopping-time)
- [Brownian representation of half-plane capacity](stochastic-process.md#brownian-representation-of-half-plane-capacity)
- [Brownian scaling](#brownian-scaling)
- [Brownian sheet](stochastic-process.md#brownian-sheet)
- [Brownian sign transform](#brownian-sign-transform)
- [Brownian sphere-hitting probability in dimension three](#brownian-sphere-hitting-probability-in-dimension-three)
- [Brownian symmetric interval-exit moments](#brownian-symmetric-interval-exit-moments)
- [Brownian terminal-to-maximum ratio](#brownian-terminal-to-maximum-ratio)
- [Brownian time reversal on a finite interval](#brownian-time-reversal-on-a-finite-interval)
- [Brownian upper law of the iterated logarithm](convergence-of-random-variables.md#brownian-upper-law-of-the-iterated-logarithm)
- [Brownian zero mode of a fluctuating interface](stochastic-process.md#brownian-zero-mode-of-a-fluctuating-interface)
- [Brownian zero set](#brownian-zero-set)
- [Cameron-Martin theorem for a linear drift](#cameron-martin-theorem-for-a-linear-drift)
- [Cauchy exit law from a Brownian half-plane](#cauchy-exit-law-from-a-brownian-half-plane)
- [Cauchy law of an infinite-horizon Brownian exponential integral](probability-theory.md#cauchy-law-of-an-infinite-horizon-brownian-exponential-integral)
- [Cauchy process](stochastic-process.md#cauchy-process)
- [Characteristic function under conditionally symmetric martingale increments](martingale.md#characteristic-function-under-conditionally-symmetric-martingale-increments)
- [Circle-average process of the Gaussian free field is Brownian motion](stochastic-process.md#circle-average-process-of-the-gaussian-free-field-is-brownian-motion)
- [Complex exponential construction of planar Brownian motion](#complex-exponential-construction-of-planar-brownian-motion)
- [Complex exponential of two orthogonal Brownian motions](stochastic-calculus.md#complex-exponential-of-two-orthogonal-brownian-motions)
- [Conditional characteristic-function criterion for Brownian increments](#conditional-characteristic-function-criterion-for-brownian-increments)
- [Conditionally Gaussian stochastic integral with an independent integrator](stochastic-calculus.md#conditionally-gaussian-stochastic-integral-with-an-independent-integrator)
- [Conformal invariance of planar Brownian motion](#conformal-invariance-of-planar-brownian-motion)
- [Conformal Markov property of SLE](stochastic-process.md#conformal-markov-property-of-sle)
- [Constant market price of risk investment](utility-function.md#constant-market-price-of-risk-investment)
- [Continuous Lévy process](stochastic-process.md#continuous-levy-process)
- [Cosine-exponential Brownian local martingale](martingale.md#cosine-exponential-brownian-local-martingale)
- [Cylindrical Brownian motion](#cylindrical-brownian-motion)
- [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem)
- [Dickey–Fuller test](time-series.md#dickey-fuller-test)
- [Diffusion amplitude](stochastic-calculus.md#diffusion-amplitude)
- [Diffusion limit](stochastic-calculus.md#diffusion-limit)
- [Diffusion with hyperbolic tangent drift](stochastic-calculus.md#diffusion-with-hyperbolic-tangent-drift)
- [Divergence of a driftless Brownian exponential clock](#divergence-of-a-driftless-brownian-exponential-clock)
- [Divergence of a positive planar Brownian occupation integral](#divergence-of-a-positive-planar-brownian-occupation-integral)
- [Domain Markov property of a chordal Loewner chain](stochastic-process.md#domain-markov-property-of-a-chordal-loewner-chain)
- [Donsker's theorem](convergence-of-random-variables.md#donsker-s-theorem)
- [Dyadic interval](real-analysis.md#dyadic-interval)
- [Dyadic quadratic variation of Brownian motion](stochastic-calculus.md#dyadic-quadratic-variation-of-brownian-motion)
- [Dynkin formula for a diffusion](stochastic-process.md#dynkin-formula-for-a-diffusion)
- [Dynkin formula for Brownian motion](#dynkin-formula-for-brownian-motion)
- [Enhanced Brownian motion](analysis.md#enhanced-brownian-motion)
- [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](stochastic-process.md#exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process)
- [Exponential martingale for Brownian motion](#exponential-martingale-for-brownian-motion)
- [Finite-horizon drift replacement by a change of measure](stochastic-calculus.md#finite-horizon-drift-replacement-by-a-change-of-measure)
- [Finite-horizon exponential-utility portfolio](utility-function.md#finite-horizon-exponential-utility-portfolio)
- [Fixed-level versus simultaneous Brownian passage-time equality](markov-process.md#fixed-level-versus-simultaneous-brownian-passage-time-equality)
- [Fourth-moment deficit and bracket variance identity](martingale.md#fourth-moment-deficit-and-bracket-variance-identity)
- [Gaussian Brownian drift filter](time-series.md#gaussian-brownian-drift-filter)
- [Gaussian continuous martingale](stochastic-process.md#gaussian-continuous-martingale)
- [Gaussian heat kernel](diffusion-equation.md#gaussian-heat-kernel)
- [Gaussian-process characterization of Brownian motion](#gaussian-process-characterization-of-brownian-motion)
- [Gaussian white noise](stochastic-process.md#gaussian-white-noise)
- [Gaussian white noise model](stochastic-process.md#gaussian-white-noise-model)
- [Girsanov density for a stopped Bessel process](stochastic-calculus.md#girsanov-density-for-a-stopped-bessel-process)
- [Global existence theorem for stochastic differential equations with Lipschitz coefficients](stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients)
- [Harmonic functions of Brownian motion](partial-differential-equation.md#harmonic-functions-of-brownian-motion)
- [Heavy-traffic limit of a queue](queueing-theory.md#heavy-traffic-limit-of-a-queue)
- [Independent Brownian arms at a deterministic time](#independent-brownian-arms-at-a-deterministic-time)
- [Infinite-horizon singularity of Brownian motion with constant drift](#infinite-horizon-singularity-of-brownian-motion-with-constant-drift)
- [Infinite occupation time of one-dimensional Brownian motion](#infinite-occupation-time-of-one-dimensional-brownian-motion)
- [Instantaneous covariance rank in a one-factor rate model](mathematical-finance.md#instantaneous-covariance-rank-in-a-one-factor-rate-model)
- [Integrated Brownian motion](#integrated-brownian-motion)
- [Inverse-square Gaussian law of Brownian first passage](markov-process.md#inverse-square-gaussian-law-of-brownian-first-passage)
- [Itô diffusion](stochastic-calculus.md#ito-diffusion)
- [Itô integral](stochastic-calculus.md#ito-integral)
- [Itô's lemma](stochastic-calculus.md#ito-s-lemma)
- [Joint distribution of Brownian motion and its running maximum](#joint-distribution-of-brownian-motion-and-its-running-maximum)
- [Knight theorem for orthogonal martingales](stochastic-calculus.md#knight-theorem-for-orthogonal-martingales)
- [Lamperti transform (diffusion)](stochastic-calculus.md#lamperti-transform-diffusion)
- [Laplace transform of symmetric Brownian interval-exit time](#laplace-transform-of-symmetric-brownian-interval-exit-time)
- [Last visit to a bounded ball for three-dimensional Brownian motion](#last-visit-to-a-bounded-ball-for-three-dimensional-brownian-motion)
- [Learning hedge in a binary-drift investment model](utility-function.md#learning-hedge-in-a-binary-drift-investment-model)
- [Lévy area](#levy-area)
- [Lévy characterization of Brownian motion](#levy-characterization-of-brownian-motion)
- [Lévy characterization of multidimensional Brownian motion](#levy-characterization-of-multidimensional-brownian-motion)
- [Lévy identity for Brownian motion](#levy-identity-for-brownian-motion)
- [Linear-boundary Brownian first-passage distribution](markov-process.md#linear-boundary-brownian-first-passage-distribution)
- [Local maximum of Brownian motion](#local-maximum-of-brownian-motion)
- [Longitudinal Brownian field with transverse covariance](#longitudinal-brownian-field-with-transverse-covariance)
- [Market price of risk](mathematical-finance.md#market-price-of-risk)
- [Martingale problem for Brownian motion](stochastic-calculus.md#martingale-problem-for-brownian-motion)
- [Maximum occupation is not a hitting probability](markov-process.md#maximum-occupation-is-not-a-hitting-probability)
- [Natural Brownian filtration](#natural-brownian-filtration)
- [Nested polygonal approximation of Brownian rough paths](analysis.md#nested-polygonal-approximation-of-brownian-rough-paths)
- [Newtonian potential of the Brownian heat kernel](diffusion-equation.md#newtonian-potential-of-the-brownian-heat-kernel)
- [Nowhere monotonicity of Brownian motion](#nowhere-monotonicity-of-brownian-motion)
- [Occupation approximations for Brownian local time](stochastic-calculus.md#occupation-approximations-for-brownian-local-time)
- [Orthogonal continuous local martingales](stochastic-calculus.md#orthogonal-continuous-local-martingales)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33.md#2/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4.md#28j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#6/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-31.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#28j/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-70.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#28j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#29j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#29i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#29j/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#1/c/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#5/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#6/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#3/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#3/3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#3/3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#3/3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#4/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#4/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#5/c/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#27k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#27j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316.md#4/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#6/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-310.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-202.md#1/1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#29k/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#29k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-4.md#29k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-220.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-220.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-220.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#29k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#29k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#29k/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-202.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#1/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4.md#29k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-202.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-353.md#4/b/i/solution)
- [Pathwise quadratic variation distinguishes Brownian speeds](stochastic-calculus.md#pathwise-quadratic-variation-distinguishes-brownian-speeds)
- [Portfolio with constant stock value in bond units](mathematical-finance.md#portfolio-with-constant-stock-value-in-bond-units)
- [Probabilistic representation of the heat equation with time-dependent Dirichlet data](diffusion-equation.md#probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data)
- [Projection criterion for Brownian avoidance of affine subspaces](#projection-criterion-for-brownian-avoidance-of-affine-subspaces)
- [Quadratic covariations of an analytic Brownian image](stochastic-calculus.md#quadratic-covariations-of-an-analytic-brownian-image)
- [Realized absolute covariation](stochastic-calculus.md#realized-absolute-covariation)
- [Recovery of a continuous Brownian integrand from short increments](stochastic-calculus.md#recovery-of-a-continuous-brownian-integrand-from-short-increments)
- [Recurrence of one-dimensional Brownian motion](#recurrence-of-one-dimensional-brownian-motion)
- [Reflected Brownian motion with negative drift](#reflected-brownian-motion-with-negative-drift)
- [Rotational invariance of Brownian motion](#rotational-invariance-of-brownian-motion)
- [Same-noise stationary Ornstein-Uhlenbeck processes](stochastic-process.md#same-noise-stationary-ornstein-uhlenbeck-processes)
- [Scaling classification of a continuous-time symmetric simple random walk](stochastic-process.md#scaling-classification-of-a-continuous-time-symmetric-simple-random-walk)
- [Schramm–Loewner evolution](stochastic-process.md#schramm-loewner-evolution)
- [Sharp-k smoothing filter](large-scale-structure-of-the-universe.md#sharp-k-smoothing-filter)
- [Skorokhod embedding theorem](martingale.md#skorokhod-embedding-theorem)
- [Skorokhod space](functional-analysis.md#skorokhod-space)
- [Small-radius Brownian winding law](#small-radius-brownian-winding-law)
- [Space-time harmonic functions along Brownian motion](diffusion-equation.md#space-time-harmonic-functions-along-brownian-motion)
- [Space-time Hermite polynomial](numerical-analysis.md#space-time-hermite-polynomial)
- [Square-root stock implied volatility](mathematical-finance.md#square-root-stock-implied-volatility)
- [Squared Bessel process](#squared-bessel-process)
- [Stochastic calculus](stochastic-calculus.md)
- [Stock-numeraire measure in the Black-Scholes model](mathematical-finance.md#stock-numeraire-measure-in-the-black-scholes-model)
- [Stopped inverse radial power martingale classification](#stopped-inverse-radial-power-martingale-classification)
- [Strict generalized inverse of a nondecreasing function](calculus.md#strict-generalized-inverse-of-a-nondecreasing-function)
- [Strict local martingale failure of the law of one price](mathematical-finance.md#strict-local-martingale-failure-of-the-law-of-one-price)
- [Strict order preservation for scalar Lipschitz diffusions](stochastic-calculus.md#strict-order-preservation-for-scalar-lipschitz-diffusions)
- [Strong existence](stochastic-calculus.md#strong-existence)
- [Strong solution of a stochastic differential equation](stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation)
- [Subordination of a Lévy process](stochastic-process.md#subordination-of-a-levy-process)
- [Support of enhanced Brownian motion](analysis.md#support-of-enhanced-brownian-motion)
- [Survival among independently moving Poisson traps](#survival-among-independently-moving-poisson-traps)
- [Tanaka equation](stochastic-calculus.md#tanaka-equation)
- [Three-dimensional Bessel process](#three-dimensional-bessel-process)
- [Time inversion of Brownian motion](#time-inversion-of-brownian-motion)
- [Transience of Brownian motion in dimension at least three](#transience-of-brownian-motion-in-dimension-at-least-three)
- [Truncation construction of a positive Bessel strong solution](#truncation-construction-of-a-positive-bessel-strong-solution)
- [Uniform ball sampling by Brownian stopping](#uniform-ball-sampling-by-brownian-stopping)
- [Up-and-out power claim](mathematical-finance.md#up-and-out-power-claim)
- [Upper-half-plane harmonic measure of the positive half-axis](#upper-half-plane-harmonic-measure-of-the-positive-half-axis)
- [Wiener measure](#wiener-measure)
- [Wiener sausage](#wiener-sausage)
- [Wiener theorem](#wiener-theorem)
