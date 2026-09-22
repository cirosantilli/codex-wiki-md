# Schramm–Loewner evolution

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schramm–Loewner_evolution)

Chordal Schramm–Loewner evolution in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) from $0$ to $\infty$ is the random [Loewner chain](#loewner-chain) driven by $U_t=\sqrt\kappa B_t$, where $B$ is standard [Brownian motion](brownian-motion.md) and $\kappa\geq0$.

**Table of contents**

- [Cardy boundary crossing formula](#cardy-boundary-crossing-formula)
- [Chordal SLE4](#chordal-sle4)
- [Radial Schramm–Loewner evolution](#radial-schramm-loewner-evolution)
  - [Radial SLE2](#radial-sle2)
- [Scale-and-domain-Markov characterization of SLE](#scale-and-domain-markov-characterization-of-sle)
- [SLE angle process](#sle-angle-process)
  - [Dirichlet boundary values of the SLE angle process](#dirichlet-boundary-values-of-the-sle-angle-process)
  - [Logarithmic martingale for SLE4](#logarithmic-martingale-for-sle4)
    - [Fixed-interior-point avoidance of SLE4](#fixed-interior-point-avoidance-of-sle4)
  - [SLE4 angle martingale](#sle4-angle-martingale)
  - [SLE interior-point martingale](#sle-interior-point-martingale)
- [Compact H-hull](#compact-h-hull)
  - [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)
    - [Monotonicity of boundary derivatives of mapping-out functions](#monotonicity-of-boundary-derivatives-of-mapping-out-functions)
    - [Differentiability estimate for a mapping-out function](#differentiability-estimate-for-a-mapping-out-function)
    - [High-level escape representation of a mapping-out height](#high-level-escape-representation-of-a-mapping-out-height)
    - [Height contraction of a hydrodynamically normalized mapping-out function](#height-contraction-of-a-hydrodynamically-normalized-mapping-out-function)
    - [Inverse-at-infinity criterion for local boundedness of a mapping-out function](#inverse-at-infinity-criterion-for-local-boundedness-of-a-mapping-out-function)
    - [Mapping-out function of a vertical slit](#mapping-out-function-of-a-vertical-slit)
    - [Real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull)
      - [Sharp displacement bound for a compact H-hull](#sharp-displacement-bound-for-a-compact-h-hull)
        - [Nearly closed semicircular slit](#nearly-closed-semicircular-slit)
    - [Hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity)
    - [Half-plane capacity](#half-plane-capacity)
      - [Half-plane capacity versus harmonic hull capacity](#half-plane-capacity-versus-harmonic-hull-capacity)
      - [Half-plane capacity of a half-disc](#half-plane-capacity-of-a-half-disc)
      - [Conformal change of half-plane capacity](#conformal-change-of-half-plane-capacity)
        - [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)
          - [Boundary derivative diffusion under conformal Loewner conjugacy](#boundary-derivative-diffusion-under-conformal-loewner-conjugacy)
          - [Transformed SLE driving function](#transformed-sle-driving-function)
      - [Half-plane capacity of a vertical slit](#half-plane-capacity-of-a-vertical-slit)
      - [Scaling and translation of half-plane capacity](#scaling-and-translation-of-half-plane-capacity)
      - [Monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity)
        - [Half-plane-capacity composition rule](#half-plane-capacity-composition-rule)
      - [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity)
      - [Half-plane capacity is bounded by squared diameter](#half-plane-capacity-is-bounded-by-squared-diameter)
      - [Half-plane capacity of a low rectangle](#half-plane-capacity-of-a-low-rectangle)
      - [Half-plane-capacity parameterization](#half-plane-capacity-parameterization)
    - [Boundary degeneration under a mapping-out function](#boundary-degeneration-under-a-mapping-out-function)
- [Loewner chain](#loewner-chain)
  - [Domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain)
    - [Simplicity of SLE from boundary-avoiding restarts](#simplicity-of-sle-from-boundary-avoiding-restarts)
  - [Capacity-parametrized scale invariance of a Loewner chain](#capacity-parametrized-scale-invariance-of-a-loewner-chain)
  - [Trace of a Loewner chain](#trace-of-a-loewner-chain)
    - [Boundary extension of the inverse map for a continuous Loewner trace](#boundary-extension-of-the-inverse-map-for-a-continuous-loewner-trace)
  - [Loewner local growth property](#loewner-local-growth-property)
    - [Loewner correspondence theorem](#loewner-correspondence-theorem)
  - [Loewner differential equation](#loewner-differential-equation)
    - [Chordal Loewner equation](#chordal-loewner-equation)
      - [Loewner variation of the Dirichlet Green function](#loewner-variation-of-the-dirichlet-green-function)
      - [Boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain)
        - [SLE boundary swallowing criterion](#sle-boundary-swallowing-criterion)
      - [Interior-point swallowing time for a Loewner chain](#interior-point-swallowing-time-for-a-loewner-chain)
      - [Loewner driving function](#loewner-driving-function)
        - [Continuity estimate for the Loewner driving function](#continuity-estimate-for-the-loewner-driving-function)
        - [Driving-function reconstruction for a chordal Loewner chain](#driving-function-reconstruction-for-a-chordal-loewner-chain)
        - [Composition rule for chordal Loewner driving functions](#composition-rule-for-chordal-loewner-driving-functions)
        - [Square-root Loewner driving function generates a straight slit](#square-root-loewner-driving-function-generates-a-straight-slit)
        - [Boundary derivative of a chordal Loewner chain](#boundary-derivative-of-a-chordal-loewner-chain)
- [Scaling invariance of SLE](#scaling-invariance-of-sle)
  - [SLE reaches every positive height](#sle-reaches-every-positive-height)
- [Conformal Markov property of SLE](#conformal-markov-property-of-sle)
  - [Characterization of the SLE driving function](#characterization-of-the-sle-driving-function)
- [Conformal invariance of SLE](#conformal-invariance-of-sle)
  - [Chordal SLE in a specified scale](#chordal-sle-in-a-specified-scale)
  - [Chordal restriction property](#chordal-restriction-property)
    - [Restriction exponent of a chordal filling](#restriction-exponent-of-a-chordal-filling)
    - [Chordal filling](#chordal-filling)
      - [Avoidance probabilities determine a chordal filling law](#avoidance-probabilities-determine-a-chordal-filling-law)
    - [Derivative avoidance criterion for chordal restriction](#derivative-avoidance-criterion-for-chordal-restriction)
    - [Avoidance probabilities determine a simple chordal curve law](#avoidance-probabilities-determine-a-simple-chordal-curve-law)
    - [SLE eight-thirds restriction martingale](#sle-eight-thirds-restriction-martingale)
  - [Locality property of SLE](#locality-property-of-sle)
    - [Locality of a chord law under conformal changes of neighborhoods](#locality-of-a-chord-law-under-conformal-changes-of-neighborhoods)
    - [Target-change locality of SLE6](#target-change-locality-of-sle6)
      - [Target-dependent continuation of SLE6](#target-dependent-continuation-of-sle6)
- [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)
  - [Space-filling SLE above parameter eight](#space-filling-sle-above-parameter-eight)
  - [SLE Green-function estimate](#sle-green-function-estimate)
  - [SLE4 left-passage probability](#sle4-left-passage-probability)
  - [Boundary-intersection threshold for SLE](#boundary-intersection-threshold-for-sle)
    - [Positive boundary-interval hitting probability for SLE above parameter four](#positive-boundary-interval-hitting-probability-for-sle-above-parameter-four)
- [Transience of chordal SLE](#transience-of-chordal-sle)
- [Reverse Loewner flow](#reverse-loewner-flow)
  - [Reverse SLE derivative martingale](#reverse-sle-derivative-martingale)
    - [Reverse SLE derivative bound above the space-filling threshold](#reverse-sle-derivative-bound-above-the-space-filling-threshold)
- [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)
  - [Boundary approach forces a small SLE Bessel gap](#boundary-approach-forces-a-small-sle-bessel-gap)
  - [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion)
    - [Strict ordering threshold for SLE boundary swallowing](#strict-ordering-threshold-for-sle-boundary-swallowing)
      - [Real-line visitation from strict SLE swallowing order](#real-line-visitation-from-strict-sle-swallowing-order)
  - [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion)
    - [SLE does not hit a fixed nonzero boundary point](#sle-does-not-hit-a-fixed-nonzero-boundary-point)
  - [Two-sided SLE boundary swallowing probability](#two-sided-sle-boundary-swallowing-probability)

## Cardy boundary crossing formula

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

For critical planar percolation in a conformal quadrilateral, Cardy's boundary-crossing probability is $I_\theta(1/3,1/3)$, where $\theta\in(0,1)$ is its conformal cross-ratio and $I$ is the regularized incomplete beta function. This conformally invariant crossing law is associated with [Schramm–Loewner evolution](schramm-loewner-evolution.md) at parameter six.

The conformally invariant critical percolation crossing probability can be expressed in an appropriate ordered boundary cross ratio $\theta\in[0,1]$ as

$$
\frac{\int_0^\theta[u(1-u)]^{-2/3}\,du}{\int_0^1[u(1-u)]^{-2/3}\,du}.
$$

For the corresponding [SLE](schramm-loewner-evolution.md) exploration at parameter six, it arises from the [beta integral for strict ordering of coupled Bessel lifetimes](brownian-motion.md#beta-integral-for-strict-ordering-of-coupled-bessel-lifetimes) with $a=1/3$. In the upper-half-plane configuration $0<x<y$, the strict-swallowing probability is this function at $\theta=1-x/y$. Exchanging the two relevant boundary arcs exchanges the probability with its complement. This is a crossing probability, not the probability of visiting a fixed boundary point.

## Chordal SLE4

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

Chordal [SLE](schramm-loewner-evolution.md) at parameter four has driver $2\beta_t$ in half-plane-capacity time. The [Itô formula](stochastic-calculus.md#ito-s-lemma) makes the imaginary part of $\log(g_t(z)-W_t)$ drift-free, a feature used in the [SLE4 coupling with a Gaussian free field](gaussian-process.md#sle4-coupling-with-a-gaussian-free-field). The trace is simple and avoids fixed nonzero boundary points.

<h2 id="radial-schramm-loewner-evolution">Radial Schramm–Loewner evolution</h2>

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

Radial [SLE](schramm-loewner-evolution.md) grows from a boundary point to an interior target. In the unit disc from $1$ to $0$, its conformal-radius parameterization satisfies

$$
\partial_tg_t(z)=g_t(z)\frac{e^{i\sqrt\kappa\beta_t}+g_t(z)}{e^{i\sqrt\kappa\beta_t}-g_t(z)},\qquad g_t'(0)=e^t.
$$

The target remains in the remaining simply connected component; the time parameter records its decreasing [conformal radius](geometry-and-topology.md#conformal-radius).

### Radial SLE2

↑ **Parent:** [Radial Schramm–Loewner evolution](#radial-schramm-loewner-evolution)

For radial [SLE](schramm-loewner-evolution.md) at parameter two, the normalized slit-domain [Poisson kernel](partial-differential-equation.md#poisson-kernel) at the growing tip is a [local martingale](martingale.md#local-martingale). This observable provides the coupling to [loop-erasure of planar Brownian motion](random-walk.md#loop-erasure-of-planar-brownian-motion), oriented from the boundary point to the interior target. Its discrete counterpart is a [loop-erased random walk](random-walk.md#loop-erased-random-walk).

## Scale-and-domain-Markov characterization of SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

Among [Loewner chains](#loewner-chain) with capacity $2t$, continuous real driver and initial driver zero, scale invariance and the centered [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain) characterize [Schramm–Loewner evolution](schramm-loewner-evolution.md) with some $\kappa\geq0$. [Driving-function reconstruction for a chordal Loewner chain](#driving-function-reconstruction-for-a-chordal-loewner-chain) turns the hull properties into stationary independent increments and Brownian scaling for the driver. The [continuous Lévy process](stochastic-process.md#continuous-levy-process) classification then gives $U_t=bt+\sqrt\kappa W_t$, and scaling eliminates $b$. Regularity and parametrization are essential hypotheses of this characterization.

## SLE angle process

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

With the upper-half-plane branch, $\theta_t\in(0,\pi)$ before the [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain). Write $Z_t=X_t+iY_t$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) and the [Chordal Loewner equation](#chordal-loewner-equation) give

$$
d\theta_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt+\sqrt\kappa\frac{Y_t}{|Z_t|^2}\,dB_t.
$$

At parameter four its drift vanishes. At other parameters the drift describes the competition between the deterministic conformal evolution and the Brownian driver.

### Dirichlet boundary values of the SLE angle process

↑ **Parent:** [SLE angle process](#sle-angle-process)

For the [SLE angle process](#sle-angle-process), the bounded [Dirichlet problem](analysis.md#dirichlet-problem) on the unbounded surviving domain has data $\pi$ on the intrinsic boundary mapped to the left of the [Loewner driving function](#loewner-driving-function) and zero on the boundary mapped to its right. For a simple [Loewner trace](#trace-of-a-loewner-chain) these are its left and right banks, with the negative and positive real rays respectively. The tip is a discontinuity point of the boundary data.

### Logarithmic martingale for SLE4

↑ **Parent:** [SLE angle process](#sle-angle-process)

For [Schramm–Loewner evolution](schramm-loewner-evolution.md) with $\kappa=4$ and $Z_t=g_t(z)-2W_t$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) for the [complex logarithm](analysis.md#complex-logarithm) gives $d\log Z_t=-2Z_t^{-1}dW_t$ before swallowing. The drift cancels exactly at this parameter. Its real part is $\log|Z_t|$ and its imaginary part is the [SLE4 angle martingale](#sle4-angle-martingale). The real-part [quadratic variation](stochastic-calculus.md#quadratic-variation) is $4\int X_t^2/|Z_t|^4\,dt$, which also gives a direct non-swallowing argument.

#### Fixed-interior-point avoidance of SLE4

↑ **Parent:** [Logarithmic martingale for SLE4](#logarithmic-martingale-for-sle4)

Every fixed $z\in\mathbb H$ has infinite [interior-point swallowing time for a Loewner chain](#interior-point-swallowing-time-for-a-loewner-chain) under [Schramm–Loewner evolution](schramm-loewner-evolution.md) at $\kappa=4$. The centered flow is bounded on any finite horizon, making $\log|Z_t|$ bounded above. The [one-sided bound criterion for a martingale clock](martingale.md#one-sided-bound-criterion-for-a-martingale-clock) gives a finite logarithmic limit at any putative finite swallowing time. Thus $|Z_t|$ stays away from zero and the imaginary coordinate remains positive, so the differential equation extends, a contradiction. In particular the trace misses each fixed interior point almost surely.

### SLE4 angle martingale

↑ **Parent:** [SLE angle process](#sle-angle-process)

For a fixed [interior](topology.md#interior-topology) point and parameter four, the [SLE angle process](#sle-angle-process) has zero drift and satisfies $\theta_t=\arg z+2\int_0^tY_s|Z_s|^{-2}\,dB_s$. Its values in $(0,\pi)$ make this continuous [local martingale](martingale.md#local-martingale) a true bounded [martingale](martingale.md). The identity $\log(\Upsilon_t/\Upsilon_0)=-[\theta]_t$, together with the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem), prevents its [Loewner conformal radius](geometry-and-topology.md#conformal-radius-under-a-chordal-loewner-flow) from vanishing at a finite lifetime. Since the parameter-four trace is simple and does not meet the real [boundary](topology.md#boundary-of-a-set) at positive times, finite swallowing would require a visit to the point and vanishing radius. Thus its [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain) is infinite almost surely. This gives a global continuous bounded [martingale](martingale.md), not just one defined before swallowing.

### SLE interior-point martingale

↑ **Parent:** [SLE angle process](#sle-angle-process)

For $\kappa>0$, $\rho>0$, let $J_t=|g_t'(z)|$, $S_t=\sin\theta_t$ and $\Upsilon_t=Y_t/J_t$. Then

$$
M_t=J_t^{(8-\kappa+\rho)\rho/(4\kappa)}\Upsilon_t^{\rho(\rho+8)/(8\kappa)}S_t^{-\rho/\kappa}
$$

is a positive continuous [local martingale](martingale.md#local-martingale) before the [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain). Indeed the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives $d\log J_t=-2(X_t^2-Y_t^2)|Z_t|^{-4}dt$, $d\log\Upsilon_t=-4Y_t^2|Z_t|^{-4}dt$, and

$$
d\log S_t=\frac{(\kappa/2-4)X_t^2-\kappa Y_t^2/2}{|Z_t|^4}\,dt+\sqrt\kappa\frac{X_t}{|Z_t|^2}\,dB_t.
$$

Combining the exponents cancels the drift of $M_t$, including the quadratic-variation correction, leaving $dM_t/M_t=-\rho X_t/(\sqrt\kappa|Z_t|^2)\,dB_t$.

## Compact H-hull

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

A compact H-hull is a bounded relatively closed subset $A$ of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) $\mathbb H$ such that $\mathbb H\setminus A$ is a [simply connected domain](complex-analysis.md#simply-connected-domain).

### Mapping-out function of a compact H-hull

↑ **Parent:** [Compact H-hull](#compact-h-hull)

The mapping-out function is the unique [conformal map](geometry-and-topology.md#conformal-map) $g_A:\mathbb H\setminus A\to\mathbb H$ with [hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity)

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

#### Monotonicity of boundary derivatives of mapping-out functions

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For nested [compact H-hulls](#compact-h-hull) whose closures avoid $x\in\mathbb R$, the [boundary derivative is an excursion avoidance probability](brownian-motion.md#boundary-derivative-is-an-excursion-avoidance-probability). Avoiding the larger hull is a subset of avoiding the smaller one, which proves the derivative inequality. For a hull contained in $\{|z|\leq R\}$ and $|x|>R$, comparison with the filled half-disc gives the sharp bound $1-R^2/x^2\leq g_A'(x)\leq1$, since that half-disc has [mapping-out function](#mapping-out-function-of-a-compact-h-hull) $z+R^2/z$. The empty hull and filled half-disc attain the two bounds.

#### Differentiability estimate for a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If a [compact H-hull](#compact-h-hull) lies in a disc of radius $r$ centred at $\xi\in\mathbb R$, the displayed estimate holds for $|z-\xi|>2r$, with an absolute constant $C$. It refines the Laurent expansion uniformly in the hull and supplies the first-order increment needed to derive the [Chordal Loewner equation](#chordal-loewner-equation) from the [Loewner local growth property](#loewner-local-growth-property).

#### High-level escape representation of a mapping-out height

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

Let $D=\mathbb H\setminus K$ and stop [planar Brownian motion](brownian-motion.md#planar-brownian-motion) from $z\in D$ on reaching height $R$ or leaving $D$. Then $\operatorname{Im}g_K(z)=\lim_{R\to\infty}R\mathbb P_z(\operatorname{Im}B_{\tau_R}=R)$. The stopped harmonic height is a bounded [martingale](martingale.md). The bounded difference $g_K(z)-z$ makes its top-boundary value differ from $R$ by a uniform constant, while optional stopping of the imaginary coordinate bounds the top exit probability by $\operatorname{Im}z/R$. Killing on the hull is essential.

#### Height contraction of a hydrodynamically normalized mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For a [compact H-hull](#compact-h-hull), $v(z)=\operatorname{Im}g_K(z)$ is harmonic and satisfies $0<v(z)\leq\operatorname{Im}z$. Local boundedness and the interior continuity of $g_K^{-1}$ show that $v$ tends to zero at every finite boundary point. The [maximum principle for harmonic functions](partial-differential-equation.md#maximum-principle-for-harmonic-functions) applied to $v-\operatorname{Im}z$, with an exhaustion controlling infinity through the Laurent expansion, proves the inequality without boundary smoothness.

#### Inverse-at-infinity criterion for local boundedness of a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

The inverse of a hydrodynamically normalized [mapping-out function](#mapping-out-function-of-a-compact-h-hull) has expansion $f(w)=w+O(1/w)$ at infinity. If bounded-domain points $z_n$ had unbounded images $w_n=g(z_n)$, then $z_n=f(w_n)=w_n+O(1/w_n)$ would be unbounded, a contradiction. Thus $g$ is bounded even near finite rough boundary points. Its own expansion at infinity then makes $g(z)-z$ uniformly bounded throughout the domain. Reflection is needed only near infinity, not along the entire hull boundary.

#### Mapping-out function of a vertical slit

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For the [compact H-hull](#compact-h-hull) $(x,x+ih]$, the square-root branch asymptotic to $z-x$ gives the [hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity) of its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull). Its expansion has coefficient $h^2/2$, the [half-plane capacity of a vertical slit](#half-plane-capacity-of-a-vertical-slit).

#### Real boundary bounds for a unit-disc H-hull

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If a [compact H-hull](#compact-h-hull) lies in the unit disc, compare its tail [harmonic measure](brownian-motion.md#harmonic-measure) with that of the empty hull and filled half-disc. The [Poisson kernel for the upper half-plane](partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) turns the inclusion of Brownian exit events into $x\leq g_K(x)\leq x+1/x$ for $x>1$. Reflection gives $x+1/x\leq g_K(x)\leq x$ for $x<-1$.

##### Sharp displacement bound for a compact H-hull

↑ **Parent:** [Real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull)

For a [compact H-hull](#compact-h-hull) inside the disc of radius $r$ centred at a real point, its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) displaces every point of its domain by at most $3r$. After scaling and translation, the [real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull) put the corresponding inverse boundary interval inside $[-2,2]$. Boundary cluster points of the inverse over this interval lie in the unit disc. The [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) applied to $w-g_K^{-1}(w)$ gives the bound without assuming [local connectedness](topology.md#locally-connected-space) of the hull. The [nearly closed semicircular slit](#nearly-closed-semicircular-slit) makes the constant three sharp.

###### Nearly closed semicircular slit

↑ **Parent:** [Sharp displacement bound for a compact H-hull](#sharp-displacement-bound-for-a-compact-h-hull)

With $m(z)=(z+1)/(1-z)$, the [compact H-hull](#compact-h-hull) $K_L=m^{-1}(i(0,L])$ is a unit semicircular arc attached at $-1$, with a narrow passage near $1$. As $L\to\infty$, its normalized [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) tends to $2$ at each fixed point of the interior bay. Points in that bay tending to $-1$ therefore have displacement approaching three. The order of these two limits is important.

#### Hydrodynamic normalization at infinity

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

A conformal map from an upper-half-plane domain has hydrodynamic normalization when $g(z)-z\to0$ at infinity. For a compact H-hull this normalization makes its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) unique.

#### Half-plane capacity

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Half-plane_capacity)

The half-plane capacity of a [compact H-hull](#compact-h-hull) is the nonnegative coefficient $a$ in

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

##### Half-plane capacity versus harmonic hull capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

The [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) is $\operatorname{hcap}(K)=\lim_{y\to\infty}y\mathbb E_{iy}\operatorname{Im}B_T$. The [harmonic capacity from infinity in the upper half-plane](brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane) uses $\operatorname{cap}(K)=\lim_{y\to\infty}\pi y\mathbb P_{iy}(B_T\in K)$. Since $0\leq\operatorname{Im}B_T\leq\operatorname{rad}(K)\mathbf1_{\{B_T\in K\}}$, the displayed bound follows. The normalization factor $\pi$ cannot be omitted. Independently, enclosure in a half-disc and [monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity) give the sharp bound $\operatorname{hcap}(K)\leq\operatorname{rad}(K)^2$.

##### Half-plane capacity of a half-disc

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $x\in\mathbb R$ and $R>0$, the filled half-disc $K=\{z\in\mathbb H:|z-x|\leq R\}$ is a [compact H-hull](#compact-h-hull). Its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) is $g_K(z)=z+R^2/(z-x)$. On the semicircle the image is real, and the inverse branch asymptotic to the identity maps the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) onto the exterior half-disc. Its [Laurent series](analysis.md#laurent-series) has coefficient $R^2/z$, so $\boxed{\operatorname{hcap}(K)=R^2}$. Using an open half-disc instead requires taking its relative [closure](topology.md#closure-topology) first.

##### Conformal change of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

Suppose a capacity-parameterized [Loewner chain](#loewner-chain) lies in a domain on which $\psi$ is a [conformal map](geometry-and-topology.md#conformal-map). For its image chain set $\psi_t=\widetilde g_t\circ\psi\circ g_t^{-1}$. Then the image [Loewner driving function](#loewner-driving-function) is $\widetilde U_t=\psi_t(U_t)$ and

$$
d\operatorname{hcap}(\widetilde A_t)=2\psi_t'(U_t)^2\,dt.
$$

The derivative is real by the [Schwarz reflection principle](complex-analysis.md#schwarz-reflection-principle). Cancellation of the pole in the differentiated conjugacy identity proves the squared-derivative rule.

###### Conformal conjugacy derivative for the chordal Loewner equation

↑ **Parent:** [Conformal change of half-plane capacity](#conformal-change-of-half-plane-capacity)

For conjugated [Loewner chains](#loewner-chain), $\phi_t=\widetilde g_t\circ\phi\circ g_t^{-1}$ and $\widetilde\xi_t=\phi_t(\xi_t)$. The image capacity speed is $2\phi_t'(\xi_t)^2$. Differentiating this identity gives $\dot\phi_t(z)=2\phi_t'(\xi_t)^2/(\phi_t(z)-\phi_t(\xi_t))-2\phi_t'(z)/(z-\xi_t)$. The removable singularity at the driver has value $-3\phi_t''(\xi_t)$.

###### Boundary derivative diffusion under conformal Loewner conjugacy

↑ **Parent:** [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)

Let $h_t$ intertwine two [Loewner chains](#loewner-chain), with driver $\xi_t=\sqrt\kappa B_t$, and set $a_t=h_t'(\xi_t)$, $b_t=h_t''(\xi_t)$, $c_t=h_t'''(\xi_t)$. Expanding the conjugacy equation at the driver gives $\partial_t h_t'(\xi_t)=b_t^2/(2a_t)-4c_t/3$; the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives the displayed diffusion. For a real exponent $p$, the drift of $a_t^p$ is $p[1+\kappa(p-1)]a_t^{p-2}b_t^2/2+p(\kappa/2-4/3)a_t^{p-1}c_t$. At $\kappa=8/3$, $p=5/8$ cancels both terms and yields the [SLE eight-thirds restriction martingale](#sle-eight-thirds-restriction-martingale).

###### Transformed SLE driving function

↑ **Parent:** [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)

Apply the [Itô formula](stochastic-calculus.md#ito-s-lemma) to the transformed [Loewner driving function](#loewner-driving-function) $\widetilde\xi_t=\phi_t(\sqrt\kappa W_t)$. The [conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation) cancels the Itô drift exactly when $\kappa=6$. Its [quadratic variation](stochastic-calculus.md#quadratic-variation) is $\kappa\int_0^t\phi_s'(\xi_s)^2ds$.

##### Half-plane capacity of a vertical slit

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For a vertical slit of height $h>0$ attached at $x\in\mathbb R$, the [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) is $g(z)=x+\sqrt{(z-x)^2+h^2}$, with the branch asymptotic to $z-x$ at infinity. Its [half-plane capacity](#half-plane-capacity) is $h^2/2$.

##### Scaling and translation of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $\lambda>0$ and $x\in\mathbb R$,

$$
g_{\lambda A+x}(z)=x+\lambda g_A\!\left(\frac{z-x}{\lambda}\right),
\qquad
\operatorname{hcap}(\lambda A+x)=\lambda^2\operatorname{hcap}(A).
$$

##### Monotonicity of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

If compact H-hulls satisfy $A\subseteq C$, then

$$
\operatorname{hcap}(A)\leq\operatorname{hcap}(C).
$$

This follows from the [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) or from composition of their mapping-out functions.

###### Half-plane-capacity composition rule

↑ **Parent:** [Monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity)

If compact H-hulls satisfy $A\subseteq C$ and $D$ is the bounded filling of $g_A(C\setminus A)$, then

$$
g_C=g_D\circ g_A,
\qquad
\operatorname{hcap}(C)
=\operatorname{hcap}(A)+\operatorname{hcap}(D).
$$

In particular, inclusion is strict exactly when the capacity increase is positive.

##### Brownian representation of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

If $\tau$ is the first exit time of planar [Brownian motion](brownian-motion.md) from $\mathbb H\setminus A$, then

$$
\operatorname{hcap}(A)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

It follows by applying the [optional sampling theorem for a supermartingale](martingale.md#optional-sampling-theorem-for-a-supermartingale) to the harmonic function $\operatorname{Im}(z-g_A(z))$.

##### Half-plane capacity is bounded by squared diameter

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

There is a universal constant $C$ such that every compact H-hull satisfies

$$
\operatorname{hcap}(A)\leq C\operatorname{diam}(A)^2.
$$

Translate and scale so the hull lies in a unit half-disc, then use the [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) and the $O(y^{-1})$ [harmonic measure](brownian-motion.md#harmonic-measure) of that half-disc as viewed from $iy$.

##### Half-plane capacity of a low rectangle

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $R_r=[-r,r]\times(0,1]$ with $r\geq1$,

$$
\operatorname{hcap}(R_r)\leq Cr.
$$

Indeed, the imaginary part at the Brownian exit point is at most one and the probability of reaching the radius-$O(r)$ neighbourhood containing the rectangle from $iy$ is $O(r/y)$. Consequently $r^{-1}R_r=[-1,1]\times(0,r^{-1}]$ has capacity $O(r^{-1})$ although its diameter tends to two.

##### Half-plane-capacity parameterization

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

A growing hull is parameterized by half-plane capacity when $\operatorname{hcap}(K_t)=2t$. The factor two makes its [Chordal Loewner equation](#chordal-loewner-equation) take the conventional form $\partial_tg_t=2/(g_t-U_t)$.

#### Boundary degeneration under a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If $z_n\in\mathbb H\setminus A$ approaches a point of a compact H-hull $A$, then

$$
\operatorname{Im}g_A(z_n)\longrightarrow0.
$$

The real part need not converge: the two sides of a vertical slit have distinct real boundary values under its mapping-out function.

## Loewner chain

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

A chordal Loewner chain is an increasing family of compact H-hulls, usually parameterized by [half-plane capacity](#half-plane-capacity), whose mapping-out functions evolve according to the [Chordal Loewner equation](#chordal-loewner-equation).

### Domain Markov property of a chordal Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

Conditionally on the entire past up to $t$, the future domains mapped and centered by $g_t-U_t$ have the original chain law and are independent of that past. For [Schramm–Loewner evolution](schramm-loewner-evolution.md) this follows from independent stationary [Brownian motion](brownian-motion.md) increments and the [composition rule for chordal Loewner driving functions](#composition-rule-for-chordal-loewner-driving-functions). The [Strong Markov property](markov-chain.md#strong-markov-property) gives the version at almost surely finite stopping times.

#### Simplicity of SLE from boundary-avoiding restarts

↑ **Parent:** [Domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain)

Suppose a chordal [SLE](schramm-loewner-evolution.md) trace stays in the open [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) at every positive time almost surely. For every deterministic rational time $s$, the [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain) makes its mapped and centered future a fresh SLE, so its positive-time future stays in the open half-plane as well. The inverse [mapping-out function](#mapping-out-function-of-a-compact-h-hull) then places that future outside the entire old hull. Intersecting these probability-one events over rational $s$ rules out every self-intersection: if two times $u<v$ shared a trace point, choose rational $s$ strictly between them. This proves simplicity using the allowed boundary-avoidance assertion for $0<\kappa\leq4$.

### Capacity-parametrized scale invariance of a Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

For a [Loewner chain](#loewner-chain) with [half-plane capacity](#half-plane-capacity) $2t$, scale invariance means $(\lambda^{-1}K_{\lambda^2t})_{t\geq0}$ has the original law for every $\lambda>0$. Its mapping-out maps are $\lambda^{-1}g_{\lambda^2t}(\lambda z)$ and its [Loewner driving function](#loewner-driving-function) is $\lambda^{-1}U_{\lambda^2t}$. This follows by differentiating the [Chordal Loewner equation](#chordal-loewner-equation). [Brownian scaling](brownian-motion.md#brownian-scaling) gives this property for [Schramm–Loewner evolution](schramm-loewner-evolution.md).

### Trace of a Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

When the indicated limit exists continuously and the hulls are generated by its past, it defines the trace of the [Loewner chain](#loewner-chain). The hull $K_t$ includes the curve up to time $t$ and any regions it disconnects from infinity. Therefore swallowing a point by $K_t$ is different from visiting that point by the [Loewner trace](#trace-of-a-loewner-chain). For [SLE](schramm-loewner-evolution.md), the continuous trace is part of its basic existence theory.

#### Boundary extension of the inverse map for a continuous Loewner trace

↑ **Parent:** [Trace of a Loewner chain](#trace-of-a-loewner-chain)

For a continuous [Loewner trace](#trace-of-a-loewner-chain) generating its hulls, the inverse [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) $g_t^{-1}$ extends continuously to the closed [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). The finite trace is a [continuous map](topology.md#continuous-map) image of an interval, and the [boundary](topology.md#boundary-of-a-set) of its unbounded complementary component has [local connectedness](topology.md#locally-connected-space); the [Caratheodory boundary extension theorem](riemann-surfaces.md#caratheodory-boundary-extension-theorem) gives the extension. In particular $g_t^{-1}(U_t)=\gamma(t)$, while $g_t^{-1}$ maps the open [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) into $D_t$. This is the deterministic boundary-extension input of [Rohde and Schramm, Theorem 4.1](https://annals.math.princeton.edu/wp-content/uploads/annals-v161-n2-p07.pdf). Under a [Conformal Markov property of SLE](#conformal-markov-property-of-sle) restart, this relates [boundary](topology.md#boundary-of-a-set) contacts of the mapped future to contacts with the old hull, without assuming the old trace is simple.

### Loewner local growth property

↑ **Parent:** [Loewner chain](#loewner-chain)

The local growth property says that, after mapping out the hull at time $t$, the new hull grown during a short interval has diameter tending uniformly to zero with the interval length. It ensures that the growth is described by one continuous boundary point.

#### Loewner correspondence theorem

↑ **Parent:** [Loewner local growth property](#loewner-local-growth-property)

An increasing family of [compact H-hulls](#compact-h-hull) of [half-plane capacity](#half-plane-capacity) $2t$ with the [Loewner local growth property](#loewner-local-growth-property) corresponds uniquely to a continuous real [Loewner driving function](#loewner-driving-function). Its [mapping-out functions](#mapping-out-function-of-a-compact-h-hull) solve the [Chordal Loewner equation](#chordal-loewner-equation) up to the maximal lifetime of each point. Conversely each continuous driver generates that hull family. A continuous [Loewner trace](#trace-of-a-loewner-chain) is an additional property, not a consequence for every continuous driver. For [SLE](schramm-loewner-evolution.md) it is supplied by the trace-existence theorem.

### Loewner differential equation

↑ **Parent:** [Loewner chain](#loewner-chain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loewner_differential_equation)

The Loewner differential equation describes a growing family of simply connected planar domains through ordinary differential equations for their normalized conformal maps.

#### Chordal Loewner equation

↑ **Parent:** [Loewner differential equation](#loewner-differential-equation)

For a capacity-parameterized locally growing hull family,

$$
\partial_tg_t(z)=\frac2{g_t(z)-U_t},
\qquad g_0(z)=z,
$$

where the continuous real function $U$ is the [Loewner driving function](#loewner-driving-function).

##### Loewner variation of the Dirichlet Green function

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

With [half-plane capacity](#half-plane-capacity) $2t$, $f_t=g_t-W_t$ and $G_{\mathbb H}(z,w)=\log|(z-\overline w)/(z-w)|$, differentiating $G_{D_t}(z,w)=G_{\mathbb H}(f_t(z),f_t(w))$ gives the displayed identity. The translation by the driver cancels in the Green function. This rank-one [covariance](variance.md#covariance) loss balances the quadratic covariation of the harmonic mean in the [SLE4 coupling with a Gaussian free field](gaussian-process.md#sle4-coupling-with-a-gaussian-free-field).

##### Boundary-point swallowing time for a Loewner chain

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

For a real point $b$ away from the initial driver, this is the maximal lifetime of the real solution $\partial_tg_t(b)=2/(g_t(b)-\xi_t)$. At finite lifetime its centred image collides with the [Loewner driving function](#loewner-driving-function). A point may be visited or separated from infinity by the hull, so swallowing is not the same as an individual trace visit.

###### SLE boundary swallowing criterion

↑ **Parent:** [Boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain)

For a continuous chordal [SLE](schramm-loewner-evolution.md) trace started at zero, hitting the real interval $[b,\infty)$ is equivalent to finite [boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain) at $b>0$. A boundary crosscut may swallow all points between its endpoints without visiting them individually. The [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) determines the probability of this event.

##### Interior-point swallowing time for a Loewner chain

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

For a continuous [Loewner driving function](#loewner-driving-function) $U$, $T_z$ is the maximal lifetime of $g_t(z)$ in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) under the [Chordal Loewner equation](#chordal-loewner-equation). A finite lifetime has $\operatorname{Im}g_t(z)\to0$ as $t\uparrow T_z$: otherwise the continuous driver and the [ordinary differential equation](differential-equation.md#ordinary-differential-equation) continue the solution. A swallowed point need not have been visited by the [Loewner trace](#trace-of-a-loewner-chain); it may lie in a disconnected pocket of the filled hull.

##### Loewner driving function

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

The Loewner driving function $U_t$ is the real boundary point at which the mapped-out hull grows. Scaling the hulls by $a^{-1}$ and time by $a^2$ transforms it to $a^{-1}U_{a^2t}$.

###### Continuity estimate for the Loewner driving function

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

Suppose the mapped increments $K_{s,t}$ have real-centred enclosing radii bounded by a nondecreasing modulus $\omega(t-s)\to0$. Nested closures define the unique growing real point $\xi_s$. For $v\in K_{t,t+h}$, its preimage $z=g_{K_{s,t}}^{-1}(v)$ belongs to $K_{s,t+h}$. The uniform displacement estimate for a [mapping-out function](#mapping-out-function-of-a-compact-h-hull) gives $|v-z|\leq C\omega(t-s)$, while $|z-\xi_s|\leq2\omega(t-s+h)$. Letting $h\downarrow0$ with $h\leq t-s$ proves the displayed estimate. It proves uniform [continuity](calculus.md#continuous-function) of the [Loewner transform](#loewner-driving-function) on each bounded time interval without evaluating a conformal map on a rough boundary.

###### Driving-function reconstruction for a chordal Loewner chain

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

The domains of a capacity-parametrized [Loewner chain](#loewner-chain) determine their hydrodynamically normalized [mapping-out functions of compact H-hulls](#mapping-out-function-of-a-compact-h-hull). At a surviving point, the [Chordal Loewner equation](#chordal-loewner-equation) gives $U_t=g_t(z)-2/\partial_tg_t(z)$. For a continuous driver and $t>0$, the left derivative uses only the hull past. High points $in$, $n\in\mathbb N$, survive up to any fixed finite time for sufficiently large $n$, making this a countable local reconstruction of the driver and its past filtration.

###### Composition rule for chordal Loewner driving functions

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

After time $t$, map remaining domains by $g_t-U_t$. The new [mapping-out function](#mapping-out-function-of-a-compact-h-hull) at elapsed time $s$ is $\widehat g_s(z)=g_{t+s}(g_t^{-1}(z+U_t))-U_t$. Direct differentiation of the [Chordal Loewner equation](#chordal-loewner-equation) proves that its driver is $U_{t+s}-U_t$, and its [half-plane capacity](#half-plane-capacity) is $2s$. Defining transformed hulls as complements of transformed domains avoids ambiguity at the old hull boundary.

###### Square-root Loewner driving function generates a straight slit

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

For the [Chordal Loewner equation](#chordal-loewner-equation) driven by $U_t=a\sqrt t$, the hull is a straight slit whose endpoint is proportional to $\sqrt t$. Put $r_\pm=(a\pm\sqrt{a^2+16})/2$ and $\alpha=-r_-/(r_+-r_-)\in(0,1)$. Its inverse map is

$$
f_t(w)=(w-r_+\sqrt t)^\alpha(w-r_-\sqrt t)^{1-\alpha},
$$

using upper-half-plane branches. The interval between the two real roots maps onto the two sides of a segment of argument $\pi\alpha$.

###### Boundary derivative of a chordal Loewner chain

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

For a real $x$ before its swallowing time,

$$
g_t'(x)=\exp\left(
-\int_0^t\frac{2\,ds}{(g_s(x)-U_s)^2}\right).
$$

It lies in $(0,1]$ and decreases with time.

## Scaling invariance of SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

For every $a>0$, if $(K_t)$ is $\operatorname{SLE}_\kappa$, then $(a^{-1}K_{a^2t})$ has the same law. Its driving function is $a^{-1}U_{a^2t}$, which has the same law as $U_t$ by [Brownian scaling](brownian-motion.md#brownian-scaling).

### SLE reaches every positive height

↑ **Parent:** [Scaling invariance of SLE](#scaling-invariance-of-sle)

For a chordal [SLE](schramm-loewner-evolution.md) trace $\gamma$, the [Scaling invariance of SLE](#scaling-invariance-of-sle) makes $\mathbb P(\sup_t\operatorname{Im}\gamma(t)>r)$ independent of $r>0$. The trace must enter the upper half-plane because its positive-time hull has positive [half-plane capacity](#half-plane-capacity). Letting $r\downarrow0$ therefore makes this probability one, and continuity implies that every positive height is reached. This argument does not assume [Transience of chordal SLE](#transience-of-chordal-sle).

## Conformal Markov property of SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

Conditionally on an $\operatorname{SLE}_\kappa$ initial segment through time $t$, mapping out that segment by $g_t-U_t$ turns the future into an independent $\operatorname{SLE}_\kappa$ in $(\mathbb H,0,\infty)$. This follows because its driving function is $U_{t+s}-U_t$, and [Brownian motion](brownian-motion.md) has [stationary increments](stochastic-process.md#stationary-increments) and [independent increments](stochastic-process.md#independent-increments).

### Characterization of the SLE driving function

↑ **Parent:** [Conformal Markov property of SLE](#conformal-markov-property-of-sle)

The conformal Markov property gives the continuous Loewner driver stationary independent increments. Scale invariance removes its deterministic drift. Therefore

$$
U_t=\sqrt\kappa B_t
$$

for a standard Brownian motion and a constant $\kappa\geq0$.

## Conformal invariance of SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

Chordal [SLE](schramm-loewner-evolution.md) is defined on any simply connected domain with two marked boundary points by applying a [conformal map](geometry-and-topology.md#conformal-map) from the upper half-plane. Its law is independent of the chosen map, up to a deterministic change of parameterization.

### Chordal SLE in a specified scale

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

A scale is a [conformal bijection](riemann-surfaces.md#biholomorphism) sending a marked starting boundary point to zero and target boundary point to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). A curve is [SLE](schramm-loewner-evolution.md) in that scale when its image is ordinary [SLE](schramm-loewner-evolution.md) using the [half-plane-capacity parameterization](#half-plane-capacity-parameterization) of that image.

### Chordal restriction property

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

A random curve $\gamma$ from $0$ to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) has the chordal restriction property when, for every admissible compact H-hull $A$ avoiding zero, the conditional law of $\psi_A(\gamma)$ given $\gamma\cap A=\varnothing$ equals the original law of $\gamma$. Here $\psi_A:\mathbb H\setminus A\to\mathbb H$ fixes zero and has derivative one at infinity.

#### Restriction exponent of a chordal filling

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

A conformally invariant random [chordal filling](#chordal-filling) has exponent $\alpha$ when its avoidance probability for every admissible hull $A$ is the displayed power, where $\Phi_A$ fixes zero and has derivative one at infinity. Composition of two hull-removing maps and the chain rule make conditional image avoidance probabilities the same as unconditional ones. The [avoidance probabilities determine a chordal filling law](#avoidance-probabilities-determine-a-chordal-filling-law) principle therefore implies the [chordal restriction property](#chordal-restriction-property). Independent unions followed by filling add exponents, since avoidance probabilities multiply.

#### Chordal filling

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

A chordal filling is the closed connected set obtained from a proper boundary-to-boundary path by adding complementary pockets disconnected from both boundary arcs between its marked endpoints. In $(\mathbb H,0,\infty)$ it meets the boundary only at zero and infinity and leaves two complementary simply connected sides, adjacent to the negative and positive real axes. Equivalently it is full with respect to the two marked boundary arcs. This definition uses the [prime ends](geometry-and-topology.md#prime-end) of a general simply connected domain and is preserved by [conformal maps](geometry-and-topology.md#conformal-map).

##### Avoidance probabilities determine a chordal filling law

↑ **Parent:** [Chordal filling](#chordal-filling)

The probabilities that a random [chordal filling](#chordal-filling) avoids each admissible [compact H-hull](#compact-h-hull) away from zero determine its law as an unparameterized closed set. Each point of its complement can be joined to the relevant real boundary arc through the complement and lies in a thin rational polygonal tube attached to that arc. These countably many hull tests recover the complement. Their joint avoidance events are tested by filled finite unions; if a union separates zero from infinity, the joint avoidance event is empty. Otherwise connectedness makes avoidance of the union equivalent to avoidance of its filled hull. Thus individual hull probabilities give every finite joint indicator distribution and determine the random complement.

#### Derivative avoidance criterion for chordal restriction

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

Suppose a random proper [simple curve](topology.md#simple-curve) from zero to infinity has the displayed avoidance probability for every admissible [compact H-hull](#compact-h-hull) $A$, with fixed $\alpha>0$. Put $\psi_A=g_A-g_A(0)$. For another admissible hull $B$ in the image [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), map composition and the [chain rule](calculus.md#chain-rule) give $g_C'(0)=g_B'(0)g_A'(0)$ for $C=A\cup\psi_A^{-1}(B)$. The conditional image curve therefore has avoidance probabilities $g_B'(0)^\alpha$, exactly those of the original. Since [avoidance probabilities determine a simple chordal curve law](#avoidance-probabilities-determine-a-simple-chordal-curve-law), the conditional image law agrees with the original. This is the [chordal restriction property](#chordal-restriction-property).

#### Avoidance probabilities determine a simple chordal curve law

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

For random proper [simple curves](topology.md#simple-curve) from $0$ to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), the probabilities of avoiding every [compact H-hull](#compact-h-hull) whose [closure](topology.md#closure-topology) excludes zero determine the unparameterized trace law. Every point off a simple chordal curve can be [connected](geometry-and-topology.md#connected-space) to a real [boundary](topology.md#boundary-of-a-set) interval away from zero within one side of its complement. A countable collection of thin rational polygonal tubes attached to that interval therefore recovers the complement from its avoidance indicators. Joint avoidance of finitely many tubes reduces to avoidance of their filled union. If the union blocks every path from zero to infinity the joint event is empty; otherwise filling pockets does not change the avoidance event. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) gives all finite indicator distributions. These determine the random complement and hence the trace. Simplicity and properness are hypotheses; the assertion is not a general determination theorem for arbitrary random closed sets.

#### SLE eight-thirds restriction martingale

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

For chordal $\operatorname{SLE}_{8/3}$ and an admissible hull $A$, let $\psi_t$ map out the image of $A$ after removing the SLE hull. Then

$$
M_t=\psi_t'(U_t)^{5/8}
$$

stopped when the trace meets $A$ is a bounded martingale. Its terminal value yields the avoidance probability

$$
\mathbb P(\gamma\cap A=\varnothing)=\psi_A'(0)^{5/8}.
$$

### Locality property of SLE

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

The locality property says that an [SLE](schramm-loewner-evolution.md) does not detect a hull lying away from its starting point until the curve reaches that hull. Among chordal Schramm-Loewner evolutions, this property holds for $\operatorname{SLE}_6$.

#### Locality of a chord law under conformal changes of neighborhoods

↑ **Parent:** [Locality property of SLE](#locality-property-of-sle)

A scale-invariant law of unparameterized chords from zero to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) is local when a boundary-preserving [conformal map](geometry-and-topology.md#conformal-map) between neighborhoods of zero, fixing zero, transports its curve stopped on leaving the first neighborhood to the same-law curve stopped on leaving the second. Equality concerns the stopped curves up to increasing reparameterization. For [SLE](schramm-loewner-evolution.md) with parameter six, the [transformed SLE driving function](#transformed-sle-driving-function) is a [continuous local martingale](martingale.md#continuous-local-martingale) with bracket six times the image capacity clock. The [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion) makes that driver Brownian in the new clock, proving the local stopped-curve invariance.

#### Target-change locality of SLE6

↑ **Parent:** [Locality property of SLE](#locality-property-of-sle)

Changing the target boundary point by a [conformal automorphism of the upper half-plane](complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) preserves the local chordal [SLE](schramm-loewner-evolution.md) law at parameter six, up to a capacity time change and until the relevant boundary point is swallowed. The [transformed SLE driving function](#transformed-sle-driving-function) has zero drift at six; the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) makes it Brownian in image capacity time.

##### Target-dependent continuation of SLE6

↑ **Parent:** [Target-change locality of SLE6](#target-change-locality-of-sle6)

At parameter six, changing a boundary target preserves the initial unparameterized [SLE](schramm-loewner-evolution.md) law until the growing hull separates the two possible targets. After separation, each curve continues in the complementary component whose boundary contains its own target. A curve targeted at infinity follows the unbounded component, whereas a finite separated target lies on a different component. The [target-change locality of SLE6](#target-change-locality-of-sle6) proof no longer applies: its [conformal automorphism of the upper half-plane](complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) conjugates corresponding surviving domains only before this separation. A zero drift before contact does not give equality of complete curve laws afterwards.

## Phase classification of the SLE trace

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

The trace of $\operatorname{SLE}_\kappa$ is [simple](topology.md#simple-curve) for $0<\kappa\leq4$, has self-intersections without being [space-filling](topology.md#space-filling-curve) for $4<\kappa<8$, and is space-filling for $\kappa\geq8$. The thresholds arise from the [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) and estimates for the [Loewner chain](#loewner-chain) near its driving point.

### Space-filling SLE above parameter eight

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For $\kappa>8$, the [Loewner trace](#trace-of-a-loewner-chain) visits every point of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) almost surely. Choose $\rho=\kappa-8$ in the [SLE interior-point martingale](#sle-interior-point-martingale) to obtain $M_t=\Upsilon_t^{(\kappa-8)/8}S_t^{-(\kappa-8)/\kappa}$. The [maximal inequality for a nonnegative supermartingale](martingale.md#maximal-inequality-for-a-nonnegative-supermartingale) bounds its running supremum. If a fixed [interior](topology.md#interior-topology) ball were avoided, its center would have $\Upsilon_t\geq c_1>0$ before swallowing, forcing $S_t\geq c_2>0$. But the [Chordal Loewner equation](#chordal-loewner-equation) gives $dY_t^2/dt=-4S_t^2$, forcing a finite lifetime with $Y_t\to0$, and $d\log\Upsilon_t/d\log Y_t=2S_t^2$ then forces $\Upsilon_t\to0$, a contradiction. Countably many rational balls give a dense trace; [continuity](calculus.md#continuous-function) and [Transience of chordal SLE](#transience-of-chordal-sle) make its image relatively closed, so it is all of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). This argument does not cover the critical parameter eight.

### SLE Green-function estimate

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For $0<\kappa<8$, the probability that chordal $\operatorname{SLE}_\kappa$ approaches an interior point $z$ to conformal radius at most $\epsilon$ is, on compact subsets of $\mathbb H$, comparable to

$$
G_\kappa(z)\epsilon^{1-\kappa/8},
$$

where $G_\kappa$ is the SLE Green function. The positive exponent implies that the trace has zero planar [Lebesgue measure](measure-theory.md#lebesgue-measure).

### SLE4 left-passage probability

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For chordal $\operatorname{SLE}_4$ in $(\mathbb H,0,\infty)$,

$$
\mathbb P(\gamma\text{ passes to the right of }z)
=\frac{\arg z}{\pi}.
$$

Indeed, $\arg(g_t(z)-U_t)$ is a bounded martingale whose terminal value is zero or $\pi$ according to the side on which the trace passes.

### Boundary-intersection threshold for SLE

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

Chordal $\operatorname{SLE}_\kappa$ intersects the domain boundary away from its endpoints exactly when $\kappa>4$. The centered image of a boundary point is a Bessel process of dimension $1+4/\kappa$, which hits zero exactly below dimension two.

#### Positive boundary-interval hitting probability for SLE above parameter four

↑ **Parent:** [Boundary-intersection threshold for SLE](#boundary-intersection-threshold-for-sle)

For $\kappa>4$, the [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) and the [SLE boundary swallowing criterion](#sle-boundary-swallowing-criterion) imply that the full [Loewner trace](#trace-of-a-loewner-chain) hits the positive real axis almost surely. Every fixed open interval in that axis has positive hitting probability: its countably many dilates cover the axis, while [Scaling invariance of SLE](#scaling-invariance-of-sle) makes all their hitting probabilities equal. Reflection gives the corresponding negative-axis statement. Together with the [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain), this produces visits to the old [Loewner trace](#trace-of-a-loewner-chain) boundary in a mapped future domain.

## Transience of chordal SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

The chordal [SLE](schramm-loewner-evolution.md) [Loewner trace](#trace-of-a-loewner-chain) eventually leaves every bounded subset of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). For $0<\kappa<4$, its time-one [compact H-hull](#compact-h-hull) is a simple slit and does not contain a half-disc. Instead, the [boundary approach forces a small SLE Bessel gap](#boundary-approach-forces-a-small-sle-bessel-gap) estimate shows that every fixed nonzero real point is outside the closure of the full [Loewner trace](#trace-of-a-loewner-chain). After mapping out the initial simple slit, the starting point has two distinct real [prime end](geometry-and-topology.md#prime-end) images. A fresh independent [SLE](schramm-loewner-evolution.md) avoids approaching either image, so the original future stays a positive distance from its starting point. [Scaling invariance of SLE](#scaling-invariance-of-sle) gives $\inf_{t\geq T}|\gamma(t)|\overset d=\sqrt T\inf_{t\geq1}|\gamma(t)|$, and decreasing-event continuity proves escape from every fixed disc. The separate argument based on a swallowed half-disc at positive time applies in the nonsimple regime $\kappa>4$; it must not be applied to a simple slit. The critical parameters require their own limiting or trace-existence arguments.

## Reverse Loewner flow

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

For a continuous driver $U$ and terminal time $T$, the reverse Loewner flow solves

$$
\partial_sh_s(z)=-\frac2{h_s(z)-(U_{T-s}-U_T)},
\qquad h_0(z)=z.
$$

It satisfies $h_T(z)=g_T^{-1}(U_T+z)-U_T$.

### Reverse SLE derivative martingale

↑ **Parent:** [Reverse Loewner flow](#reverse-loewner-flow)

For the reverse $\operatorname{SLE}_\kappa$ flow, write $X_s+iY_s=h_s(z)-(U_{T-s}-U_T)$. Then

$$
M_s=|h_s'(z)|^2\left(1+\frac{X_s^2}{Y_s^2}\right)^{4/\kappa}
$$

is a nonnegative [local martingale](martingale.md#local-martingale) and hence a [supermartingale](martingale.md#supermartingale).

#### Reverse SLE derivative bound above the space-filling threshold

↑ **Parent:** [Reverse SLE derivative martingale](#reverse-sle-derivative-martingale)

If $\kappa>8$, then for every $0<\alpha<(1-8/\kappa)/2$ and fixed $T$, there is an almost surely finite random $C$ such that

$$
|h_T'(x+iy)|\leq Cy^{-1+\alpha}
$$

for $|x|\leq1$ and $0<y\leq1$. The proof combines the derivative martingale, [Markov inequality](probability-inequality.md#markov-s-inequality), a dyadic lattice, the [Borel-Cantelli lemmas](probability-theory.md#borel-cantelli-lemmas), and the [Koebe distortion theorem](riemann-surfaces.md#koebe-distortion-theorem).

## Boundary-point Bessel flow for SLE

↑ **Parent:** [Schramm–Loewner evolution](schramm-loewner-evolution.md)

For chordal $\operatorname{SLE}_\kappa$, the centered image of a real boundary point, divided by $\sqrt\kappa$, evolves as a [Bessel process](brownian-motion.md#bessel-process) of dimension

$$
d=1+\frac4\kappa.
$$

Its first hit of zero is the time at which the point is swallowed by the Loewner hull.

### Boundary approach forces a small SLE Bessel gap

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $0<\kappa<4$ and $x>0$, stop the simple chordal [SLE](schramm-loewner-evolution.md) trace on first entering the radius-$r$ half-disc about $x$, with $r<x/4$. A crosscut from its tip to $x$ separates the positive-side boundary arc containing $x/2$ from infinity. [Harmonic measure](brownian-motion.md#harmonic-measure) comparison with the half-disc bounds the length of that arc's mapped interval, $g_t(x/2)-\xi_t$, by a universal constant times $r$. This centered boundary image is a positive [Bessel process](brownian-motion.md#bessel-process) of dimension $1+4/\kappa>2$ and has a strictly positive all-time minimum. Hence the full trace stays a positive distance from each fixed nonzero real point. Reflection gives the negative-side version.

### SLE two-boundary-point ratio diffusion

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $0<x<y$, let $D_t=g_t(y)-g_t(x)$. Before the first [boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain), the ratio obeys

$$
dZ_t=-\frac{\sqrt\kappa}{D_t}d\beta_t+\frac2{D_t^2}\left(\frac1{Z_t}+\frac1{Z_t-1}\right)dt.
$$

The clock $u=\int D_t^{-2}dt$ removes the denominator. An increasing [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) is $s_\kappa(z)=\int_1^z[v(v-1)]^{-4/\kappa}dv$. For $\kappa>4$ the endpoint $1$ represents strict swallowing; escape at infinite clock represents simultaneous swallowing.

#### Strict ordering threshold for SLE boundary swallowing

↑ **Parent:** [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion)

For $\kappa\geq8$, almost surely the positive-boundary swallowing times satisfy $T(x)<T(y)$ simultaneously for every $0<x<y$. The [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion) has unbounded scale, ruling out escape before hitting $1$. For $4<\kappa<8$, its total scale $S_\kappa$ is finite, and the simultaneous-swallowing probability is $s_\kappa(y/(y-x))/S_\kappa$. At $\kappa=4$, fixed positive points have infinite swallowing times.

##### Real-line visitation from strict SLE swallowing order

↑ **Parent:** [Strict ordering threshold for SLE boundary swallowing](#strict-ordering-threshold-for-sle-boundary-swallowing)

A continuous capacity-parameterized [Loewner trace](#trace-of-a-loewner-chain) with finite, strictly ordered positive swallowing times visits every positive real point. An unvisited swallowed point has an interval disjoint from the compact trace up to its swallowing time; that interval is swallowed simultaneously, contradicting strict order. Reflection yields the negative-axis conclusion for chordal [SLE](schramm-loewner-evolution.md) at $\kappa\geq8$.

### SLE boundary-point logarithmic separation diffusion

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For two boundary points $1<r$, let $V_t^x=g_t(x)-U_t$ and set $Z_t=\log(V_t^r-V_t^1)-\log V_t^1$. After the clock $q(u)=\int_0^u(V_s^1)^{-2}ds$, the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) gives

$$
d\widetilde Z_t=\sqrt\kappa\,dW_t+\left(\frac{\kappa-4}{2}-\frac2{1+e^{\widetilde Z_t}}\right)dt.
$$

This one-dimensional [diffusion process](stochastic-calculus.md#markov-diffusion) compares the swallowing times of nearby boundary points.

#### SLE does not hit a fixed nonzero boundary point

↑ **Parent:** [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion)

For every $x\in\mathbb R\setminus\{0\}$, the probability that a chordal $\operatorname{SLE}_\kappa$ trace in $(\mathbb H,0,\infty)$ passes through $x$ is zero. The [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion) shows that the chance for $x$ to be swallowed strictly before a nearby point tends to zero as that point approaches $x$; [Scaling invariance of SLE](#scaling-invariance-of-sle) and reflection then handle every nonzero $x$.

### Two-sided SLE boundary swallowing probability

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $1<d<2$, couple Bessel flows $X>0>Y$ with the same Brownian motion and let $v=x/y<0$. Then

$$
\mathbb P(\tau_x>\tau_y)=\frac{\displaystyle\int_v^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}}{\displaystyle\int_{-\infty}^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}}.
$$

It is the probability that the SLE hull swallows the chosen point on the negative side before the point on the positive side.

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process.md)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (12)

- [Capacity-parametrized scale invariance of a Loewner chain](#capacity-parametrized-scale-invariance-of-a-loewner-chain)
- [Cardy boundary crossing formula](#cardy-boundary-crossing-formula)
- [Domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain)
- [Fixed-interior-point avoidance of SLE4](#fixed-interior-point-avoidance-of-sle4)
- [Logarithmic martingale for SLE4](#logarithmic-martingale-for-sle4)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-203.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#3/a/solution)
- [Scale-and-domain-Markov characterization of SLE](#scale-and-domain-markov-characterization-of-sle)
